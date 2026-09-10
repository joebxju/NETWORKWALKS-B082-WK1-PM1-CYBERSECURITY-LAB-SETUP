<h1 align="center">Cybersecurity Lab Environment Setup</h1>

<p align="center">
</p>
<p align="center">

  <img src="https://img.shields.io/badge/Cybersecurity-0F172A?style=for-the-badge&labelColor=2563EB&logo=kalilinux&logoColor=white" alt="Cybersecurity" />

  <img src="https://img.shields.io/badge/Kali%20Linux-v2026.2-111827?style=for-the-badge&labelColor=0EA5E9&logo=kalilinux&logoColor=white" alt="Kali Linux" />

  <img src="https://img.shields.io/badge/VirtualBox-v7.2.14-111827?style=for-the-badge&labelColor=2563EB&logo=virtualbox&logoColor=white" alt="VirtualBox" />

  <img src="https://img.shields.io/badge/Linux-111827?style=for-the-badge&labelColor=475569&logo=linux&logoColor=white" alt="Linux" />

  <img src="https://img.shields.io/badge/Networking-111827?style=for-the-badge&labelColor=0891B2" alt="Networking" />

  <img src="https://img.shields.io/badge/Penetration%20Testing-111827?style=for-the-badge&labelColor=7C3AED&logo=kalilinux&logoColor=white" alt="Penetration Testing" />

  <img src="https://img.shields.io/badge/Ethical%20Hacking-111827?style=for-the-badge&labelColor=4F46E5&logo=kalilinux&logoColor=white" alt="Ethical Hacking" />

  <img src="https://img.shields.io/badge/Network-10.0.0.0%2F24-111827?style=for-the-badge&labelColor=0891B2" alt="Network" />

  <img src="https://img.shields.io/badge/Virtualization-111827?style=for-the-badge&labelColor=2563EB&logo=virtualbox&logoColor=white" alt="Virtualization" />

  <img src="https://img.shields.io/badge/Networkwalks-111827?style=for-the-badge&labelColor=2563EB" alt="Networkwalks" />

  <img src="https://img.shields.io/badge/Mentor-Waqas%20Karim%20(CCIE)-111827?style=for-the-badge&labelColor=475569" alt="Waqas Karim CCIE" />

  <img src="https://img.shields.io/badge/Developer-Syed%20Bilal%20Ahmed-111827?style=for-the-badge&labelColor=0F766E&logo=github&logoColor=white" alt="Joel Biju" />
</p>
<p align="center">
  <strong
     
  <strong>networkwalks-B082-week1-Cybersecurity-lab-setup</strong>
</p>

<p align="center">
  VirtualBox • Kali Linux • Virtual Networking • Linux Networking
</p>

---
# Lab Purpose

The purpose of this lab is to build a **controlled and isolated cybersecurity environment** using Oracle VirtualBox and Kali Linux.

A dedicated virtual lab provides a safer environment for practicing cybersecurity concepts without directly experimenting on production systems or unauthorized networks.

The lab will be used as a foundation for practical learning in:

- Networking
- Linux
- Cisco
- Ethical Hacking
- VAPT
- Security Labs
- Python
- Security Automation

---

# Lab Environment

| Component | Details |
|---|---|
| Host Operating System | Windows 11 |
| Processor | Intel Core i3 |
| RAM | 8 GB – 16 GB |
| Storage | 512 GB – 1 TB |
| Virtualization Platform | Oracle VirtualBox 7.2.14 |
| VirtualBox Package | Platform Packages |
| Guest Operating System | Kali Linux 2026.2 |
| Network Type | NAT Network |
| Network CIDR | 10.0.0.0/24 |
| Kali Linux IP | 10.0.0.2/24 |
| Gateway | 10.0.0.1 |
| DNS | 8.8.8.8 |

---


# Tools & Resources

