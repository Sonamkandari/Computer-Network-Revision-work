# Computer-Network-Revision-Work
---
# Resource : https://www.youtube.com/watch?v=IPvYjXCsTg8
---
## How did it start? (History of the Internet)

- There are some rules set by people about how particular data is to be sent. These rules are called **protocols**:  
  - IP Protocol  
  - UDP Protocol  
  - TCP/IP Protocol  

- **This is the world's first website**:  
  - `WWW.com` – commonly known as the Web (World Wide Web) was invented by Tim Berners-Lee.  
  - The WWW allows you to access different documents and links.  
  - The World Wide Web (WWW) is a global system of interconnected webpages and information resources, accessed via the Internet, linked together by hyperlinks and identified by URLs. It is part of the Internet (not the same thing) and allows users to easily find and share information by surfing through different web pages using a web browser.

- When the WWW was invented, there were no search engines. Users could only go from one hyperlink to another.  

- Yahoo was one of the first services to introduce the concept of a **search engine**.

---

## Protocols

### Q1. What are protocols?
**Answer:** A protocol in computer networks is a set of rules that defines how two or more devices communicate with each other.

### Q2. Why do we need protocols?
**Answer:** Without protocols, devices would be like two people speaking completely different languages. They wouldn't understand when to talk, when to listen, or how to recognize valid information.

**We need protocols to:**  
- **Enable communication** → Devices from different vendors can talk if they follow the same rules.  
- **Provide structure** → Defines how data is packaged, addressed, transmitted, and received.  
- **Maintain security** → Encryption, authentication, and integrity checks rely on protocols.  

---

### How do protocols work?

Protocols work by defining rules at each layer of communication. For example, if you send a WhatsApp message:  

- **Application layer protocol (HTTP, SMTP, etc.)** – Defines the format of the message.  
- **Transport protocol (TCP/UDP)** – Decides how data is split into packets and reassembled.  
- **Network protocol (IP)** – Adds source and destination addresses to each packet.  
- **Link/Physical layer (Ethernet, Wi-Fi, etc.)** – Handles actual transmission over wires or air.  

When the message reaches the other device, the same layers (in reverse) decode the data.

---

### Why are protocols required?

Protocols are required because they provide:  

- **Interoperability** → A Windows PC can talk to a Linux server because both use the same networking protocols (like TCP/IP).  
- **Standardization** → Organizations like IEEE, IETF, and ISO define global standards so every device follows the same rules.  
- **Efficiency** → They manage data flow, avoid collisions, and optimize bandwidth usage.  
- **Error handling** → Protocols detect and correct errors in transmission.  

---

### Examples of common protocols

- **HTTP/HTTPS** → For browsing websites.  
- **SMTP/IMAP/POP3** → For email.  
- **FTP/SFTP** → For file transfer.  
- **TCP/IP** → The foundation of the Internet.  
- **DNS** → Converts domain names (like google.com) into IP addresses.  

---

### Internet Society

To request adding your idea to the Internet standards, you must write a document called **RFC (Request for Comments)**.

---

### Server and Client

- **Server:** A device or program that provides services to other devices (clients).  
- **Client:** A device or program that requests services from a server.

---

