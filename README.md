# 🧠 CCNA Practice Skills Assessment – ITN Network Configuration

This repository contains my **recreated version** of the official **Cisco Networking Academy – CCNA: Introduction to Networks (ITN) Practice Skills Assessment (PTSA)** where I scored the maximum number of points for the task. All configurations, subnetting, and documentation were fully rebuilt by me based on the original PTSA scenario using **Cisco Packet Tracer**.

---

## 🗂️ Project Overview

The goal of this project was to design, configure, and document a complete IPv4/IPv6 departmental network,  
demonstrating practical routing, switching, and network management skills.

Tasks included:
- Subnetting of the 192.168.1.0/24 network  
- IPv4 and IPv6 addressing  
- Router and switch configuration  
- Secure remote management using SSH and Telnet  
- Device hardening and password policies  
- Network connectivity verification

---

## ⚙️ Devices Used

| Device | Interfaces | Description |
|:--|:--|:--|
| **CS Department Router** | G0/0, G0/1 | Provides inter-LAN routing and secure management via SSH |
| **LAB 214-A Switch** | VLAN 1 (SVI) | Allows remote management via Telnet |
| **LAB 124-C PCs** | PC124-1, PC124-5 | Hosts in LAB 124-C LAN |
| **LAB 214-A PC and Server** | PC214-1, Server | Hosts in LAB 214-A LAN |

---

## 🧩 Addressing Summary

| Network | Subnet | Mask | Hosts | Purpose |
|:--|:--|:--|:--|:--|
| LAB 124-C LAN | 192.168.1.96/27 | 255.255.255.224 | 30 | PCs in 124-C |
| LAB 214-A LAN | 192.168.1.144/28 | 255.255.255.240 | 14 | PCs and Server in 214-A |

IPv6 networks:
- `2001:db8:acad:a::/64`  
- `2001:db8:acad:b::/64`

---

## 🚀 Configurations

### **Router: CS-Department**
Full configuration file: [`router_configuration.md`](./router_configuration.md)

### **Switch: LAB-214A-SW**
Full configuration file: [`switch_configuration.md`](./switch_configuration.md)

---

## 🧠 Skills Demonstrated
- IPv4 & IPv6 subnetting and addressing  
- Router & switch configuration  
- SSH and Telnet remote management  
- Device hardening and password encryption  
- IPv6 routing and interface setup  
- Network verification and troubleshooting  

---

## 🧾 Files Included

| File | Description |
|:--|:--|
| `CCNA_PTSA_ITN_Configuration.pkt` | Cisco Packet Tracer report |
| `CCNA_PTSA_ITN_Configuration.pdf` | Full configuration report |
| `router_configuration.md` | Router setup and commands |
| `switch_configuration.md` | Switch setup and commands |
| `addressing_table.png` | IPv4 and IPv6 addressing summary |
| `logical_topology.png` | Logical network topology diagram exported from Packet Tracer |

---

💬 _“Recreated the official CCNA ITN PTSA configuration entirely from scratch to demonstrate practical networking skills.”_

