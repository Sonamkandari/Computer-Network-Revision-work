# Computer-Network-Revision-Work

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
# QUES: if two persons are using a chatting application to communicate with each other will there ip adress will be different ?. And also will there port number will be different..?
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
* UDP -> User datagram protocol
* HTTP -> Hyper text transfer protocol -> this defines the format of data transmission between your web clients


---
# How data is Transffered?
# Data will be tranffered into packets
---
## What are Packets

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
# 📡 Network Topologies

## 🚌 Bus
- All devices share a **single cable**.  
- ✅ Cheap, easy to set up  
- ❌ If cable fails → whole network down, slow with many devices  

## 🔄 Ring
- Devices connected in a **circle**.  
- ✅ Equal access, less collision  
- ❌ One failure can break network, harder to troubleshoot  

## ⭐ Star
- All devices connect to a **central hub/switch**.  
- ✅ Easy to manage/expand, one failure doesn’t affect others  
- ❌ Central device failure = network down, more cabling  

## 🌳 Tree
- **Combination of Bus + Star**.  
- ✅ Easy to expand, hierarchical structure  
- ❌ Backbone failure affects all, higher cost  

## 🔗 Mesh
- **Every device connects to every other**.  
- ✅ Highly reliable, fault tolerant  
- ❌ Very costly, hard to scale  
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
  ##  Application Layer
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
  
