# Enterprise-Network-Design-Implementation
Network Design and  Implementation , this is a Cisco Packet Tracer project that simulates a real-world enterprise network using VLANs, inter-VLAN routing, OSPF, DHCP, NAT, ACLs, and security features. It demonstrates scalable network architecture, efficient communication, and hands-on enterprise networking skills.
====================================================================================================================================================================

🌐 Enterprise Network Design (CCNA Project)


📌 Overview
This project demonstrates a multi-site enterprise network built using Cisco Packet Tracer. It includes VLAN segmentation, dynamic routing, NAT for internet access, and security using ACLs.

____________________________________________________________________________________________________________________________________________________________________

🏗️ Network Architecture

Head Office (HQ) with 3 departments:

HR (VLAN 10)
IT (VLAN 20)
Sales (VLAN 30)
Branch 1 and Branch 2 networks

ISP simulation for internet connectivity

____________________________________________________________________________________________________________________________________________________________________

⚙️ Technologies Used

OSPF (Open Shortest Path First) – Dynamic routing
VLAN & Inter-VLAN Routing
NAT (PAT) – Internet access
ACL (Access Control List) – Security
HSRP – Gateway redundancy

____________________________________________________________________________________________________________________________________________________________________

🌐 IP Addressing Scheme

| Network        | Subnet             |
|----------------|--------------------|
| VLAN 10 (HR)   | 192.168.10.0/24    |
| VLAN 20 (IT)   | 192.168.20.0/24    |
| VLAN 30 (Sales)| 192.168.30.0/24    |
| Branch 1       | 192.168.40.0/24    |
| Branch 2       | 192.168.50.0/24    |

____________________________________________________________________________________________________________________________________________________________________

🔐 Security Implementation

Configured ACL to block HR network from accessing IT network
Allowed all other traffic for normal operations

____________________________________________________________________________________________________________________________________________________________________

🌍 Features

Full connectivity between HQ and branches
Internet access using NAT (PAT)
Dynamic routing using OSPF
Network segmentation using VLANs

____________________________________________________________________________________________________________________________________________________________________

🧪 Testing & Verification

✅ Connectivity Test

Successfully pinged across VLANs and branch networks
Verified internet access using NAT

🔁 OSPF Verification
Routes learned dynamically across all routers

🌐 NAT Verification
Private IPs translated to public IP using PAT

🔒 ACL Verification
HR network blocked from accessing IT network

____________________________________________________________________________________________________________________________________________________________________

📸 Screenshots

🗺️ Topology
<img width="1917" height="996" alt="Screenshot 2026-07-23 154849" src="https://github.com/user-attachments/assets/18844ab7-9b17-4d27-afa6-3fe5b3a81f69" />
