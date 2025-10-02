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
* IP address decides which device to send the data but how we will decide that which application has to be sent data
---
* TCP -> Transmission control protocol it will ensure that data will reached to its destination without any interuption  or not get corrupted in middle of the data transmission process
* UDP -> User datagram protocol
* HTTP -> Hyper text transfer protocol -> this defines the format of data transmission between your web clients

---
# How data is Transffered?
# Data will be tranffered into packets
---
## What are Packets


