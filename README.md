# University Network Design

![Cisco Packet Tracer](https://img.shields.io/badge/Cisco%20Packet%20Tracer-8.x-00bceb?style=for-the-badge&logo=cisco&logoColor=white)
![Network Status](https://img.shields.io/badge/Network%20Status-Simulated%20%26%20Tested-success?style=for-the-badge)
![Project Type](https://img.shields.io/badge/Project-Diploma%20Final%20Year-blueviolet?style=for-the-badge)

## Overview

This project is my Diploma Final Year Project.

The objective of this project is to design and simulate a secure and scalable university network using Cisco Packet Tracer. The network consists of a Main Campus and a Branch Campus, supporting approximately **5,000 users**.

---

## Project Features

- **Routing & Switching**: VLAN Segmentation, Inter-VLAN Routing, Site-to-Site VPN (IPsec/GRE)
- **Security & Access Control**: Access Control Lists (ACL), Cisco ASA Firewall, AAA Authentication, SSH Remote Management
- **Network Services**: DHCP, Network Address Translation (NAT), DNS Server, Syslog Server
- **Application Servers**: FTP Server, Email Server, Web Server
- **Wireless & VoIP**: Wireless LAN Controller (WLC), IP Phone System (Telephony Service)
- **Smart Campus (IoT)**: CCTV Surveillance System, RFID Door Access System

---

## Core VLAN & Subnet Scheme

| VLAN ID | Name | Subnet | Gateway | Purpose |
| :---: | :--- | :--- | :--- | :--- |
| **VLAN 10** | Administration | 192.168.10.0/24 | 192.168.10.1 | Admin staff & management |
| **VLAN 20** | Faculty / Teachers | 192.168.20.0/24 | 192.168.20.1 | Teacher offices |
| **VLAN 30** | Students | 192.168.30.0/24 | 192.168.30.1 | Classrooms & labs |
| **VLAN 40** | Guest Wi-Fi | 192.168.40.0/24 | 192.168.40.1 | Public wireless access |
| **VLAN 99** | Server Farm | 192.168.99.0/24 | 192.168.99.1 | Centralized network servers |

*(Note: Refer to the full project report for the complete IP addressing table.)*

---

## Network Topology

![Network Topology](network-topology.png)

---

## Main Campus

![Main Campus](main-campus.png)

---

## Branch Campus

![Branch Campus](branch-campus.png)

---

## How to Run / Usage

1. Install **Cisco Packet Tracer** (Version 8.0 or above recommended).
2. Download and open the `Final Year Project.pkt` file.
3. Wait a few seconds for all switch ports and routing protocols to converge (green links).
4. **Testing Connectivity**:
   - Open a Student PC desktop -> Command Prompt -> `ping` the Web Server IP or Branch Campus Gateway.
   - Test IoT features by toggling RFID access or viewing the CCTV monitor in the server room.

---

## Project Files

| File | Description |
|------|-------------|
| `Final Year Project.pkt` | Cisco Packet Tracer simulation source file |
| `Final Year Project Report (Word).pdf` | Full project documentation and architecture report |
| `Final Year Project Report (PPT).pdf` | Project presentation slides |

---

## Author

**Lee Han Liang**
