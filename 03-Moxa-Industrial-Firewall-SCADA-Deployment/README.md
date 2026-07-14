# Moxa Industrial Firewall Deployment for SCADA Network

## Overview

This project demonstrates the deployment of a **Moxa Industrial Firewall** to secure communication between the **DMZ network** and an **Industrial SCADA network**. A **Sophos Firewall** protects the enterprise network and connects to the Moxa Industrial Firewall through the **DMZ zone**. The Moxa firewall isolates the Operational Technology (OT) environment and provides secure access to industrial devices connected through an **Moxa O-Ring Industrial Ethernet Switch**.

This architecture follows industrial cybersecurity best practices by separating the IT and OT networks while allowing only authorized communication between them.

---

## Network Topology

```text
                          ISP
                           │
                    ┌──────────────┐
                    │ Sophos FW    │
                    └──────────────┘
                           │
                         DMZ Zone
                           │
                ┌────────────────────┐
                │ Moxa Industrial FW │
                └────────────────────┘
                           │
                        Switch
                           │
          ┌──────────┬──────────┬──────────┐
          │          │          │          │
        SCADA      PLCs       RTUs       HMIs
        Server                           Workstations
```

---

## Project Objectives

* Deploy a Moxa Industrial Firewall to protect the SCADA network.
* Connect the Sophos Firewall DMZ zone to the Moxa Firewall.
* Secure communication between IT and OT environments.
* Connect industrial devices through the Moxa O-Ring Switch.
* Restrict network access using firewall policies.
* Enable secure communication for SCADA systems.

---

## Technologies Used

* Moxa Industrial Firewall
* Sophos Firewall
* Moxa O-Ring Industrial Switch
* SCADA Network
* Industrial Ethernet
* DMZ Architecture
* Static Routing
* Firewall Policies
* VLAN Segmentation
* Network Address Translation (NAT)
* Industrial Cybersecurity

---

## Configuration Highlights

### Sophos Firewall

* Configured DMZ interface.
* Created routes to the SCADA network through the Moxa Firewall.
* Implemented firewall policies allowing only required industrial protocols.
* Restricted direct access from the enterprise LAN to the OT network.

### Moxa Industrial Firewall

* Configured LAN and WAN interfaces.
* Implemented firewall policies for industrial communication.
* Allowed only authorized traffic between the DMZ and SCADA network.
* Configured static routes for industrial subnets.
* Enabled logging and event monitoring.

### Industrial Switch

* Connected downstream from the Moxa Firewall.
* Provided high-availability ring topology for industrial devices.
* Connected SCADA servers, PLCs, RTUs, HMIs, and engineering workstations.
* Enabled rapid network recovery in the event of a link failure.

---

## Security Features

* IT/OT Network Segmentation
* DMZ Isolation
* Stateful Firewall Inspection
* Static Routing
* Access Control Policies
* Event Logging
* Industrial Network Protection
* High Availability Ring Topology

---

## Verification

The deployment was validated by performing the following tests:

* Connectivity between the Sophos Firewall DMZ and the Moxa Firewall.
* Secure communication between the enterprise network and SCADA network.
* SCADA server communication with PLCs and RTUs.
* Firewall policy verification.
* Static route validation.
* Switch redundancy and failover testing.
* Network event and security log verification.

---

## Skills Demonstrated

* Moxa Industrial Firewall Deployment
* Sophos Firewall Integration
* SCADA Network Security
* Industrial Network Segmentation
* DMZ Architecture
* Switch Network Design
* Static Routing
* Firewall Policy Configuration
* OT Network Security
* Industrial Cybersecurity
* Network Troubleshooting

---

## Author

**Nagaganapathi**
**Network & Security Engineer**
GitHub: https://github.com/NagaNetOps
