In this repo I will write my notes about websockets and I will do a project with websockets.

# Topics

## What are websockets?

The WebSocket API is an advanced technology that makes it possible to open a two-way interactive communication session between the user's browser and a server. With this API, you can send messages to a server and receive event-driven responses without having to poll the server for a reply

### Benefits
- Wire traffic efficient - incur less traffic than http
- no CORS
- simple API
- Bidirectional
- Real-time
- Widely available

### Challenges
- State management
- Backpressure
- Load balancing

## Why are websockets invented?
WebSockets initiate continuous, full-duplex communication between a client and WebSocket server. This reduces unnecessary network traffic, as data can immediately travel both ways through a single open connection. This provides speed and realtime capability on the web.

## What are the alternatives?
- Polling - Good for big data, not good for small amount of data
- SSE
- WebRTC

## How are websockets designed?
Before a client and server exchange data, they must use the TCP layer to establish the connection. Using their WebSocket protocol, webSockets effectively run as a transport layer over the TCP connection.  
Once connected through an HTTP request/response pair, the clients can use an HTTP/1.1 upgrade header to switch their connection from HTTP to WebSockets. WebSocket connection is established through a WebSocket handshake over the TCP. During a new WebSocket handshake, the client and server also communicate which subprotocol will be used for subsequent interactions. After this is established, the connection will run on the WebSocket protocol.

### Some notes:

**REST vs WebSockets?**
REST wanky solution is *short polling* but it's very inefficient
In WS on application load both applications of A and B users establish a connection to the server.


Measuring performance
