1. What is an IP address? (100 words)
An IP address  idetifies a node in a network, functioning like a phone number.
• Why do we need IP addresses? 
We need IP adresses to properly route data packets to their correct destinations across the network.

• What is the relation between TCP and IP?
TCP is built on top of IP. While IP handles the adressing and routing of packets, TCP ensures the reliable ordered delivery of those packets.

• What is a socket? Have you heard of different types of sockets?
A socket is a sftware endpoint for communication between two machines, which is bound to a port number so the TCP layer can identify the correct target. Different types of sockets include TCP, UDP, and Raw sockets.

• What is up with the address: 127.0.0.1?
This is a special IP address known as a localhost, which is used to establish a connection to the exact same machine you are using.

2. What does a client-server architecture mean? (150 words)
A client-server architecture separates a system into two main components that communiacate via request/reply protocol. This structure centralizes the management of shared resources to improve the availability, and modifiability. It is also called a 2-tier architecture. That can be generalised to more tiers

• Give a concrete example of where you would encounter this in real life.
The lecture mention e-mail, calendars, and collaborative documents (as SaaS). For example Google Docs, here the serveer hosts and manages the document file. When you make edits to the text or write in it, then your client will send an "request" with the the edits to the server. Then the server proccesses these edits, updates the central file, and sends "replies" back to all the other users' clients so everyone sees the updates.


• How do you decide who is the server and who is the client?
You decide based on their roles. The server is the component that hold, manages, and provides access to shared resources and services. The client is the component that initiates requests to consume those services

3. What is the difference between client-server architecture and the broker architecture?
(100 words)
In a standard client-server architecture, clients and servers interact directly. In a broker architecture, an the broker is inserted between them.

• What are the benefits to the broker pattern?
The benefits are the client remains completely ignorant of the servers identity, location, and characteristics. If a server goes down, the broker can chose a replacement without breaking the clients connection.

• What could be potential downsides?
The downsides is that it introduces complexity, as systems often require additional proxies or bridges to translate data and protocols.

4. What does Peer-to-Peer mean? (150 words)
Peer-to-Peer is an architecture that conneccts a set of identical distributed computational entities using a common protocol to share services

• What are the main characteristics of this architecture?
All peers are eqaual and interact directly. No single peer is critical for the health of the network.

• Have you encountered it anywhere online?
For file sharing and instants messaging

• Does Peer-to-Peer applications mean that there are no servers and only clients?
No, it means every peer acts as both the client and the server simulataneously using the same protocol.

• What benefits could there be to using this pattern?
That there is high availability and scalability, beacuse peers can be added or removed from the network without having a significant impact.

• What downsides could there be to this pattern?
The downsides is that discovering other peers can be difficult because search requests are only dispearsed for a limited number of steps. It often requires specialized peers to handle routing and indexing to search larger portions of the network.