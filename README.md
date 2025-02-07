# Network Design Case Study

## Objective
This project focuses on designing a scalable and redundant network for a medium-sized business using hierarchical network design principles.

## Scenario
A company, **SmartTech Solutions**, requires a robust network infrastructure to connect three buildings: **Administration, Sales, and IT**. The network must support 50 employees per building, ensure secure communication, and provide room for future expansion.

## Network Design

### 1. **Architecture Overview**
- **Core Layer**: A high-performance core switch serves as the backbone.
- **Distribution Layer**: Two distribution switches connect to the core for redundancy.
- **Access Layer**: Each building has two access switches for connecting employees' devices.

### 2. **IP Addressing Scheme**
| Department     | Network Address     | VLAN ID |
|----------------|---------------------|---------|
| Administration | 192.168.10.0/24     | 10      |
| Sales          | 192.168.20.0/24     | 20      |
| IT             | 192.168.30.0/24     | 30      |

### 3. **Routing & Redundancy**
- **Inter-VLAN Routing** is enabled for department communication.
- **HSRP/VRRP** ensures backup router availability.
- **EtherChannel** is used to bundle redundant links.

### 4. **Security Features**
- **Access Control Lists (ACLs)** restrict inter-department access.
- **Port Security** limits unauthorized device connections.
- **MAC Address Filtering** is enforced on access switches.

## Tools & Technologies Used
- **Cisco Packet Tracer** or equivalent network simulation software
- **EtherChannel, VLANs, Inter-VLAN Routing**
- **HSRP/VRRP for redundancy**
- **ACLs and Port Security for security enforcement**

## Setup Instructions
1. Open **Cisco Packet Tracer**.
2. Load the provided **network design file**.
3. Verify **VLAN, IP addressing, and routing configurations**.
4. Run **ping and traceroute** commands to test connectivity.
5. Simulate **failover scenarios** to confirm redundancy.

---

## Author
This project was created by the repository owner.
