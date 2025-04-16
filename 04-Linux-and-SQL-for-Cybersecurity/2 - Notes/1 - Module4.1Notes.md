# Course 4 – Module 1
## The Wonderful World of Operating Systems

---

## Introduction to Operating Systems

**Operating System (OS)** – The interface between computer hardware and the user.
- Manages resources for efficient use
- Provides a way to interact with the computer
- Acts as the foundation of all system operations

---

## Hardware vs. Software

**Hardware** – The physical components of a computer
**Binary Language** – The computer communicates in 0s and 1s

---

## Common Operating Systems

- **Windows** – Closed-source
- **macOS** – Partially open-source
- **Linux** – Fully open-source; widely used in cybersecurity
- **ChromeOS** – Derived from Chromium (open-source); used in education
- **Android** – Open-source mobile OS
- **iOS** – Partially open-source mobile OS

---

## OS Vulnerabilities

### Legacy Operating Systems
- Outdated but still used due to software compatibility
- Vulnerable because they’re no longer supported or updated

### Embedded Software
- Software within hardware components
- Harder to upgrade

### Resources for OS Vulnerabilities:
- **Microsoft Security Response Center (MSRC)**
- **Apple Security Updates**
- **CVE for Ubuntu**
- **Google Cloud Security Bulletin**

---

## How an Operating System Works

- **Boot Process:**
  1. Power button activates hardware
  2. BIOS or UEFI chip runs boot instructions
  3. Bootloader starts the OS

- **BIOS (Basic Input/Output System):** Used in older systems
- **UEFI (Unified Extensible Firmware Interface):** Replaces BIOS in modern systems

> Vulnerabilities in BIOS/UEFI can be exploited since antivirus tools often don’t scan them.

---

## Task Execution Flow

1. **User** initiates a task (e.g., opens calculator)
2. **Application** sends request to OS
3. **OS** directs request to appropriate hardware
4. **Hardware** processes and sends output back through OS to application

---

## Example: Using Calculator

- Click app → enter number
- App → OS → CPU → OS → app → Display result

---

## Example: Downloading a File

- User clicks download
- Browser communicates with OS
- OS sends request to hardware
- Hardware downloads
- OS updates browser → Browser notifies user

---

## OS as Resource Manager

- Manages memory, CPU, and other hardware usage
- Ensures tasks receive appropriate resources
- Handles allocation and deallocation

---

## Virtualization Technology

### Virtual Machines (VMs)

- Simulated computers using software-defined resources
- Example: Divide 16GB RAM between host and 3 VMs

### Benefits:
- **Security** – Isolated sandbox environments
- **Efficiency** – Run multiple VMs simultaneously

### Hypervisor:
- Manages VMs
- Allocates hardware to each VM
- Bridges virtual and physical resources

---

## Other Virtualization Types

- Virtual networks
- Virtual servers
> Some do not require an OS

---

## User Interfaces

### Graphical User Interface (GUI)
- Uses icons and visuals (e.g., Windows desktop)
- Components: Start menu, taskbar, desktop

### Command-Line Interface (CLI)
- Text-based; uses typed commands
- Can execute multiple commands at once
- More efficient for cybersecurity tasks
- Keeps **history file** for tracking commands

---

## CLI Advantages in Cybersecurity

- **Speed & Power:** Efficient task execution
- **Traceability:** Use history to audit tasks or trace attacker behavior

---

## Glossary – Module 1 Terms

| Term | Definition |
|------|------------|
| **Application** | Program that performs a specific task |
| **BIOS** | Microchip with startup instructions; used in older systems |
| **Bootloader** | Software that boots the OS |
| **CLI** | Text-based interface using typed commands |
| **GUI** | Visual interface with icons and menus |
| **Hardware** | Physical components of a computer |
| **Legacy OS** | Outdated operating system still in use |
| **Operating System (OS)** | Interface between hardware and user |
| **RAM** | Short-term memory component |
| **UEFI** | Replaces BIOS in modern systems |
| **User Interface** | Program allowing user to control OS functions |
| **Virtual Machine (VM)** | Simulated version of a physical computer |

---
