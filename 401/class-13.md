# 401 - Class 13 Reading Notes

---

## REVIEW, RESEARCH, DISCUSSION

1. What does it mean that web sockets are bidirectional? Why is this useful?
- The bidirectionality of websockets means that each device in the two way connection can send and receive data. It does not require one to be the requester and one to be the responder.
- This is useful in many ways, but one example is the low latency/fast response time this type of connection affords.

2. Does socket.io use HTTP? Why?
- Yes, it does. In the initial handshake. Socket.io is more than a standard websocket, it contains more metadata.

3. What happens when a client emits an event?
- When a client emits an event it is picked up by the server. If the sever is listening for that event, it will trigger some predefined code to run.

4. What happens when a server emits an event?
- When a sever emits an event it is picked up by any connected clients. If the clients are listening for that event, it will trigger some predefined code to run.

1. What happens if a client “misses” an event?
- If the event is missed because the client is not connected, and we are not checking, it will be missed. Client to server will be buffered until reconnected. 

2. How can we mitigate this?
  - Check server side if a specific client is connected.

--- 

## Vocabulary Terms

  - Socket: A socket is an endpoint of a communication between two programs running on a network. Sockets are used to create a connection between a client program and a server program.

  - Web Socket: A web socket is more or less the same, but a socket could be physically connected whereas websocket endpoints would communicate via the internet or using internet technologies.

  - Socket.io: Socket.IO is a library that enables real-time, bidirectional and event-based communication between the browser and the server.

  - Client: Client is an endpoint in a network, it may be user facing or another computer, but it is not the central node in a network.

  - Server: A server traditionally will be the central point serving data to the endpoints. It brokers/stores/communicates data for it's clients.

  - OSI Model: See Picture

  ![OSI]('./OSI.JPG')

  - TCP Model: See Picture

  ![TCP]('./TCP.JPG')

  - TCP: Transmission Control Protocol (TCP) is a standard that defines how to establish and maintain a network conversation by which applications can exchange data.

  - UDP: User Datagram Protocol (UDP) is a communications protocol that is primarily used to establish low-latency and loss-tolerating connections between applications on the internet. UDP speeds up transmissions by enabling the transfer of data before an agreement is provided by the receiving party.

  - Packets: Packets are the basic units of communication over a TCP/IP network. Devices on a TCP/IP network divide data into small pieces, allowing the network to accommodate various bandwidths, to allow for multiple routes to a destination, and to retransmit the pieces of data which are interrupted or lost.

## Resources

[Resource](https://www.cloudflare.com/learning/network-layer/what-is-a-packet/)
[Resource](https://www.techtarget.com/searchnetworking/definition/TCP)
[Resource](https://www.geeksforgeeks.org/tcp-ip-model/)
[Resource](https://socket.io/get-started/chat)
[Resource](https://socket.io/docs/v4/emitting-events/)
[Resource](https://www.amx.com/en/site_elements/benefits-and-applications-of-websockets)
[Resource](https://docs.oracle.com/javase/tutorial/networking/sockets/definition.html)
[Resource](https://www.geeksforgeeks.org/what-is-web-socket-and-how-it-is-different-from-the-http/)
[Resource](https://zetcode.com/javascript/socket/)