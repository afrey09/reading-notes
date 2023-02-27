Event Driven Applications

What native Node.js module allows us to get started with Event Driven Programming?

  EventEmitter

What is the value of Object Oriented Programming used in tandem with Event Driven Programming?

  "By registering event listeners we can actually reverse the flow of communication between our objects. Rather than on object needing to reach inside another object to trigger a function, our objects can just emit events and whichever objects are listening to those event will process it in the way they have been told to. The source of an objects behavior is now entirely contained within itself, rather than needing to be accessed by external objects."

Consider your knowledge of Event Driven Programming in the Web Browser, now explain to a non-technical friend how Event Driven Programming might be useful on the backend using Node.js.

  It helps to avoid issues of complexity and collision by having a way to trigger specific events and have listeners that specifically listen to those events only. It makes the communication from the front and back ends more fluid and free of errors.
  
source:https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming