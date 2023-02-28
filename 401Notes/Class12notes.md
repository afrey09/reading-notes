Socket.io

Web Sockets

What is a Web Socket?
  "A computer communications protocol, providing full-duplex communication channels over a single TCP connection."

Describe the Web Socket request/response handshake and what happens once the connection is established.
  "To establish a WebSocket connection, the client sends a WebSocket handshake request, for which the server returns a WebSocket handshake response, as shown in the example below"

Web Sockets provide a standardized way for the server to send content to a client without first receiving a __request__ from that client.


Socket.io Tutorial

What does the event handler io.on() do? "io.on event handler handles connection, disconnection, etc., events in it, using the socket object."

Describe some possible proof of life or proof that the code works as expected.
  console.logs an emitted event 

What does socket.emit() do? Create and fire custom events 

Socket.io vs Web Sockets

What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).
  "WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

  Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.

  Client-Side: it is the library that runs inside the browser
  Server Side: It is the library for Node.js"

When would you use Socket.IO?
  For online gaming

When would you use WebSockets?
  For creating real-time applications that have two-way communication between two network systems 

Videos
OSI Model Explained

What are a couple of key takeaways from this video?
  OSI Model has seven layers that are transferring data: application, presentation, session, transport, network, data link and physical.

TCP Handshakes Explained
  3-way handshake:

  Part 1. The client sends a SYN segment to the server, asking for synchronization
  Part 2. The server replies with SYN-ACK (synchronization and acknowledgment)
  Part 3. The client replies with ACK, which is like YES and then the two way connection is established.

sources:
https://en.wikipedia.org/wiki/WebSocket
https://www.tutorialspoint.com/socket.io/
https://www.educba.com/websocket-vs-socket-io/
https://www.youtube.com/watch?v=vv4y_uOneC0
https://www.youtube.com/watch?v=xMtP5ZB3wSk