![Computer Network Image](https://github.com/user-attachments/assets/52f2177c-a816-459b-ac85-79d6da3f1f52)

---

## what are IP Address
<img width="776" height="306" alt="image" src="https://github.com/user-attachments/assets/1ccae5cf-0b8e-4919-8764-09346f8233e0" />

* for example every website is associated with an ip address
* or a domain name is always linked to a IP address

# <img width="696" height="463" alt="image" src="https://github.com/user-attachments/assets/f32cc76e-891d-4ec0-84a4-3ee97025abf1" />
* NET - Network access translator

* A router knows that which device had been sent the request but how will it know that which application has sent the request
  ## important note
* An IP address decides which device should receive the data, but a port number decides which application on that device should  receive it.
* Since a single device can send many requests to a server, the port number is used to identify which application sent the request, so the server can reply correctly to the right application.

* The IP address tells us the location of your computer, while the port number tells us which application on your computer is being used.

# prorts
* ports are 16 bit numbers
---
# If two people are using the same application to communicate with each other, will their IP addresses be the same or different? Also, will their port numbers be different?
ChatGPT said:

-> Great question 👍 Let’s break it down clearly:
1. IP Address
Yes, the two people will usually have different IP addresses.
If they are on different networks (e.g., one at home, one at office), their public IP addresses will be different.
If they are on the same Wi-Fi network, they will have the same public IP (the router’s IP) but different private/local IPs inside that network.
2. Port Numbers
Yes, their port numbers will also be different.
Port numbers are used by the operating system to identify which application/process is handling a particular communication.
Even if both are using the same chat app, the OS assigns a different temporary (ephemeral) port for each connection.
👉 Example analogy:
Think of the IP address as the street address of a building (which building to deliver to).
The port number is like the apartment number (which person inside the building to deliver to).
Two people chatting are in different apartments (ports), possibly in different buildings (IPs).

---
* TCP -> Transmission control protocol it will ensure that data will reached to its destination without any interuption  or not get corrupted in middle of the data transmission process
* UDP ->**User datagram protocol** : UDP (User Datagram Protocol) is a fast, connectionless, and lightweight network protocol that sends data without establishing a dedicated connection or ensuring delivery and order, making it ideal for real-time applications where speed matters more than reliability.
* HTTP -> Hyper text transfer protocol -> this defines the format of data transmission between your web clients


---
# How data is Transffered?
Data transfer means moving digital information (bits of 0s and 1s) from one device or system to another — like sending a message, downloading a file, or streaming a video.
<img width="724" height="565" alt="image" src="https://github.com/user-attachments/assets/5de007da-1d61-4cd5-8904-1f4123147bbb" />
---
# Data will be tranffered into packets
---
## What are Packets
- Packets are small, formatted units of data that are sent over a network to transmit larger messages. They are the fundamental building blocks of data communication on the internet and consist of a header (containing destination and source information), a payload (the actual data), and a footer (with error-checking information). When a large message is sent, it is broken into multiple packets, sent independently, and then reassembled in the correct order by the receiving device

--- 
# Information about Ports
## we know that web pages are using which protocol that is a HTTP protocol
##  Note
** Ports are chosen either by a standard organization or by the computer itself. Common services (like websites and emails) use standard port numbers set by rules, while temporary connections get random numbers picked by the computer

* HTTP = 80 (it has a fixed port number)
*Mongodb=2707 (it also has a fixed port)
# Note  
* ports from 0-1023 these are reserved ports we cannot use them only
* 1024 - 49152 are also reserved for applications

  <img width="814" height="189" alt="image" src="https://github.com/user-attachments/assets/ec4fe2f7-bba9-4fc7-befe-b92722bda396" />

---
* how Intenet is connected world wide Or How countries are connected - using submarine cables
* Submarine cable map
* Physically: Optical fibre cables, coaxial cables
* wireless : Blutooth , wifi, 3G,4G and 5G
* 
# WHy we use cables under the oceans why we don't use settlelight?
* Beacuse through cables internet transffered faster compare to the sattlelight
  
---
* LAN : Loacal area network (like small house/office -> your phone wifi is connected to your to your office or building wifi but it can be only connected for a certain range like 10 m to 20m ),Ethernets and wifi
* PAN : Personal area network (like health monitoring sensors are connected to your phone blutooth for transmatting the data
* MAN : Metropolean Area network (Across the city)
* WAN : Across Countries (It allow users to connect over countries ) like for example you are travelling from your home country to a * new country but you can still connected to your network through roaming facility
---
## OR

# Types of Networks

## 🌐 LAN (Local Area Network)
- A network within a small area like a **house, office, or building**.  
- Devices (phones, laptops, printers) connect through **Wi-Fi** or **Ethernet cables**.  
- Range is usually limited (**10–100 meters** depending on Wi-Fi strength).  

## 📱 PAN (Personal Area Network)
- A very small network around a **person**.  
- Example: **smartwatch or health sensors** connect to your phone via **Bluetooth** or **NFC** to transfer data.  

## 🏙️ MAN (Metropolitan Area Network)
- A larger network that covers a **city or big campus**.  
- Connects multiple **LANs** together.  
- Example: a **city's cable TV or broadband network**.  

## 🌍 WAN (Wide Area Network)
- A network that spans **countries and continents**.  
- The **Internet** is the biggest WAN.  
- When you travel abroad and use **roaming**, you are still accessing the WAN through your mobile operator.
- SONET -> Synchronouse optical network
- frame Relay : A way to connect your local area to the wide area network
  
# Extra Networking Technologies

## 🔦 SONET (Synchronous Optical Network)
- A **standard for transmitting data over optical fiber**.  
- Works like a **highway system for data**, synchronizing huge amounts of traffic (voice, video, internet).  
- Used by telecom companies for **fast, reliable, long-distance communication**.  

## 📦 Frame Relay
- A **WAN technology** (older, but important historically).  
- Works like a **postal service for data packets**: breaks information into **frames** and sends them across a shared network.  
- Was cheaper and faster than older methods, but today is mostly replaced by **MPLS, fiber, and broadband**.  

---

## 🔎 Comparison Table

| Network Type | Coverage Area       | Example                           |
|--------------|---------------------|-----------------------------------|
| **PAN**      | Around one person   | Phone ↔ Smartwatch (Bluetooth)    |
| **LAN**      | Building/office     | Home Wi-Fi, Office LAN            |
| **MAN**      | City / large campus | City-wide broadband, cable TV     |
| **WAN**      | Country / World     | The Internet, Mobile Roaming      |

---
# MODEM , ROUTER
- A MODEM can convert your digital data into electrical signal so that we can transmit into the other MODEM  to the another side 
- Router : A router routes data based on there IP Address
- 
---
# 📡 Network Topologies
# Network Topologies

## Bus
- All devices share a **single cable**.  
- **Advantages:** Cheap, easy to set up.  
- **Disadvantages:** If the cable fails, the whole network goes down; performance decreases with more devices.  

## Ring
- Devices are connected in a **circular path**.  
- **Advantages:** Equal access, fewer collisions.  
- **Disadvantages:** One failure can break the entire network; harder to troubleshoot.  

## Star
- All devices connect to a **central hub or switch**.  
- **Advantages:** Easy to manage and expand; one device failure doesn’t affect others.  
- **Disadvantages:** If the central device fails, the entire network stops; requires more cabling.  

## Hybrid topology
Definition: A hybrid topology is the combination of two or more different network topologies to create a network that leverages the strengths of each.
Examples: A star-bus topology (two or more star networks connected by a bus backbone) or a star-ring topology are common examples of a hybrid network.
Purpose: Used to balance traffic flow, improve fault tolerance, or connect different types of existing networks. 
## Tree topology
**Definition**: A tree topology is a specific type of hybrid topology that combines a main bus backbone with several star networks branching off of it, forming a hierarchical structure.
Structure: It can be viewed as a collection of star networks arranged in a hierarchy, with the bus serving as the main trunk.
Purpose: It offers excellent scalability and a logical layout for large organizations, making it easier to manage and troubleshoot. 
## Mesh
- **Every device is connected to every other device**.  
- **Advantages:** Highly reliable and fault-tolerant.  
- **Disadvantages:** Very expensive; complex and difficult to scale.  

---

--- 
# Structure of the Networks
  - Application layer ->
    # OSI MODEL - Open system interconnection model : why it is developed ?
    
  # there are 7 Layers of OSI model
* 7:  Application Layer -> Application layer is implemented in software. It provides data to the presentation layer for further processing.
          
* 6: presentation layer -> It Prepares data from the application layer for transmission.And Handles **formatting, encryption, and compression** so other systems can understand it.
          
* 5: Session Layer ->  Session layer protocols help in setting up and managing connections. They enable sending and receiving of data, and handle the termination of the connection.
          
* 4: tranportation layer ->The transport layer is responsible for ensuring that data is delivered correctly and in order from one device to another. It handles error checking, flow control, and proper sequencing of data.
          
* 3:  network layer -> function of network layer is logical addressing, wehenver you are working with router that is network layer
          
* 2:  Data Link Layer -> It allows you to directly communicate with computers and host (It will recieves the data packets from the network layer and this data packet will contain the ip addresses of both source and destination (or sender or the reciver) ..Physcal addressing is also done by data  link layer
          
* 1: physical layer -> Deals with the **actual hardware and transmission** of raw bits over the network medium.  It transmits the bits from electrical singnals

---
## Transport Layer
### port Number,  Sequence number, Segmentation, flow control , Error Control, Load BAlancing
---
1. Port Number:
A numeric identifier used to distinguish different applications or services on a device.
Example: HTTP uses port 80, HTTPS uses port 443.

2. Sequence Number:
A number assigned to each segment of data to keep track of the order in which data should be reassembled at the receiver.

3. Segmentation:
The process of breaking large data into smaller pieces (segments) so it can be sent efficiently over a network.

4. Flow Control:
A method to regulate the rate of data transmission between sender and receiver, preventing the receiver from being overwhelmed.

5. Error Control:
Techniques used to detect and correct errors in transmitted data to ensure reliable communication.

Example: retransmitting lost or corrupted data.

6. Load Balancing:
A process of distributing network traffic or workload across multiple servers or paths to ensure no single device is overloaded and performance is optimized.
---
   <img width="1024" height="1536" alt="ChatGPT Image Oct 3, 2025, 11_37_07 AM" src="https://github.com/user-attachments/assets/0d01ca65-cfc6-4b36-8a76-f9fd53ec9eb0" />
---

### MAC Address (Every component of your system have diffrent MAC Address) ###
- So every device gets a different MAC address to ensure correct and unique communication on the network.
---
# TCP IP MODEL 
<img width="420" height="501" alt="image" src="https://github.com/user-attachments/assets/ee095afe-4280-4f2d-a25a-5c0e1fc36dda" />
<img width="579" height="373" alt="image" src="https://github.com/user-attachments/assets/4cbb1db2-e04d-4368-8ea5-f0fdfcaac81f" />

* (this is basically known as internet protocol shoot
* Number of layers are reduced in this model
  <img width="619" height="177" alt="image" src="https://github.com/user-attachments/assets/8482cae2-b33a-4b0b-8742-461c433a81e5" />

* So the TCP/IP  model used more for practical implimentations
* where as the OSI Model is used more conceptually or we can say implimented theoritically
  🌐 TCP/IP vs. OSI Model
Model	Use	Description
TCP/IP Model	Practical / Implementation	This model is the functional architecture that the internet (and most networks) actually use today. It is less rigid and combines some OSI layers.
OSI Model	Conceptual / Theoretical	This model is a seven-layer framework used for teaching, describing, and standardizing networking functions. It offers a detailed, vendor-neutral structure.
---
💻 Detailed Layers: Application Layer
#  Application Layer
 1) What are the responsibilities of this layer?
The Application Layer is responsible for providing network services to the end-user's application. This includes:

Identifying communication partners: Determining if the requested communication partner is available.
Determining resource availability: Checking if sufficient network resources exist for the request.
Synchronizing communication: Setting up and managing the agreement between the application and the network service.
Data formatting/presentation: While the Presentation Layer (in the OSI model) traditionally handles data formatting, the Application Layer in the TCP/IP model often incorporates these duties, preparing data to be sent across the network.

2) Why are we using this layer? / What do we do with this layer?
We use this layer because it is the entry point for users to access network services. It allows the applications we use daily (browsers, email clients, WhatsApp) to send and receive data over the network.

3) Why does this layer exist?
This layer exists to interact directly with the user's software application and translate the user's request into a format that the lower network layers can understand and process. It acts as the bridge between the human user and the networking stack.

## Notes on Application Layer: Clarification
-User Interaction: Applications like WhatsApp and Web Browsers (Chrome, Firefox) operate at this layer. In the TCP/IP model, this layer sits on top of the Transport Layer.

- Protocols:  The functionality of this layer relies entirely on Application Layer Protocols (like HTTP, DNS, SMTP, FTP) to define how data is exchanged, what kind of data is transferred, and how the applications communicate.
--- 
# 🤝 Client-Server Architecture
 - how  application talk to each other
 - <img width="607" height="143" alt="image" src="https://github.com/user-attachments/assets/3d98fd86-10d6-4bf3-b681-8b1fef66a846" />

-  What is a server?
- A server is a powerful computer or program that provides a service, resource, or data to other computers (the clients) over a network. It is always listening and ready to respond to a client's request.

- Clarifications using the YouTube Example:
Client (You): When you search for a video, your device (laptop, phone) is the client. Your web browser sends an HTTP request (an Application Layer protocol) to the YouTube server.

- Server: The YouTube server receives this request, processes it, and sends back the requested video data.

- Scalability: Correct. Large companies like YouTube use multiple servers to handle the massive volume of client requests. This is called load balancing.

- Data Centers: Correct. A Data Center is a secure facility housing a vast collection of interconnected, high-performance computing resources, including servers, storage systems, and networking gear. They are essentially the physical home for the internet's infrastructure.

- IP Addresses: Correct. Servers that host public services often have static (fixed) IP addresses so clients can reliably locate and connect to them every time.

---
##  ping time : 
- ping measures the round trip time for messages sent from the originating host to the destination of the computer and that are echoed back
- <img width="855" height="584" alt="image" src="https://github.com/user-attachments/assets/a80abc8d-36b6-46cb-a9a4-0820d8bf7cf8" />
 --- 
  # Another Architecture is Peer to Peer Architecture
 *  Protocols:
 * Web Protocols

-- Deep diving in to protocol of Application layer
 TCP/IP Protocols
   * HTTP Protocols
   * Dynamic host control Protocol
   * FTP
   * SMTP
   * POP3 & IMAC
   * SSH
   * vNC
   * Telnet: terminal emulation
   * UDP:connection less session(state less connection) data may be lost in this
     ---
- Process : process is an running intance of a programme
- Thread : A thread is an lighter version of a process
* Multi threading
* Sockets: when you need to send messages from one system to like another system this can be done through sockets(It is a software process) interface between a process and internet
  ---
  # ports
  - Ip address tell us with which devices we are working with and ports tells us  about which application we are working with
  - # Ephermeral Ports # :
 ---
- HttP: It is a client server protocol and it tells us how you request this data from the server and it also tells us how the server will send back data to the client
- HTTP : uses Transmission control protocol inside it
- because  TCP makes sure that all data is recieved and everything
- so when a client makes a request to the server that known as an HTTP request and  when the server sends back a response to the client that is known as HTTP response
 - Note
* Every Application layer protocol also requires some transport layer protocols
# HTTP Methods:
 - The method is basically that is telling the server what to do
 - Get Method :you are requesting for some data
 - Post method : you are a client and you are giving some data to the server like a web form when you ragister somewhere like user name password ao whatever
 - Put Method: puts data at a particular loacation
 - Delete Method:
 - status codes: tell about that how much requested are successfull or not(informational category)
 - cookies : it is a unique string(stored in my browser)
 - Third party cookies:
 - How Email works ?
 - for sendinng email SMTP ,PoP3
 - which transport layer will email use TCP or UDP
 - it will use TCP beacause we want the entire data available to us
 - DNS (Domain name System): it keeps the record that every domain name will be assosciated with an ip address (It is similar to a phone book where in the phone book we have the number of each custome and the phone number is always associated with a particular user) 
---
## TCP and Udp Or TCP vs UDP

---
# **DNS (Domain Name System)**  
*(It is a directory or database service)*  

- Domain names are mapped to IP addresses.  
- **Why is DNS part of the Application Layer?**  
  Remembering IP addresses is often very difficult, so we use domain names because they are simpler and easier to remember.  
- **NOTE:** ICANN registers all top-level domains.  
- **Root DNS Servers:**  
  They manage top-level domains such as `.io`, `.org`, `.com`, etc. These servers are the first point of contact in the DNS hierarchy.  

![DNS Diagram](https://github.com/user-attachments/assets/90cd3019-bfc4-4e96-876b-9879bce20c25)

**NOTE:** You cannot buy a domain name — you can only rent it.  

---
## **Key Reasons**

- **Leasing, not buying:** You rent a domain for a set period, typically between 1 to 10 years.  
- **Preventing hoarding:** This model prevents entities from buying up valuable domain names indefinitely, keeping the market fair.  
- **Promoting turnover:** If a domain isn’t renewed, it eventually becomes available again, preventing unused names from being lost forever.  
- **Funding internet infrastructure:** Registration fees help fund the maintenance of the Domain Name System (DNS).  

---
# **Transport Layer**
- **What is the difference between the Transport Layer and the Network Layer?**  
- The **Network Layer** handles data transfer between different networks.  
- The **Transport Layer** operates within end devices (hosts).  
- **Role of the Transport Layer:**  
  It takes information from the network and delivers it to the application layer.  
- If data needs to be transferred from one network to another, it is done by the **Network Layer**.  
- If data is transferred from one computer to another (end-to-end), it is done by the **Transport Layer**.  

![Transport Layer Diagram](https://github.com/user-attachments/assets/9b00ba55-316b-41ac-8ae3-2e453bffce40)

- The Transport Layer also handles **congestion control**.  
- Congestion control algorithms are **built into TCP**.  
---
## **Multiplexing and Demultiplexing**

*(These processes help the transport layer handle multiple communication streams efficiently.)*
---
## **Checksum**
**What is a checksum?** 

A checksum is an integer value used to verify data integrity during transmission. It ensures that the data received matches the data sent.

---
## **Timers**

*(Section under development — to be expanded later.)*
- Re transmission timer
- <img width="823" height="401" alt="image" src="https://github.com/user-attachments/assets/37e37c3a-cb29-4643-b48b-a80ea2c073c4" />

---
- Deep Diving into Protocols of Transport Layer
- TCP/IP
- UDP : user datagram protocols :
- Here the issues are that Data may not be Delivered
- Data may change
- Data may not be in order
- Basically it is aconnectionless protocol
- UDP uses check sum (**UDP while check is the data is corrupted or not but it will not do anything of it**)
- source Port Number 2bites
- Destination Port 2 bites 
- Length of datagram  2 bites
- check sum 2 bytes
- header is of 8 bytes
- Data will be added ( total size of data is  2^26 - header)
---
* Use cases of UDP
* it is very fast
* video conferencing application
* DNS also uses UDP
* Gaming
* sudo tcpdump -c 5
---
--**TCP protocol**

## **HTTP and TCP Protocol Relationship**

- **HTTP uses the TCP protocol.**  
- **TCP** stands for **Transmission Control Protocol**.  
- It is part of the **Transport Layer** in the TCP/IP model.  
- The **Application Layer** sends a large amount of raw data, and **TCP segments** this data — meaning it divides the data into smaller, manageable chunks called **segments**.  
- TCP may also **collect (reassemble)** the data received from the **Network Layer** to deliver it properly to the Application Layer.
  ---
### **Congestion Control**

- **Congestion Control:** It manages situations when data packets are delayed or fail to arrive.  
- It also ensures that all data segments are received **in the correct order**, maintaining reliable communication between sender and receiver.
---
### **Features of TCP**

- **Connection-oriented:** TCP first establishes a connection between the sender and receiver before data transmission begins.  
- **Error control:** TCP provides mechanisms to detect and recover from transmission errors.  
- **Congestion control:** It manages network traffic to prevent data loss and maintain stable performance.  
- **Full duplex communication:** Both devices can **send and receive data simultaneously**, enabling efficient two-way communication.  

---
### ** Three way hand shake **
- What is the TCP 3-Way Handshake?
- The TCP 3-Way Handshake is a fundamental process used in the Transmission Control Protocol (TCP) to establish a reliable connection between a client and a server before data transmission begins. This handshake ensures that both parties are synchronized and ready for communication.
  <img width="551" height="214" alt="image" src="https://github.com/user-attachments/assets/1de955b0-316a-4438-9f08-fd24d75ea038" />
### **TCP 3-Way Handshake**

1. **SYN:** The client sends a SYN (Synchronize Sequence Number) packet to the server to initiate a connection.  
2. **SYN + ACK:** The server replies with a SYN-ACK, acknowledging the client’s request and indicating its own readiness to communicate.  
3. **ACK:** The client sends an ACK back to the server, completing the handshake and establishing a reliable connection for data transfer.  

---
## **Network Layer**

- In the **Network Layer**, we work primarily with **routers**.  
  <img width="361" height="221" alt="image" src="https://github.com/user-attachments/assets/c2591d23-5bc9-4bdc-9c09-efa111c0c085" />  
- Every router operates with its own **network layer logic**.  
- Communication at this layer happens **hop-by-hop**, meaning data is passed from one router to another until it reaches its destination.  
- Every device has a unique **MAC address** (used at the Data Link Layer).  
- When we talk about a **network interface**, it also has its own **logical address (IP address)** used at the Network Layer.
- 
### **Static Routing and Dynamic Routing**

#### **Static Routing**
- In **static routing**, routes are **manually configured** by the network administrator.  
- The routing path **does not change automatically**, even if the network topology changes.  
- Best suited for **small networks** where routes rarely change.  
- **Advantages:** Simple to configure, predictable routing behavior.  
- **Disadvantages:** Not scalable, requires manual updates when changes occur.  

#### **Dynamic Routing**
- In **dynamic routing**, routers **automatically learn and update** routes using routing protocols.  
- The routing tables are **updated in real-time** based on network changes or failures.  
- Common **dynamic routing protocols** include **RIP, OSPF, EIGRP, and BGP**.  
- **Advantages:** Scalable, adapts automatically to changes.  
- **Disadvantages:** More complex and requires additional resources (CPU, bandwidth).  

---
## Internet Protocol(IP)
- IP v 4-> 32 bit numbers  , with 4 words
- IP v 6-> 128 - bits
- Subnetting : 
---

- 
     
  
