# Module 1 Course 3 Notes

## 📘 What You’ll Learn

- Structure of a network (network architecture)
- Network operations and protocols
- Network attacks and security hardening
- Cloud networks
- TCP/IP model
- Standard networking tools

---

## 🌐 Network Basics

A **network** is a group of connected devices that communicate via cables or wireless connections.

### Types of Networks

- **LAN (Local Area Network)**: Small geographic area (e.g., home, school).
- **WAN (Wide Area Network)**: Large area like cities, states, or countries (e.g., the internet).

---

## 🔧 Network Tools

### Hub
- Broadcasts info to all devices.
- Less secure.

### Switch
- Forwards data to specific devices.
- Maintains a MAC address table.
- Part of the data link layer.

### Router
- Connects multiple networks.
- Uses IP addresses for communication.
- Can include firewall features.

### Modem
- Connects network to the internet via ISP.
- Converts digital signals to analog and vice versa.

### Virtualization Tools
- Perform functions of network hardware in software form.
- Offered by cloud providers.

---

## 🔌 Network Devices & Diagrams

### Common Devices
- Computers, smartphones, printers, servers
- Identified by **MAC** and **IP** addresses

### Firewalls
- Monitor and filter incoming/outgoing traffic.
- First line of defense.

### Servers
- Provide services to clients (DNS, file storage, email).

---

## ☁️ Cloud Networks

### Cloud Computing
- Use of remote servers via internet.
- Reduces cost and increases scalability.

### CSP Services
- **SaaS**: Software (e.g., Google Docs)
- **IaaS**: Infrastructure (e.g., VMs, storage)
- **PaaS**: Platform for app development

### Hybrid & Multi-Cloud
- **Hybrid**: Combines local and cloud infrastructure
- **Multi-cloud**: Uses multiple CSPs

### SDNs (Software-defined networks)
- Virtual network devices (routers, firewalls, switches)

---

## 📡 Network Communication

### Data Packet Components
- **Header**: Source/Destination IP & MAC, protocol number
- **Body**: Message content
- **Footer**: Signals end of packet

### Ports
- Organize traffic by service type (e.g., Port 443 for HTTPS)

---

## 📊 Network Performance

- **Bandwidth**: Max data rate (bps)
- **Speed**: Rate of data received
- **Packet Sniffing**: Monitoring traffic for analysis

---

## 🧱 TCP/IP Model

1. **Network Access Layer**
   - Hardware, cables, ARP
2. **Internet Layer**
   - IP addresses, routing
3. **Transport Layer**
   - TCP/UDP protocols, flow control
4. **Application Layer**
   - User-facing services (HTTP, DNS, FTP)

---

## 🧬 OSI Model Overview (7 Layers)

1. **Physical** – Hardware (cables, modems)
2. **Data Link** – Switches, MAC addressing
3. **Network** – IP routing (Routers)
4. **Transport** – TCP/UDP, data delivery
5. **Session** – Managing sessions
6. **Presentation** – Data formatting/encryption
7. **Application** – End-user services (Web, Email)

---

## 🌍 IP Addressing

- **IPv4**: 4 sets of numbers (e.g., 192.168.1.1)
- **IPv6**: 8 groups of hex digits (e.g., 2001:0db8::1)

### Public vs Private IP
- **Public**: Assigned by ISP, visible on internet
- **Private**: Internal network use only

---

## 🛠 Components of Network Layer Communication

- IPv4 Header: Contains version, source/destination IPs, TTL, protocol, and more
- IPv6: Simplified headers, better routing, avoids address collisions

---

## 📚 Glossary

- **Bandwidth**: Max data transmission capacity
- **Cloud Computing**: Remote network services
- **Hub**: Broadcasts to all devices
- **Router**: Connects different networks
- **Switch**: Directs packets intelligently
- **Modem**: Connects router to ISP
- **MAC Address**: Device identifier
- **IP Address**: Device’s network location
- **Packet Sniffing**: Capturing network data
- **TCP/IP**: Communication framework
- **Port**: Logical channel for traffic
- **UDP**: Lightweight, fast, connectionless
- **TCP**: Reliable, connection-oriented
- **LAN/WAN**: Network size classifications

---
