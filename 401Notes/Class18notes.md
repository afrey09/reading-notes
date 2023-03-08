AWS: API, Dynamo and Lambda

AWS API Gateway Overview

1. What is Amazon API Gateway?
  "Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic."

2. Why is Amazon API Gateway an important part of the Serverless ecosystem?
  "API Gateway is the piece that ties together Serverless functions and API definitions. Being able to trigger the execution of a Serverless function directly in response to an HTTP request is the key reason why API Gateway is so valuable in Serverless setups"

3. How does API Gateway integrate with other AWS services?
  "...it enables a truly serverless architecture for web applications. When using API Gateway together with other AWS services, it’s possible to build a fully functional customer-facing web application without maintaining a single server yourself."

AWS API Gateway

1. What are the some benefits of using Amazon API Gateway?
  - fully managed service
  - allows you to create RESTful APIs and WebSocket APIs with real-time two-way communication app
  - handles all tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls
  - has no minimum fees or startup costs

2. What two API types might you choose from?
  - RESTful and WebSocket

AWS DynamoDB Guide

1. What is DynamoDB? "a hosted NoSQL database offered by Amazon Web Services (AWS)"
2. Under what circumstances would you recommend DynamoDB over MongoDB?
  - For applications with large amounts of data and strict latency requirements
  - For serverless applications using AWS Lambda
  - For data sets wtih simple, known access paterns.
AWS DynamoDB

1. Explain to a non-technical friend how DynamoDB works.
  - It is a database offered through AWS

Dynamoose

1. What is Dynamoose? A modeling tool for Amazon's DynamoDB
2. What are some key features of Dynamoose? 
    Type safety
    High level API
    Easy to use syntax
    DynamoDB Single Table Design Support
    Ability to transform data before saving or retrieving items
    Strict data modeling (validation, required attributes, and more)
    Support for DynamoDB Transactions
    Powerful Conditional/Filtering Support
    Callback & Promise support
    AWS Multi-region support

Sources:
https://www.serverless.com/guides/amazon-api-gateway
https://aws.amazon.com/api-gateway/
https://www.dynamodbguide.com/what-is-dynamo-db/
https://aws.amazon.com/dynamodb/
https://dynamoosejs.com/getting_started/Introduction