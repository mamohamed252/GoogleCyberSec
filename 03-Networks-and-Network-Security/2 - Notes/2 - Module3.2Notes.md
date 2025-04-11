# Module 2 Course 3 Notes

## 📘 What You'll Learn
- Network Protocols
- Virtual Private Networks (VPNs)
- Firewalls, Security Zones, and Proxy Servers

---

## 🌐 Network Protocols

### Transmission Control Protocol (TCP)
- Establishes reliable connections using a 3-way handshake (SYN → SYN/ACK → ACK).
- Ensures data is delivered correctly.

### Address Resolution Protocol (ARP)
- Resolves IP addresses to MAC addresses on a local network.

### HyperText Transfer Protocol Secure (HTTPS)
- Secure version of HTTP using SSL/TLS.
- Uses port 443.

### Domain Name System (DNS)
- Translates domain names (e.g., `google.com`) into IP addresses.
- Uses UDP on port 53 (TCP if data is large).

---

## 🛡️ Security Protocols

### Secure File Transfer Protocol (SFTP)
- Transfers files securely over SSH (port 22).

### Secure Shell (SSH)
- Secure access to remote systems (port 22).

### Internet Control Message Protocol (ICMP)
- Used to report errors or test connectivity (e.g., `ping`).

### Simple Network Management Protocol (SNMP)
- Manages devices on a network.
- Can query bandwidth, reset passwords, etc.

---

## 📦 Network Management Protocols

### Dynamic Host Configuration Protocol (DHCP)
- Assigns IP addresses and gateway/DNS info dynamically.
- Operates on UDP ports 67 (server) and 68 (client).

---

## 🧩 Additional Protocols and Ports

| Protocol | Port | Layer | Description |
|---------|------|--------|-------------|
| HTTP | 80 | Application | Insecure web traffic |
| HTTPS | 443 | Application | Secure web traffic |
| FTP | 21 | Application | File transfer |
| Telnet | 23 | Application | Remote access (not secure) |
| SMTP | 25 / 587 | Application | Email sending (unencrypted/encrypted) |
| POP3 | 110 / 995 | Application | Email retrieval (unencrypted/encrypted) |
| IMAP | 143 / 993 | Application | Email access (unencrypted/encrypted) |

---

## 🔐 VPNs and Encryption

- VPNs mask your IP and encrypt data in transit.
- Use **encapsulation** to wrap encrypted data in a readable packet.
- Create a tunnel between your device and the VPN server.

### VPN Protocols
- **Wireguard**: Simple, fast, modern, open-source.
- **IPSec**: Older, complex but widely supported.

---

## 🧱 Firewalls

### Types
- **Hardware**: Physical devices.
- **Software**: Installed on computers/servers.
- **Cloud-based (FaaS)**: Managed by CSPs.

### Modes
- **Stateful**: Tracks traffic and behavior.
- **Stateless**: Relies on predefined rules.

### Next-Gen Firewalls (NGFW)
- Offer deep packet inspection, intrusion detection, threat intelligence.

---

## 🛰️ Proxy Servers

- Sit between the user and external server.
- **Forward Proxy**: Hides user's IP.
- **Reverse Proxy**: Controls internet access to internal servers.
- **Email Proxy**: Filters spam and phishing attempts.

---

## 🔐 Security Zones

### Zone Types
- **Uncontrolled Zone**: Public networks like the internet.
- **Controlled Zone**: Internal network protected by firewalls.

#### Within Controlled Zones:
- **DMZ (Demilitarized Zone)**: Hosts public-facing servers (web, DNS, etc.).
- **Internal Network**: Contains private, secure resources.
- **Restricted Zone**: Confidential, privileged-access data.

---

## 📶 Wireless Security

### IEEE 802.11 (Wi-Fi Standards)

### Security Protocols:
- **WEP**: Insecure, outdated.
- **WPA**: Improved but still vulnerable.
- **WPA2**: Uses AES, standard today.
- **WPA3**: Strongest encryption, uses SAE to prevent KRACK attacks.

---

## 🧮 Subnetting & CIDR

### Subnetting
- Divides networks into logical groups for better performance/security.

### CIDR Notation
- Format: `192.168.1.0/24`
- Reduces routing table entries, improves IP allocation.

---

## 🧠 Glossary (Select Terms)

- **ARP**: Resolves IP to MAC.
- **DHCP**: Assigns IP addresses.
- **DNS**: Resolves domain to IP.
- **Encapsulation**: Wraps data for secure transport.
- **Firewall**: Monitors and filters traffic.
- **NAT**: Translates private IPs to public IPs.
- **Proxy Server**: Intermediary for requests.
- **SFTP**: Secure file transfer.
- **SSH**: Secure remote access.
- **SNMP**: Network management.
- **TCP**: Reliable transport.
- **UDP**: Fast, connectionless transport.
- **VPN**: Encrypts traffic, masks IP.
- **WPA2/3**: Wi-Fi security protocols.

---

## ✅ Summary

- **Network Protocols**: TCP, ARP, DNS, HTTPS
- **VPNs**: Protect privacy on public networks
- **Firewalls & Proxies**: Key to securing internal networks
- **Security Zones**: Layered defense using DMZ and subnetting
- **Wireless Security**: WPA2/WPA3 recommended
