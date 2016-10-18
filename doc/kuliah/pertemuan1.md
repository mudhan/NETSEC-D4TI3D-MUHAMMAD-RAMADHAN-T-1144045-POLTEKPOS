TCP / IP
TCP / IP (stands for Transmission Control Protocol / Internet Protocol) is a data communications standard used by the Internet community in the process of exchanging data from one computer to another computer on the network Internet. This protocol can not stand alone, because this protocol is a set of protocols (protocol suite) .Protokol is also the most widely used protocol today. The data are implemented in software (software) operating system. The term given to this software is the TCP / IP stack. TCP / IP is always evolving over time, given the increasing demand for computer networks and the Internet. The development is carried out by several agencies, such as the Internet Society (ISOC), the Internet Architecture Board (IAB) and Internet Engineering Task Force (IETF). Various protocols running on atasTCP / IP addressing scheme, and the concept of TCP / IP is defined in documents called Request for Comments (RFC) issued by IETF.

OSI Layer
OSI reference model of open networks or OSI Reference Model for open networking is a network architectural model developed by the agency the International Organization for Standardization (ISO) in Europe in 1977. OSI itself is an acronym for Open Systems Interconnection. This model is also called the model "seven layer OSI Model" (OSI seven layer model).
Before the advent of the OSI reference model, the computer network system is dependent upon suppliers (vendors). OSI seeks to establish a common standard computer networks to support interoperability between different suppliers. In a large network there are usually many different network protocols. The absence of a similar protocol, making many devices can not communicate with each other.
OSI Reference Model has seven layers, which is as follows:
Ke- coating layer Name Description
7 Application layer
Serves as an interface to applications with network functionality, manage how applications can access the network, and then create error messages. Protocols that are in this layer are HTTP, FTP, SMTP, and NFS.

6 Presentation layer
Serves to translate the data to be transmitted by the application into a format that can be transmitted over the network. Protocols that are in this level is software redirektor (redirector software), such as the Workstation service (in Windows NT) and Network shell (such as Virtual Network Computing (VNC) or Remote Desktop Protocol (RDP)).

5 Session Layer
Serves to define how connections can be created, maintained, or destroyed. In addition, at this level also carried the name resolution.
4 Transport layer
Serves to break down the data into packets of data and provide the serial number of all packets so that they can be rearranged on the side of the goal after receipt. In addition, at this level also makes a sign that the packet is received successfully (acknowledgment), and terhadp retransmit lost packets in the middle of the road.
3 Network layer
Serves to define the IP addresses, create the header for the packets, and then perform routing through internetworking using routers and layer-3 switches.

2 Data-link layer
Befungsi to determine how the bits of data grouped into a format called a frame. In addition, at this level of error correction, flow control, addressing hardware (such halnyaMedia Access Control address (MAC address)), and determine how the network devices sepertihub, bridge, repeater, and a layer 2 switch operates. IEEE 802 specification, this level divides into two child level, the layer Logical Link Control (LLC) and Media Access Control layer (MAC).

1 Physical layer
Serves to define the network transmission medium, signaling methods, bit synchronization, network architecture (such as Ethernet or Token Ring), network topology and cabling. In addition, this level also defines how the Network Interface Card (NIC) can interact with the media cable or radio.



ARP
Abbreviated Address Resolution Protocol ARP is a protocol within the TCP / IP Protocol Suite responsible in conducting IP address resolution into a Media Access Control address (MAC address).
ARP is a protocol that serves ipaddress mapped into a MAC address. He is the link between the data link layer and IP layer in TCP / IP. All Ethernet-based communication uses this ARP protocol. Essentially any computer or device that will communicate will surely make transactions or exchange of related information between IP and MAC address. Each transaction will be stored in the cache of your OS. Can be viewed using the arp command (either in Windows or Linux).
However, this protocol has serious limitations, because each computer can only provide transaction ARP packet is manipulated. By changing the actual MAC address. This weakness utilized for these types of attacks ARP Poisoning or ARP spoofing or Man In The Middle Attack. Anyone can tap even to kill an active connection to the LAN!
