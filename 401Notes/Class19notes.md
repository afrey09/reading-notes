AWS: Events

AWS SQS vs SNS

1. What is the difference betweeen SQS and SNS?
- SNS..
   Is a distributed publish-subscribe service
   Fast, flexible fully managed push notification service
   Supports several end points

   "Key Differences
      Entity Type
      SQS : Queue (similar to JMS, MSMQ).
      SNS : Topic-Subscriber (Pub/Sub system).

      Message consumption
      SQS : Pull Mechanism — Consumers poll messages from SQS.
      SNS : Push Mechanism — SNS pushes messages to consumers.

      Persistence
      SQS : Messages are persisted for some duration is no consumer available. The retention period value is from 1 minute to 14 days. The default is 4 days.
      SNS : No persistence. Whichever consumer is present at the time of message arrival, get the message and the message is deleted. If no consumers available then the message is lost.

      In SQS the message delivery is guaranteed but in SNS it is not.

      Consumer Type
      SQS : All the consumers are supposed to be identical and hence process the messages in exact same way.
      SNS : All the consumers are (supposed to be) processing the messages in different ways."

      - SQS..
        Is fully mananged distributed queuing service
        Messages not pushed to receivers but can be stored for a short duration of time (max 14 days)
        Messages can't be received by multiple receivers at the same time
   


2. What are some use cases for both SNS and SQS?

    "Choose SNS if:

    You would like to be able to publish and consume batches of messages.
    You would like to allow same message to be processed in multiple ways.
    Multiple subscribers are needed.
    Choose SQS if:

    You need a simple queue with no particular additional requirements.
    Decoupling two applications and allowing parallel asynchronous processing.
    Only one subscriber is needed."


source: https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5

AWS SNS and SQS

1. Describe how to use SQS and SNS in a “fanout” pattern.

    "We can design fanout pattern by using both SNS and SQS. In this pattern, a message published to an SNS topic is distributed to multiple SQS queues in parallel."

    "You can also use fanout to replicate data sent to your production environment with your test environment. Expanding upon the previous example, you can subscribe another SQS queue to the same SNS topic for new incoming orders. Then, by attaching this new SQS queue to your test environment, you can continue to improve and test your application using data received from your production environment."

2. Explain how “push notifications” work, using SNS.    
    "Amazon Simple Notification Service (SNS) sends notifications two ways, A2A and A2P. A2A provides high-throughput, push-based, many-to-many messaging between distributed systems, microservices, and event-driven serverless applications. These applications include Amazon Simple Queue Service (SQS), Amazon Kinesis Data Firehose, AWS Lambda, and other HTTPS endpoints. A2P functionality lets you send messages to your customers with SMS texts, push notifications, and email. "
    
source:
    https://docs.aws.amazon.com/sns/latest/dg/sns-common-scenarios.html
    https://www.youtube.com/watch?v=mXk0MNjlO7A



SQS and SNS Basics

1. How might a large scale, distributed application make use of a Queue system like SQS?

source:
https://www.youtube.com/watch?v=UesxWuZMZqI
https://aws.amazon.com/blogs/aws/scaling-with-amazon-sqs/