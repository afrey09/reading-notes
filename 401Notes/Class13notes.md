Message Queues

Socket.io Chat Example

1. Explain to a non-technical recruiter what the Chat Example (above) does. 
  It creates a messaging application where users can send and receive messages in real-time through the use of socket.io.

2. What proof of life are we getting on the backend from the above app? listening on the designated port

3. Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket? The broadcast flag

Rooms

1. What is a room and how might a room be useful? "A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients"

2. How do you join a room? You call join to subscribe the socket

3. how do you leave a room? You can call leave in the same way you used join

Namespaces

1. What is a Namespace and what does it allow you to do? "A Namespace is a communication channel that allows you to split the logic of your application over a single shared connection (also called "multiplexing")."

2. Each namespace potentially has its own what? (hint: 3 things)
    - events handlers
    - rooms
    - middlewares
3. Discuss a possible use case for separate namespaces
    To provide different abilities depending on the role or namespace

sources:
https://socket.io/get-started/chat/
https://socket.io/docs/v4/rooms
https://socket.io/docs/v4/namespaces/
