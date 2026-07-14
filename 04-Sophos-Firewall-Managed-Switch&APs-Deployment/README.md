# Sophos Firewall Deployment with Managed and Unmanaged Switches

## Overview

This project demonstrates the deployment of a **Sophos Firewall** in an enterprise network. The firewall is connected to a **Sophos Managed Switch**, which serves as the central distribution switch. The managed switch is further connected to **three Sophos Unmanaged Switches** that provide network connectivity to end-user devices and **Sophos Access Points** for secure wired and wireless access.

The Sophos Firewall provides internet security, routing, Network Address Translation (NAT), firewall policy enforcement, DHCP services, and secure access for enterprise users.

---

## Network Topology

```text
                      Internet
                          │
                 ┌────────────────┐
                 │ Sophos Firewall│
                 └────────────────┘
                          │
              Sophos Managed Switch
                 ┌────────┼─────────-┬
                 │        │          │        
             Unmanaged  Unmanaged  Unmanaged 
             Switch 1   Switch 2   Switch 3
                │           │         │
            Sophos AP   Sophos AP   Sophos AP
```

## Project Objectives

* Deploy a Sophos Firewall as the enterprise security gateway.
* Connect the firewall to a Sophos Managed Switch.
* Extend network connectivity through three Sophos Unmanaged Switches.
* Deploy Sophos Access Points for wireless connectivity.
* Configure secure internet access, NAT, firewall policies, and DHCP services.

## Technologies Used

* Sophos Firewall
* Sophos Managed Switch
* Sophos Unmanaged Switches
* Sophos Access Points
* VLANs
* DHCP
* Static Routing
* Network Address Translation (NAT)
* Firewall Policies
* Wireless Networking

## Configuration Highlights

### Sophos Firewall

* Configured WAN and LAN interfaces.
* Configured internet access and NAT.
* Created firewall policies.
* Configured DHCP services.
* Enabled secure administrative access.

### Sophos Managed Switch

* Connected directly to the Sophos Firewall.
* Configured VLANs and trunk/access ports (where required).
* Distributed network connectivity to downstream switches and access points.

### Sophos Unmanaged Switches

* Extended LAN connectivity.
* Connected desktop computers, IP phones, printers, and other network devices.
* Required no additional configuration.

### Sophos Access Points

* Connected through the managed and unmanaged switches.
* Configured secure wireless SSIDs.
* Provided wireless access for enterprise users and mobile devices.

## Verification

The deployment was verified by performing the following tests:

* Internet connectivity for wired and wireless users.
* DHCP address assignment.
* Firewall policy validation.
* NAT translation verification.
* Wireless client connectivity.
* Connectivity between managed and unmanaged switches.
* Administrative access verification.

## Skills Demonstrated

* Sophos Firewall Deployment
* Sophos Managed Switching
* Sophos Access Point Deployment
* LAN Switching
* VLAN Configuration
* DHCP Configuration
* Firewall Policy Configuration
* Network Address Translation (NAT)
* Enterprise Network Security
* Wireless Network Deployment
* Network Troubleshooting

---

## Author

**Nagaganapathi**
**Network & Security Engineer**
GitHub: https://github.com/NagaNetOps
