# Module 3 Course 3 Notes

## 📘 What You’ll Learn
- Network Security
- Network Intrusion Tactics
- Network Attack Protection

---

## 🚨 Common Network Intrusion Attacks
- **Malware**
- **Spoofing**
- **Packet Sniffing**
- **Packet Flooding**

---

## 🕵️‍♂️ Network Interception Tactics

### Packet Sniffing
- Captures data in transit using tools.
- Can modify or spy on data packets.

### Backdoor Attacks
- Exploits hidden system access left by devs/admins.
- Can be installed after compromise.
- Used to maintain persistent access.

### DoS (Denial of Service) Attacks
- Flood servers/networks to disrupt service.
- **DDoS**: Uses multiple devices to amplify attack.

---

## 🧨 Common DoS Attacks

### 1. SYN Flood
- Abuses TCP handshake by spamming SYN requests.
- Server gets overloaded with half-open connections.

### 2. ICMP Flood
- Sends repeated ICMP echo requests.
- Server wastes bandwidth replying until it crashes.

### 3. Ping of Death
- Sends oversized ICMP packets (>64KB) to crash systems.

---

## 📊 Network Protocol Analyzer: tcpdump

### What is it?
- Command-line packet analyzer.
- Lightweight, uses little memory.
- Pre-installed on many Linux systems.

### Key Features
- Shows **timestamp**, **source/destination IP & ports**.
- Can be used for:
  - Troubleshooting
  - Detecting malicious traffic
  - Creating alerts
  - Identifying unauthorized activity

---

## 🧠 Real-Life Example: DNS DDoS Attack

- A botnet created by students overwhelmed a DNS service provider.
- Tens of millions of DNS requests caused outage for many major websites.
- Botnet = network of malware-infected computers under attacker control.

---

## 🔍 Packet Sniffing (Detailed)

### Data Packet Structure
- **Header**: IP addresses
- **Body**: Sensitive data like names, credit cards

### Types
- **Passive**: Eavesdropping only
- **Active**: Alters data or redirects traffic

### Protection
- Use **VPNs**, **HTTPS**, and **avoid open Wi-Fi**.

---

## 🎭 IP Spoofing

### What Is It?
- Fakes source IP to impersonate legitimate systems.

### Attack Types
- **On-Path Attack**: Intercepts and alters communication.
- **Replay Attack**: Re-sends captured packets to impersonate users.
- **Smurf Attack**: Spoofs IP and floods with ICMP packets.

### Protection
- Encrypt data (e.g., TLS).
- Configure firewalls to reject packets with spoofed IPs.

---

## 🛡️ DoS Defense and Firewall Rules

- Firewalls should deny packets with local IPs from external sources.
- Next-Gen Firewalls (NGFW) detect traffic anomalies like:
  - Packet floods
  - Oversized broadcasts
  - ICMP abuse

---

## 📦 Flashcard Definitions

- **DoS Attack**: Flooding network/server to stop function.
- **DDoS Attack**: Multiple sources flood the target.
- **SYN Flood**: Exploits TCP handshake with SYN packets.
- **Packet Sniffing**: Captures network data in transit.
- **IP Spoofing**: Changes packet source IP to trick systems.
- **On-Path Attack**: Intercepts or alters legitimate connections.
- **Replay Attack**: Re-sends captured packets later.
- **Smurf Attack**: Spoof + flood using ICMP.
- **Ping of Death**: Sends oversized ping packets.

---

## 🧰 Glossary Terms (Select)

| Term | Definition |
|------|------------|
| **Active Packet Sniffing** | Manipulates data packets in transit |
| **Botnet** | Malware-controlled group of devices |
| **ICMP** | Reports errors in network transmission |
| **ICMP Flood** | DoS using repeated ICMP requests |
| **NIC (Promiscuous Mode)** | Accepts all packets, even unintended |
| **Firewall Rules** | Can block spoofed IP packets |
| **NGFW** | Advanced firewall with deep inspection |
| **Replay Attack** | Delays or repeats legitimate data packets |

---

## ✅ Summary

- **Network Security**: Securing against DoS, spoofing, sniffing
- **Intrusion Tactics**: Packet sniffing, backdoors, spoofing
- **Protection Measures**: Encryption, VPNs, firewalls, NGFWs

