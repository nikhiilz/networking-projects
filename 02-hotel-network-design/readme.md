# Hotel Network Design – Enterprise Campus Network

![Network Diagram](screenshots/hotel-network-design.png)
<p align="center"><strong>Network Representation</strong></p>

## Project Overview
This project simulates a **multi-floor hotel enterprise network** designed using Cisco Packet Tracer  
The goal was to understand and implement industry-standard networking technologies

## Technologies Implemented

- VLANs & 802.1Q Trunking
- Inter-VLAN Routing (Router-on-a-Stick)
- OSPF Dynamic Routing (Area 0)
- DHCP (Router-based)
- Wireless Access Points (WPA2-PSK)
- Secure Remote Management (SSH)
- Port Security (Sticky MAC, Shutdown Mode)

---

## Verification & Testing (Summary)

**Detailed verification was performed on core enterprise technologies**, including:

<details>
<summary><strong>OSPF Dynamic Routing </strong>(click to expand)</summary>

**Test Performed:**
- Verified OSPF adjacency routers
- Confirmed OSPF-learned routes in routing table

**Test Result:** Routers successfully formed adjacencies in Area 0 and learned routes

![OSPF Adjacency Test](screenshots/ospf-adjacency-test.png)
![OSPF Route Test](screenshots/ospf-route-test.png)


</details>

<details>
<summary><strong>Inter-VLAN routing </strong>(click to expand)</summary>


**Test Performed:** An inter-vlan communication test was performed from PC-REC-F1 to PC-ADMIN-F3

**Test Result:** Successful ICMP packets were received

![PC-REC-F1 > PC-ADMIN-F1](screenshots/inter-vlan-routing-test.png)

</details>

<details>
<summary><strong>DHCP address assignment </strong>(click to expand)</summary>

**Test Performed:** DHCP Bindings on each router
**Test Result:** IP Addresses very assigned

![Router Floor 1](screenshots/dhcp-binding-RF1.png)
![Router Floor 2](screenshots/dhcp-binding-RF2.png)
![Router Floor 3](screenshots/dhcp-binding-RF3.png)

</details>
<details>
<summary><strong>Secure remote management (SSH) </strong> (click to expand)</summary>

**Test Performed:** SSHing from TEST-PC to R-FLOOR-3

**Test Result:** Succefully accessed!

![SSH TEST-PC > R-FLOOR-3](screenshots/ssh-testpc-rwf3.png)
</details>



## Project Files

- Packet Tracer File: [`/packet-tracer/hotel-network-design.pkt`](packet-tracer/hotel-network-design.pkt)

- Network Documentation & Testing: [`/documentation`](documentation/)

- Device Configurations: [`/configs`](configs/)