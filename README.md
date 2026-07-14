1. Project Overview

This project involved the deployment and configuration of an enterprise campus network infrastructure for Zamil Steel Industries Co., Ltd. using Cisco Catalyst 9300 Series switches and a FortiGate 201G Next-Generation Firewall.

The solution was designed to provide a secure, scalable, and high-performance network supporting user connectivity, server communication, and Internet access while following Cisco enterprise design best practices.

The network consists of a dedicated Layer 3 Core Switch connected to multiple access switches through redundant EtherChannel links. A FortiGate 201G firewall serves as the network perimeter, enforcing security policies and providing controlled Internet connectivity.

2. Network Architecture
## Network Topology

                               Internet
                                   │
                                  ISP
                                   │
                      +------------------------+
                      |     FortiGate 201G     |
                      +-----------┬------------+
                                  │
                          Transit Gateway
                                  │
              +--------------------------------------+
              | Cisco Catalyst C9300X-24Y-A          |
              |            Core Switch               |
              +---------┬------------┬---------------+
                        │            │
                   Po11 │       Po12 │       Po13
                        │            │
        +---------------+--------+---+----------------+
        │                        │                    │
+------------------+   +------------------+   +------------------+
|  Access Stack 1  |   |  Access Switch 2 |   |  Access Switch 3 |
| 3 × C9300L-48P   |   | C9300L-48P-4X-E  |   | C9300L-48P-4X-E  |
+------------------+   +------------------+   +------------------+
        │                     │                     │
        └───────────────┬─────┴─────────────────────┘
                        │
   Users • Servers • IP Phones • Printers • Wireless APs
3. Device Inventory
Device Role	Model	Quantity	Description
Firewall	FortiGate 201G	1	Enterprise Next-Generation Firewall
Core Switch	Cisco Catalyst C9300X-24Y-A	1	Layer 3 Core Switch with 25G Uplink Ports
Access Stack	Cisco Catalyst C9300L-48P-4X-E	3	StackWise Access Switch Stack
Access Switch	Cisco Catalyst C9300L-48P-4X-E	1	Standalone Access Switch
Access Switch	Cisco Catalyst C9300L-48P-4X-E	1	Standalone Access Switch

Total Network Devices: 6

4. Solution Features
Core Network
Cisco Catalyst 9300X Layer 3 Core Switch
Centralized Inter-VLAN Routing
High-speed Fiber Uplinks
Transit Gateway Connectivity to Firewall
Enterprise Campus Architecture
Access Layer
Cisco Catalyst 9300L Access Switches
One StackWise Stack consisting of three switches
Two Standalone Access Switches
PoE Connectivity for End Devices
High-speed Uplink Connectivity
VLAN Implementation

The network was logically segmented using Virtual LANs (VLANs) to separate different business functions. Layer 3 routing was configured on the core switch to enable secure communication between VLANs while maintaining proper network isolation.

Switching Technologies

The following Cisco enterprise switching technologies were implemented:

VLAN Configuration
Access Ports
Trunk Ports
Layer 3 Switching
Inter-VLAN Routing
Switch Virtual Interfaces (SVIs)
EtherChannel (LACP)
Switch Stacking (StackWise)
Network Security

Multiple Layer 2 security mechanisms were implemented to protect the access network from unauthorized devices and switching attacks.

Configured security features include:

Port Security
Sticky MAC Address Learning
PortFast
BPDU Guard
BPDU Filter
Storm Control
Secure Management Access
Firewall Configuration

The FortiGate 201G firewall was deployed as the Internet edge security appliance and integrated with the Cisco campus network.

Configuration included:

Initial Firewall Deployment
Interface Configuration
Transit Gateway Integration
Static Routing
Security Policies
Network Address Translation (NAT)
Internet Access Control
Security Hardening
5. Technologies Implemented
Cisco Technologies
Cisco Catalyst 9300X Series
Cisco Catalyst 9300L Series
Cisco IOS-XE
VLAN
EtherChannel
Layer 3 Switching
StackWise
STP
PortFast
BPDU Guard
BPDU Filter
Port Security
Fortinet Technologies
FortiGate 201G
FortiOS
Firewall Policies
Static Routing
NAT
Security Policy Configuration
6. Project Highlights
Enterprise Campus Network Design
Secure Layer 2 and Layer 3 Architecture
High Availability Uplink Design
Scalable Network Infrastructure
Centralized Routing
Enterprise Firewall Integration
Best Practice Security Configuration
Modular Network Design
Simplified Network Management
Future Expansion Ready
7. Skills Demonstrated
Enterprise Network Design
Cisco Switching
Cisco IOS-XE Configuration
FortiGate Firewall Administration
VLAN Planning and Implementation
Layer 2 Security
Layer 3 Routing
EtherChannel Configuration
Switch Stacking
Firewall Integration
Network Hardening
Infrastructure Deployment
Network Documentation
Enterprise Network Troubleshooting
8. Conclusion

This project demonstrates the successful deployment of a secure and scalable enterprise campus network using Cisco Catalyst 9300 Series switches and a FortiGate 201G firewall. The implementation incorporates enterprise-grade switching, Layer 3 routing, network segmentation, and security best practices, resulting in a reliable infrastructure capable of supporting current business operations while allowing for future growth.
