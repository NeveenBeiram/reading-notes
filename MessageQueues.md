# Message Queues

1. What does it mean that web sockets are bidirectional? Why is this useful?

Whereas HTTP relies on a client request to receive a response from the server for every exchange,
WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates
asynchronously, without requiring the client to submit a request each time. In the context of networked AV and control
systems, this allows devices to send and receive continuous streams of data to and from any point on the network.
[source](https://www.amx.com/en/site_elements/benefits-and-applications-of-websockets)

2. Does socket.io use HTTP? Why?

yes,Even when websockets can be used, the initial connection setup it done over HTTP. Also, a socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js.

That said, although you don't need an HTTP server to regular websockets, there's no denying that the websocket protocol was designed with HTTP in mind (as to allow HTTP and websocket servers to co-exist on the same TCP port).
[source](https://stackoverflow.com/questions/37836130/socket-io-why-does-it-need-an-http-server#:~:text=The%20premise%20on%20which%20your,%2C%20which%20it%20isn't.&text=Even%20when%20websockets%20can%20be,%2Fsocket.io.js%20.)

3. What happens when a client emits an event?

when the server is listening to that event, the server will execute the handler function for that event.

4. What happens when a server emits an event?

All listening clients will execute the handler for that event.(sends the data)

5. What happens if a client “misses” an event?

for that event will not execute the handler function for it

6. How can we mitigate this?
using messaging queueing

<hr>


## Term

- Socket: A socket is one endpoint of a two-way communication link between two programs running on the network.
 A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to.
[source](https://docs.oracle.com/javase/tutorial/networking/sockets/definition.html#:~:text=A%20socket%20is%20one%20endpoint,destined%20to%20be%20sent%20to.&text=Every%20TCP%20connection%20can%20be%20uniquely%20identified%20by%20its%20two%20endpoints.)

- Web Socket:WebSocket is bidirectional, a full-duplex protocol that is used in the same scenario of client-server communication, unlike HTTP it starts from ws:// or wss://. It is a stateful protocol, which means the connection between client and server will keep alive until it is terminated by either party (client or server). after closing the connection by either of the client and server, the connection is terminated from both the end.

- Socket.io:Socket.IO enables real-time, bidirectional and event-based communication.

- Client: hardware or software that accesses a remote service on another computer

- Server:A server is a computer program or device that provides a service to another computer program and its user, also known as the client. In a data center, the physical computer that a server program runs on is also frequently referred to as a server. That machine might be a dedicated server or it might be used for other purposes.

- OSI Model:The OSI Model (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software. In the OSI reference model, the communications between a computing system are split into seven different abstraction layers: Physical, Data Link, Network, Transport, Session, Presentation, and Application.

- TCP Model:The TCP/IP model (Transmission Control Protocol/Internet Protocol) is a model with four layers which is for both modelling current Internet architecture, as well as providing a set a rules that govern all forms of transmission over a network

- TCP:Transmission Control Protocol (TCP) is one of the main protocols of the Internet protocol suite. It originated in the initial network implementation in which it complemented the Internet Protocol (IP). Therefore, the entire suite is commonly referred to as TCP/IP. TCP provides reliable, ordered, and error-checked delivery of a stream of octets (bytes) between applications running on hosts communicating via an IP network.

- UDP:User Datagram Protocol (UDP) is one of the core members of the Internet protocol suite. With UDP, computer applications can send messages, in this case referred to as datagrams, to other hosts on an Internet Protocol (IP) network. Prior communications are not required in order to set up communication channels or data paths.

- Packets:A packet is a small amount of data sent over a network, such as a LAN or the Internet. Similar to a real-life package, each packet includes a source and destination as well as the content (or data) being transferred. When the packets reach their destination, they are reassembled into a single file or other contiguous block of data.

While the exact structure of a packet varies between protocols, a typical packet includes two sections — a header and payload. Information about the packet is stored in the header.

<hr>


## Preparation Materials

[Socket.io Chat Example](https://socket.io/get-started/chat/)

[Rooms and Namespaces](https://socket.io/docs/rooms-and-namespaces/)

[Socket.io Emit Cheatsheet](https://socket.io/docs/emit-cheatsheet/)