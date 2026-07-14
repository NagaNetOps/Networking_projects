# FortiGate 50G Firewall Deployment

## Overview

This project demonstrates the deployment of a **FortiGate 50G Next-Generation Firewall** in an enterprise headquarters with **dual ISP connectivity** and **multiple Site-to-Site IPsec VPN tunnels** connecting remote branch offices. The branch offices use **SonicWall firewalls**, providing secure encrypted communication between the headquarters and multiple locations.

The FortiGate firewall is connected to a **Cisco Meraki Switch**, which provides connectivity to the enterprise LAN, including user devices, servers, IP phones, printers, and wireless access points. The firewall also provides internet access, routing, Network Address Translation (NAT), and security policy enforcement.

---

## Network Topology

```text
                               Internet
                           ┌─────────────┐
                           │             │
                       ISP 1         ISP 2
                           │             │
                           └──────┬──────┘
                                  │
                      ┌─────────────────────┐
                      │   FortiGate 50G     │
                      │   Headquarters FW   │
                      └─────────────────────┘
                        │      │       │
                    IPsec    IPsec   IPsec
                     VPN      VPN     VPN
                      │        │       │
                ┌────────┐ ┌────────┐ ┌────────┐
                │SonicWall│ │SonicWall│ │SonicWall│
                │ Branch 1│ │ Branch 2│ │ Branch 3│
                └────────┘ └────────┘ └────────┘
                                  │
                        Cisco Meraki Switch
                                  │
       PCs • Servers • IP Phones • Printers • Wireless Access Points
```

## Project Objectives

* Deploy a FortiGate 50G firewall at the headquarters.
* Configure dual ISP connectivity for internet redundancy.
* Establish multiple Site-to-Site IPsec VPN tunnels with SonicWall firewalls at branch offices.
* Connect the FortiGate firewall to the Cisco Meraki switching infrastructure.
* Configure static routing, NAT, and firewall policies.
* Provide secure communication between headquarters and branch locations.

## Technologies Used

* FortiGate 50G
* FortiOS
* SonicWall Firewall
* Cisco Meraki Switch
* Site-to-Site IPsec VPN
* Dual ISP
* Static Routing
* Network Address Translation (NAT)
* Firewall Policies
* IPv4 Routing

## Configuration Highlights

### FortiGate Firewall

* Configured dual ISP internet connectivity.
* Created multiple Site-to-Site IPsec VPN tunnels with SonicWall branch firewalls.
* Configured static routes for remote branch networks.
* Implemented firewall security policies.
* Configured Source NAT (SNAT) for outbound internet access.
* Enabled secure administrative access.

### Site-to-Site IPsec VPN

* Configured multiple IPsec VPN tunnels between headquarters and branch offices.
* Configured Phase 1 and Phase 2 parameters.
* Implemented secure encryption and authentication.
* Added routing for remote branch subnets.
* Applied firewall policies to allow encrypted traffic between sites.

### Cisco Meraki Switch

* Connected directly to the FortiGate firewall.
* Provided LAN connectivity for enterprise users.
* Extended network access to PCs, servers, IP phones, printers, and wireless access points.

## Verification

The deployment was verified by performing the following tests:

* Internet connectivity through both ISP links.
* Successful IPsec tunnel establishment with all SonicWall branch firewalls.
* Secure communication between headquarters and branch networks.
* NAT translation verification.
* Firewall policy validation.
* Administrative access verification.
* End-user internet connectivity through the Meraki network.

## Skills Demonstrated

* FortiGate 50G Deployment
* Dual ISP Configuration
* Site-to-Site IPsec VPN
* FortiGate to SonicWall VPN Integration
* Multi-Branch Network Connectivity
* Cisco Meraki Switching
* Static Routing
* Firewall Policy Configuration
* Source NAT (SNAT)
* Enterprise Network Security
* Network Troubleshooting

---

## Author

**Nagaganapathi**
**Network & Security Engineer**
GitHub: https://github.com/NagaNetOps
