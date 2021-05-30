# Socket.io

- What is the benefit of transforming data into packets?

A packet is a small amount of data sent over a network, such as a LAN or the Internet. Similar to a real-life package, each packet includes a source and destination as well as the content (or data) being transferred. When the packets reach their destination, they are reassembled into a single file or other contiguous block of data.

While the exact structure of a packet varies between protocols, a typical packet includes two sections — a header and payload. Information about the packet is stored in the header.

Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data, sending smaller packets helps ensure each section is transmitted successfully. If a packet is not received or is dropped, only the dropped packet needs to be resent.

- UDP is often refereed to as a connectionless protocol. Why is this?

Connectionless protocols, in contrast, allow data to be exchanged without setting up a link between processes. Each unit of data, with all the necessary information to route it to the intended destination, is transferred independent of other data packets and can travel over different paths to reach the final destination. Some data packets might be lost in transmission or might arrive out of sequence to other data packets.

UDP is a connectionless protocol. It is known as a datagram protocol because it is analogous to sending a letter where you don't acknowledge receipt.

Examples of applications that use connectionless transport services are broadcasting and tftp. Early implementations of NFS used UDP, whereas newer implementations prefer to use TCP.

- Can a socket server application have multiple socket connections?

For a stateless protocol (ie UDP), there is no problem because "connections" don't exist - multiple people can send packets to the same port, and their packets will arrive in whatever sequence. Nobody is ever in the "connected" state.

For a stateful protocol (like TCP), a connection is identified by a 4-tuple consisting of source and destination ports and source and destination IP addresses. So, if two different machines connect to the same port on a third machine, there are two distinct connections because the source IPs differ. If the same machine (or two behind NAT or otherwise sharing the same IP address) connects twice to a single remote end, the connections are differentiated by source port (which is generally a random high-numbered port).

Simply, if I connect to the same web server twice from my client, the two connections will have different source ports from my perspective and destination ports from the web server's. So there is no ambiguity, even though both connections have the same source and destination IP addresses.

Ports are a way to multiplex IP addresses so that different applications can listen on the same IP address/protocol pair. Unless an application defines its own higher-level protocol, there is no way to multiplex a port. If two connections using the same protocol simultaneously have identical source and destination IPs and identical source and destination ports, they must be the same connection.


- Can a socket connection application be connected to multiple socket servers?

A server socket listens on a single port. All established client connections on that server are associated with that same listening port on the server side of the connection. An established connection is uniquely identified by the combination of client-side and server-side IP/Port pairs. Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.

On the client-side, it is common practice for new outbound connections to use a random client-side port, in which case it is possible to run out of available ports if you make a lot of connections in a short amount of time.

- Can an application be both a socket server and a socket connection?

Yes you can have socket app for both socket-server and socket connection.

## Term: 

- Observer Pattern: is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.

- Listener:An event listener is a procedure in JavaScript that waits for an event to occur.

- Event Handler: function runs when a specific event fires

- Event Driven Programming:is a programming paradigm in which the flow of program execution is determined by events - for example a user action such as a mouse click, key press, or a message from the operating system or another program. An event-driven application is designed to detect events as they occur, and then deal with them using an appropriate event-handling procedure. 

- Event Loop: is a programming construct or design pattern that waits for and dispatches events or messages in a program. The event loop works by making a request to some internal or external "event provider" (that generally blocks the request until an event has arrived), then calls the relevant event handler ("dispatches the event"). The event loop is also sometimes referred to as the message dispatcher, message loop, message pump, or run loop.

The event-loop may be used in conjunction with a reactor, if the event provider follows the file interface, which can be selected or 'polled' (the Unix system call, not actual polling). The event loop almost always operates asynchronously with the message originator.

- Event Queue:Recall that the operating system interacts with the run-time support for the programming language to pass on events such as keystrokes and mouse movements. These are automatically resolved into high level events in terms of the components being manipulated by the program, such as buttons

- Call Stack:is a stack data structure that stores information about the active subroutines of a computer program. This kind of stack is also known as an execution stack, program stack, control stack, run-time stack, or machine stack, and is often shortened to just "the stack". Although maintenance of the call stack is important for the proper functioning of most software, the details are normally hidden and automatic in high-level programming languages. Many computer instruction sets provide special instructions for manipulating stacks.


- Emit/Raise/Trigger: All these three mean firing the event, which is telling the event listener that the event is fired, then the listener activates the handler.

- Subscribe: waiting for the events to take a place in the event loop cycle.

- database:an organized collection of data, generally stored and accessed electronically from a computer system.



## Additional Resources 


The OSI Model (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software. In the OSI reference model, the communications between a computing system are split into seven different abstraction layers: Physical, Data Link, Network, Transport, Session, Presentation, and Application.


[OSI Model Explained](https://www.youtube.com/watch?v=vv4y_uOneC0)

[TCP Handshakes Explained](https://www.youtube.com/watch?v=xMtP5ZB3wSk)


[Web Sockets](https://en.wikipedia.org/wiki/WebSocket)

[Socket.io Tutorial](https://www.tutorialspoint.com/socket.io/)

[Socket.io vs Web Sockets](https://www.educba.com/websocket-vs-socket-io/)


[Socket.io Documentation](https://socket.io/docs/)

[Socket.io Server API](https://socket.io/docs/server-api)

[Socket.io Client API](https://socket.io/docs/client-api)

[Socket Testing Tool](https://amritb.github.io/socketio-client-tool/)
