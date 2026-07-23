Network Design and  Implementation , this is a Cisco Packet Tracer project that simulates a real-world enterprise network using VLANs, inter-VLAN routing, OSPF, DHCP, NAT, ACLs, and security features. It demonstrates scalable network architecture, efficient communication, and hands-on enterprise networking skills.
===================================================================================================================================================================

🌐 Enterprise Network Design (CCNA Project)


📌 Overview

This project demonstrates a multi-site enterprise network built using Cisco Packet Tracer. It includes VLAN segmentation, dynamic routing, NAT for internet access, and security using ACLs.

___________________________________________________________________________________________________________________________________________________________________

🏗️ Network Architecture

Head Office (HQ) with 3 departments :

> HR (VLAN 10)

> IT (VLAN 20)

> Sales (VLAN 30)

> Branch 1 and Branch 2 networks

> ISP simulation for internet connectivity

___________________________________________________________________________________________________________________________________________________________________

⚙️ Technologies Used

> OSPF (Open Shortest Path First) – Dynamic routing

>VLAN & Inter-VLAN Routing

> NAT (PAT) – Internet access

> ACL (Access Control List) – Security

> HSRP – Gateway redundancy

___________________________________________________________________________________________________________________________________________________________________

🌐 IP Addressing Scheme

| Network        | Subnet             |
|----------------|--------------------|
| VLAN 10 (HR)   | 192.168.10.0/24    |
| VLAN 20 (IT)   | 192.168.20.0/24    |
| VLAN 30 (Sales)| 192.168.30.0/24    |
| Branch 1       | 192.168.40.0/24    |
| Branch 2       | 192.168.50.0/24    |

___________________________________________________________________________________________________________________________________________________________________

🔐 Security Implementation

> Configured ACL to block HR network from accessing IT network

> Allowed all other traffic for normal operations

___________________________________________________________________________________________________________________________________________________________________

🌍 Features

> Full connectivity between HQ and branches
> Internet access using NAT (PAT)
> Dynamic routing using OSPF
> Network segmentation using VLANs

___________________________________________________________________________________________________________________________________________________________________

🧪 Testing & Verification

✅ Connectivity Test

> Successfully pinged across VLANs and branch networks
> Verified internet access using NAT

🔁 OSPF Verification
> Routes learned dynamically across all routers

🌐 NAT Verification
> Private IPs translated to public IP using PAT

🔒 ACL Verification
> HR network blocked from accessing IT network

___________________________________________________________________________________________________________________________________________________________________

📸 Screenshots

🗺️ Topology

<img width="1917" height="996" alt="Screenshot 2026-07-23 154849" src="https://github.com/user-attachments/assets/18844ab7-9b17-4d27-afa6-3fe5b3a81f69" />

___________________________________________________________________________________________________________________________________________________________________


🌐 Ping Test

<img width="1668" height="807" alt="Screenshot 2026-07-23 155202" src="https://github.com/user-attachments/assets/5bcdb32f-2115-40e7-8458-3b3f6dcb217f" />
<img width="1668" height="807" alt="Screenshot 2026-07-23 155202" src="https://github.com/user-attachments/assets/84c0cb32-28dc-4547-be5f-f19b9873a32e" />

___________________________________________________________________________________________________________________________________________________________________

🔁 OSPF Routes

<img width="1697" height="797" alt="Screenshot 2026-07-23 155530" src="https://github.com/user-attachments/assets/b111a47b-85dc-4693-9432-ccf2054ed032" />

___________________________________________________________________________________________________________________________________________________________________

🌍 NAT Translation

<img width="1236" height="157" alt="Screenshot 2026-07-23 155729" src="https://github.com/user-attachments/assets/27c695e5-ca61-4bfa-93d3-91dd696dd8df" /> 

___________________________________________________________________________________________________________________________________________________________________

🔒 ACL Test

<img width="891" height="432" alt="Screenshot 2026-07-23 155746" src="https://github.com/user-attachments/assets/f2ef107e-dbdb-4395-99db-d738f88ab5a0" />

___________________________________________________________________________________________________________________________________________________________________

🚀 Outcome

> Successfully designed and implemented a scalable enterprise network with routing, security, and internet connectivity.

___________________________________________________________________________________________________________________________________________________________________

👨‍💻 Author
> Ayush Tiwari

______________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