- **7-Zip:** [https://7-zip.org/download.html](https://7-zip.org/download.html)
- **VirtualBox:** [https://virtualbox.org/wiki/Downloads](https://virtualbox.org/wiki/Downloads)
- **Kali Linux:** [https://kali.org/get-kali](https://kali.org/get-kali)

---

# Steps 1/6 

- 7-Zip
- Oracle VirtualBox
- Kali Linux
- NAT Network
- Linux Networking
- IPv4
- VirtualBox Snapshots

---

# Lab Setup

The Networkwalks Phase 1 workflow consists of six setup steps:

1. Install 7-Zip
2. Install Oracle VirtualBox
3. Configure the VirtualBox NAT Network
4. Download and import Kali Linux
5. Configure Kali Linux IP settings
6. Create a VM snapshot

---
---

# Phase 01 — Lab Setup

## 1. 7-Zip Installation

## What I Did

Installed **7-Zip** to extract and manage the virtual machine files required for the cybersecurity lab.

## Why

The Kali Linux VM files need to be extracted and prepared before importing them into the virtualization environment.

---

## 2. Oracle VirtualBox Installation

## What I Did

Installed and configured **Oracle VirtualBox** as the virtualization platform for the cybersecurity laboratory.

## Why

VirtualBox provides the virtualized environment required to run Kali Linux as a separate virtual machine.

## Result

<img width="960" height="540" alt="Screenshot 2026-09-08 173030" src="https://github.com/user-attachments/assets/b16dd0cc-f0b8-4b44-8077-a9efeb5e83c0" />

---

## 3. NAT Network Configuration

## What I Did

Created a dedicated **NAT Network** in Oracle VirtualBox for the cybersecurity lab.

## Why

The NAT Network provides a controlled virtual networking environment for the laboratory machines.
```text
Network Type : NAT Network
Network CIDR : 10.0.0.0/24
DHCP         : Enabled
```

<img width="960" height="540" alt="Screenshot 2026-09-08 174050" src="https://github.com/user-attachments/assets/de127a20-605e-419e-8a3b-f3e3fef12a15" />


---

## 4. Kali Linux VM Setup

## What I Did

Downloaded and imported the **Kali Linux virtual machine** into Oracle VirtualBox and connected the VM to the configured `NatNetwork`.

## Why

Kali Linux is used as the primary cybersecurity operating environment for practical security learning, laboratory exercises, and authorized security testing.
## VM Configuration 
Operating System : Kali Linux
Version          : 2026.2
Virtualization   : Oracle VirtualBox
Network          : NatNetwork


<img width="1280" height="800" alt="Screenshot_2026-09-09_06_23_16" src="https://github.com/user-attachments/assets/882030f1-5c2e-48e3-92dd-9e5ed175b7ef" />


## 5. Kali Linux Network Configuration

### What I Did

Configured the **Kali Linux network interface** with the required IP address, subnet, gateway, and DNS settings.

### Why

Proper IP configuration is required for Kali Linux to communicate with the configured **NAT Network** and access network resources.

```text
IP Address : 10.0.0.2/24
Gateway    : 10.0.0.1
DNS        : 8.8.8.8
```
<img width="1280" height="800" alt="Screenshot_2026-09-09_06_27_30" src="https://github.com/user-attachments/assets/a273b36f-a256-4f1a-9c01-5d61f5e8a816" />
<img width="960" height="540" alt="Screenshot 2026-09-09 155631" src="https://github.com/user-attachments/assets/dfbf0e28-b25b-4f85-94ea-258473b12c46" />


### Commands Used

```bash
ifconfig
sudo ifconfig eth0 down
sudo ifconfig eth0 up
ping google.com
```
<img width="1920" height="891" alt="Screenshot_2026-08-10_09_29_30" src="https://github.com/user-attachments/assets/cb24fd6c-4303-4aec-b38e-bfdaf4837dff" />

<img width="1920" height="891" alt="Screenshot_2026-08-10_05_32_37" src="https://github.com/user-attachments/assets/d1959ac8-3666-462b-90ee-08c6ae6db979" />

---

## 6.VirtualBox Snapshot

### What I Did

Created a **VirtualBox snapshot** after completing the initial Kali Linux lab configuration.

### Why

The snapshot provides a **safe restore point** before continuing with future cybersecurity labs and experiments.


# 🏗️ Lab Architecture

```text
Host Machine
     │
     ▼
Oracle VirtualBox
     │
     ▼
NAT Network
10.0.0.0/24
     │
     ▼
Kali Linux VM
10.0.0.2/24
     │
     ▼
Cybersecurity Labs
```

---

# Key Learning

During this phase, I gained practical experience with:

- Virtual machine deployment
- VirtualBox configuration
- Kali Linux setup
- IPv4 and subnet configuration
- NAT networking
- Linux network configuration
- Routing and connectivity verification
- VM snapshot and recovery

---

# Security & Ethics

This laboratory is intended for **educational and authorized cybersecurity practice only**.

Security testing should only be performed on systems, networks, applications, or devices that you own or have explicit permission to test.

---

# Mentor

**Waqas Karim (CCIE)**

Thank you for the technical guidance and practical learning opportunity throughout the internship.

---
# Phase 01 Progress

**6 / 6 Steps Completed**

**Networkwalks Cybersecurity Internship — Week 01**
