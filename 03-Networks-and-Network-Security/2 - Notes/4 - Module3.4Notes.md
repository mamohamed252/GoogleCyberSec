# Module 4 Course 3 Notes

## 📘 What You’ll Learn

- Security Hardening
- OS Hardening
- Network Hardening Practices
- Cloud Network Hardening

---

## 🔐 What is Security Hardening?

**Security Hardening**: Strengthening a system to reduce vulnerabilities and attack surface.

**Attack Surface**: All potential vulnerabilities that a threat actor could exploit.

### Hardening Targets:

- Hardware
- Operating Systems
- Applications
- Networks
- Databases
- Physical Devices & Environments

---

## 🛠️ Common Hardening Procedures

- Software patches and updates
- Config changes (e.g., encryption standards)
- Disabling unused apps/services/ports
- Reducing access permissions
- Penetration testing (simulated attacks)

---

## 💻 OS Hardening

**OS** = Interface between hardware and software.

### Regular Tasks:

- **Patch Updates**: Fix vulnerabilities ASAP
- **Baseline Configuration**: Compare current state to default secure state
- **Disposal**: Wipe old hardware/software
- **Password Policies**: Strong requirements
- **MFA**: Multi-Factor Authentication

### Attack Prevention:

- **Brute Force Attacks**:

  - **Simple**: Guessing credentials
  - **Dictionary**: Using known/stolen passwords

- **Preventative Tools**:
  - Virtual Machines
  - Sandbox environments
  - Hashing & salting passwords
  - CAPTCHA & reCAPTCHA

---

## 🌐 Network Hardening

### Regular Tasks:

- Firewall rule updates
- Network log analysis
- Patch updates
- Server backups

### One-Time Setup:

- **Port Filtering**: Only needed ports allowed
- **Access Privileges**
- **Encryption**
- **Network Segmentation**:
  - Isolate departments/zones
  - Limit scope of attacks

### Tools:

- **SIEM** (Security Info & Event Management): Aggregates and analyzes logs from all devices

---

## 🧱 Defense in Depth: Network Security Applications

| Tool                                  | Function                                            |
| ------------------------------------- | --------------------------------------------------- |
| **Firewall**                          | Allows/blocks traffic based on rules                |
| **IDS** (Intrusion Detection System)  | Alerts on suspicious activity                       |
| **IPS** (Intrusion Prevention System) | Actively blocks threats                             |
| **SIEM**                              | Collects, visualizes, and prioritizes security logs |

> IDS + Firewall = More defense
> IPS = Proactive stopping of threats
> NGFW = Packet inspection + rule-based filtering

---

## ☁️ Cloud Hardening

**Cloud Network** = Remote data centers for apps/data.

### Best Practices:

- Server **baseline image** comparison
- Separate sensitive apps/functions
- Cloud log analysis via **flow logs** and **packet mirroring**

### IAM (Identity Access Management):

- Manages digital identities and permissions
- Prevent misconfigured roles

### Other Measures:

- **Encryption** and key management
- **Hypervisors** (Type 1 preferred in CSPs)
- **VM Escape Prevention**
- **Cryptographic Erasure** (Crypto Shredding)
- **TPM/CloudHSM** for secure key storage

---

## 🧠 Cloud Security Concepts

- **Zero-Day Attacks**: CSPs often detect/respond faster
- **Shared Responsibility Model**:
  - **CSP** secures infrastructure
  - **Customer** secures applications/data/configs

---

## 🔑 Cryptography in the Cloud

- **Encryption**: Converts data to ciphertext using keys
- **Salting & Hashing**: Secure password storage
- **Key Management**: TPM & CloudHSM
- **Crypto Erasure**: Destroy keys = unreadable data

---

## 📚 Glossary (Select Terms)

| Term                       | Definition                                       |
| -------------------------- | ------------------------------------------------ |
| **Security Hardening**     | Reducing vulnerabilities in systems/networks     |
| **Baseline Configuration** | Secure default settings for comparison           |
| **Patch Update**           | Fixes vulnerabilities in software/OS             |
| **MFA**                    | Requires two+ factors for login                  |
| **Pen Test**               | Simulated cyberattack for finding weak points    |
| **SIEM**                   | Central tool for security event analysis         |
| **Sandbox**                | Isolated test environment for malware/patches    |
| **IAM**                    | Controls cloud identity and access               |
| **Hypervisor**             | Manages virtual machines                         |
| **Crypto Erasure**         | Destroying keys to render encrypted data useless |

---

## ✅ Summary

- **Security Hardening**: Covers OS, network, cloud, hardware.
- **OS Hardening**: Updates, baseline configs, strong passwords.
- **Network Hardening**: Firewalls, port filtering, log analysis.
- **Cloud Hardening**: IAM, encryption, VM security, shared responsibility.
