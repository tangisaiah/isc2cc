Chapter 4 Network Security
---------

## Module 1: Understand Computer Networking
### What is Networking
A network is simply **two or more computers linked together** to share data, information or resources.

### Types of Networks
* Local area network (LAN) - A network typically spanning a single floor or building. This is commonly a limited geographical area.
* Wide area network (WAN) - Long-distance connections between geographically remote networks.

### Network Devices
* Hub: Hubs are used to connect multiple devices in a network, not smart.
* Switch: Intelligent hub know the addresses of the devices connected to them and route traffic to that port/device rather than broadcast. Can create VLANs
* Router: Connect similar networks and control traffic flow between them. Connect multiple switches.
* Firewall: Controlling (filter) network traffic and protecting the network.
* Server: Provides information to other computers on a network. 
* Endpoints: Client

### Networking Models
Those simple goals can be re-expressed in network (and security) terms such as:
* Provide reliable, managed communications between hosts (and users)
* Isolate functions in layers
* Use packets as the basis of communication
* Standardize routing, addressing and control
* Allow layers beyond internetworking to add functionality
* Be vendor-agnostic, scalable and resilient

### Open Systems Interconnection (OSI) Model
* To establish a **common way** to describe the communication structure for interconnected computer systems.
* Theoritical model, abstract framework

![Images/osi.svg]

Example:
* When someone references an image file like a JPEG or PNG, we are talking about the Presentation Layer (6). 
* When discussing logical ports such as NetBIOS, we are discussing the Session Layer (5).
* When discussing TCP/UDP, we are discussing the Transport Layer (4).
* When discussing routers sending packets, we are discussing the Network Layer (3). 
* When discussing switches, bridges or WAPs sending frames, we are discussing the Data Link Layer (2). 
* Physical Layer (1) the data unit is converted into binary, i.e., 01010111

#### Terminology
* **Payload**: The primary action of a malicious code attack.
* ** Encapsulation**: Bundling data and methods, can also refer as packing or hiding in another data structure.
* **de-encapsulation**: The opposite process of encapsulation, in which bundles of data are unpacked or revealed.

### TCP/IP
* Most widely used protocol
* Developed in the early 1970s
* A protocol stack comprising dozens of individual protocols
* Consume a lot resources
* Easy to hack as designed for ease of use only
* TCP: full-duplex connection-oriented protocol
* UDP: simplex connectionless protocol

Layer | Description |
------|-------------|
Application Layer | Defines the protocols for the transport layer |
Transport Layer | Permits data to move among devices |
Internet Layer  | Creates/inserts packets |
Network Interface Layer | How data moves through the network |

![Images/tcpip.svg]

### Internet Protocol (IPv4 and IPv6)
IPv4:
* 32-bit
* Not enough addresses
* 127.0.0.1 is reserved for loopback
* IPsec is optional

Private IP:
Range |
------|
10.0.0.0 to 10.255.255.254 |
172.16.0.0 to 172.31.255.254  |
192.168.0.0 to 192.168.255.254  |

IPv6:
* 128-bit
* Solution for not enough addresses
* Improved security as IPsec is mandatory
* Can be shorten: 2001:0db8:0000:0000:0000:ffff:0000:0001 -> 2001:db8::ffff:0:1

### Security of the Network
* DDoS attack: The **prevention of authorized access to resoures** or the delaying of time-critical operations
* Fragment attack: An attacker **fragments traffic** in such a way that a system is **unable to put data packets back together**.
* Purposely sending a network packet that is **larger than can be handled** by the receiving system, causing the receiving system to **fail** unexpectedly.
* MITM attack: An attacker where positions himself **in between the user and the system** so that he can **intercept and alter** data travelling between them.
* Sniffing: Passive, act of **monitoring traffic patterns** to obtain information about a network.

### Ports and Protocols (Applications/Services)
* Physical Ports: On routers, switches, servers, computers, etc
* Logical ports: 
	* Used between two systems to communicate or establish connection
	* Socket: ip address + port 
	* Port: Allow multiple simultaneous communications for single IP
	* **Well-known (0-1023)**: Common protocols. e.g. SMTP, DNS, SSH
	* **Registered ports (1024-49151)**: Proprietary applications from vendors and developers.Approved by IANA.
	* **Dynamic or private ports (49152-65535)**: Used for connecting well-known or registered ports.Released once session ends.
	
### Secure Ports
* Some network protocols transmit information in clear text
* Not encrypted


Insecure Port | Description | Protocol | Secure Alternative | Protocol |
--------------|-------------|----------|--------------------|----------|
21 - FTP | Sends the username and password using plaintext | File Transfer Protocol | 22 - SFTP | Secure File Transfer Protocol |
23 - Telnet | Not encrypted (Plaintext) | Telnet | 22 - SSH | Secure Shell |
25 - SMTP | Unencrypted port for sending email messages | Simple Mail Transfer Protocol | 587 - SMTP | SMTP with TLS |
37 - Time | Legacy. NTP has better error-handling and reduces likelihood of unexpected erros | Time Protocol | 123 - NTP | Network Time Protocol |
53 - DNS | Not encrypted (Plaintext) | Domain Name Service | 853 - DoT | DNS over TLS (DoT) |
80 - HTTP | Not encrypted (Plaintext) | HyperText Transfer Protocol | 443 - HTTPS | HyperText Transfer Protocol (SSL/TLS) |
143 - IMAP | retrieving emails, not encrypted (Plaintext) | Internet Message Access Protocol | 993 - IMAP | 	IMAP for SSL/TLS |
161/162 - SNMP | used for managing infrastructure devices, it is recommended to use SNMP version 2 or 3 to include encryption and additional security features. | Simple Network Management Protocol | 161/162 - SNMP | SNMPv3 |
445 - SMB | Files are transmitted unencrypted, and many vulnerabilities are well-known | Server Message Block |  Block	2049 - NFS | Network File System |
389 - LDAP | Used to communicate directory information from servers to clients, not encrypted | Lightweight Directory Access Protocol | 636 - LDAPS | 	Lightweight Directory Access Protocol Secure |

