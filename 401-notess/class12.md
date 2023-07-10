**A Web Socket:**
1. A Web Socket is a communication protocol that provides full-duplex communication channels over a single TCP connection.
2. It enables real-time, two-way communication between a client (typically a web browser) and a server.

**Web Socket Request/Response Handshake and Connection:**
- The Web Socket handshake begins with an HTTP-based request from the client to the server, called the Web Socket handshake request.
  - This request includes an HTTP header called "Upgrade" with a value of "websocket" to indicate the client's intention to establish a WebSocket connection.
- If the server supports Web Sockets, it responds with a Web Socket handshake response.
  - The server includes the same "Upgrade" header in the response along with other necessary headers to complete the handshake.
  - If the handshake is successful, the connection is upgraded from HTTP to Web Socket.
- Once the Web Socket connection is established, it transitions from the HTTP protocol to the WebSocket protocol.
  - The connection remains open, allowing bidirectional communication between the client and the server.
  - Both the client and server can send messages to each other asynchronously without the need for continuous HTTP requests/responses.

**Web Sockets vs. HTTP Request/Response:**
- Web Sockets provide a standardized way for the server to send content to a client without first receiving a request (or "polling") from that client.
- With traditional HTTP, the server can only send content as a response to a client's request.
- Web Sockets enable real-time, push-based communication where the server can initiate communication and send data to the client at any time.

**Socket.io:**
- `io.on()` is an event handler in the Socket.io library.
  - It listens for events on the server-side and allows you to define actions to be performed when those events occur.
- Possible proof of life or proof that the code works as expected in Socket.io can include:
  - Testing the connection establishment between the server and client.
  - Emitting events from the server and verifying that the client receives them.
  - Implementing specific functionality and verifying that it behaves correctly.
- `socket.emit()` is a method in Socket.io that allows the server to send a custom event with data to a specific client or all connected clients.
  - It emits an event from the server that can be listened to on the client side.

**Difference between WebSocket and Socket.IO:**
- WebSocket is a low-level communication protocol that provides a standardized way for two endpoints (client and server) to establish a full-duplex communication channel over a single TCP connection.
- Socket.IO is a JavaScript library that provides a higher-level abstraction over WebSocket and other fallback transports.
  - It offers additional features like real-time event-based communication, automatic reconnection, and support for older browsers.
  - Socket.IO simplifies working with WebSocket by providing a unified API and handling various transport mechanisms.

**When to Use Socket.IO:**
- Use Socket.IO when you need real-time, event-driven communication between the server and clients.
- It is suitable for scenarios where you want to support older browsers or require additional features like automatic reconnection, fallbacks, and rooms/namespace management.

**When to Use WebSockets:**
- Use WebSocket directly (without Socket.IO) when you need a low-level, lightweight, and efficient protocol for real-time, bidirectional communication between a client and server.
- WebSocket is a good choice for performance-critical applications or when you have specific protocol requirements that Socket.IO does not fulfill.
 ## What are a couple of key takeaways from this video? 
 there are 7 layers of OSI that organise and authinticates connection between computers and are runnignt he hole wide web
 ## Translate the gist of this video to a non-technical friend
 TCP three way hand shake is a way to make both parties sequnize with each other by  doing a 3 step operation where they add one to the id of eachother send a bracket.
