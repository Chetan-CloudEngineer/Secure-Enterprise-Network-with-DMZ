# Secure Enterprise Network with DMZ
### Cisco Packet Tracer Project

## 1. Project Overview

Designed and implemented a secure enterprise network using Cisco Packet Tracer.

The project demonstrates enterprise network architecture with multiple departments, a centralized server farm, a Demilitarized Zone (DMZ), and a branch office.

The main objective is to provide secure communication between departments while protecting internal resources and allowing controlled access to public-facing services.

## 2. Network Architecture

The network includes:

- ISP connectivity
- Enterprise edge router
- Core Layer 3 switches
- Department-wise access switches
- Internal server farm
- DMZ network
- Branch office connectivity
- External network access

## 3. Technologies Implemented

- VLANs and VTP
- Inter-VLAN Routing
- 802.1Q Trunking
- EtherChannel (LACP)
- OSPF Dynamic Routing
- DHCP
- NAT, PAT and Static NAT
- Extended Access Control Lists (ACLs)
- Port Security
- Rapid PVST+
- DMZ Architecture
- Web and DNS Servers
- Branch Office Networking

## 4. VLAN and IP Addressing

| VLAN | Department | Network |
|---|---|---|
| 10 | HR | 192.168.10.0/24 |
| 20 | Finance | 192.168.20.0/24 |
| 30 | IT | 192.168.30.0/24 |
| 40 | Management | 192.168.40.0/24 |
| 50 | Server Farm | 192.168.50.0/24 |

**DMZ Network:** 172.16.100.0/24

- Web Server: 172.16.100.10
- DNS Server: 172.16.100.11
- DMZ Gateway: 172.16.100.1

## 5. Network Security Implementation

- Department-wise network segmentation using VLANs.
- HR-to-Finance communication restricted using an extended ACL.
- Public-facing Web and DNS servers placed in the DMZ.
- Static NAT configured for public access to DMZ services.
- PAT configured for internal network Internet access.
- Access restrictions configured to protect internal networks.
- Port Security implemented on access switch ports.
- Rapid PVST+ used to prevent Layer 2 switching loops.

## 6. Routing and Connectivity

- Inter-VLAN routing configured on the Layer 3 core switch.
- OSPF configured between the core switch and edge router.
- Default route configured towards the ISP.
- NAT/PAT configured on the edge router.
- Separate branch office network connected through the ISP.

## 7. Testing and Verification

The following tests are planned/performed to validate the network:

- Verify VLAN creation and VTP synchronization.
- Verify trunk links and EtherChannel operation.
- Verify STP root bridge selection.
- Verify DHCP address allocation.
- Test communication between different VLANs.
- Verify OSPF neighbor relationships and routing tables.
- Test internal Internet connectivity using PAT.
- Test external access to DMZ Web and DNS services.
- Verify ACL restrictions between networks.
- Test port security and network failure scenarios.

## 8. Tools and Devices

**Tool:** Cisco Packet Tracer

**Network Devices:**
- Cisco Catalyst 3560 Multilayer Switches
- Cisco Catalyst 2960 Layer 2 Switches
- Cisco Routers
- Web Server
- DNS Server
- End-user PCs

## 9. Project File

The Cisco Packet Tracer project file (`.pkt`) is available in this repository.

## 10. Learning Outcomes

This project helped develop practical knowledge of enterprise LAN/WAN architecture, Layer 2 and Layer 3 switching, dynamic routing, network security, DMZ implementation, NAT/PAT, and network troubleshooting.
