# Atlas Vitae University Hospital

## Enterprise Network Infrastructure

Atlas Vitae University Hospital is a fictional healthcare organization used as the environment for the design, implementation and validation of an enterprise network infrastructure in Cisco Packet Tracer.

The project focuses on building a secure, scalable and highly available hospital network capable of supporting clinical, administrative and network-management operations.

## Project Overview

The infrastructure follows a hierarchical enterprise architecture based on Core, Distribution and Access layers.

The implementation includes:

* Layer 3 Core switching
* Distribution and Access switching
* OSPF dynamic routing
* HSRP gateway redundancy
* EtherChannel using LACP
* VLAN-based network segmentation
* Inter-VLAN routing through SVIs
* Dual enterprise edge routers
* Wired and wireless connectivity
* Enterprise network services
* VoIP and Cisco Call Manager Express
* QoS
* ACL-based security
* NAT and PAT
* SSH remote management
* Centralized monitoring and logging

## Network Segmentation

The hospital network is divided into dedicated VLANs according to operational and infrastructure requirements.

| VLAN | Name        | Purpose                                |
| ---: | ----------- | -------------------------------------- |
|   10 | ADMIN       | Administrative Staff                   |
|   20 | DOCTORS     | Medical Staff                          |
|   30 | NURSES      | Nursing Department                     |
|   40 | DIAGNOSTICS | Medical Imaging & Diagnostic Equipment |
|   50 | SERVERS     | Enterprise Data Center                 |
|   60 | NOC         | Network Operations Center              |
|   70 | GUEST       | Visitor Wireless Network               |
|   80 | VOICE       | IP Telephony                           |
|   90 | MANAGEMENT  | Infrastructure Management              |
|   99 | NATIVE      | Native VLAN and unused switch ports    |

## Enterprise Network Services

The infrastructure integrates several services required for hospital operations and network administration:

* DHCP
* DNS
* FTP
* E-mail
* NTP
* Syslog
* Internal and public web services
* Network monitoring
* Cisco Call Manager Express
* VoIP

## Internet Connectivity

Internet connectivity is implemented through a simulated ISP environment.

The project uses:

* Public IPv4 addressing
* Static NAT for published services
* Dynamic NAT
* PAT / NAT overload for internal users
* Controlled external access through the enterprise edge

A public hospital website is exposed through Static NAT, while internal users receive controlled Internet access through NAT/PAT.

## Security

Security is implemented through multiple complementary mechanisms:

* VLAN segmentation
* Extended and standard ACL policies
* Dedicated Management VLAN
* Restricted NOC access
* Secure SSH administration
* Controlled exposure of public services
* Dedicated Native VLAN
* Administrative shutdown of unused interfaces

These mechanisms provide separation between user, infrastructure, voice, guest and server traffic.

## High Availability

The network incorporates redundancy mechanisms to reduce the impact of equipment and link failures.

The main mechanisms are:

* HSRP
* Dual Layer 3 Core Switches
* Dual Enterprise Edge Routers
* EtherChannel using LACP
* Spanning Tree Protocol with defined primary and secondary root roles

## Network Validation

The implementation was validated through functional testing of the main network components and services, including:

* OSPF adjacencies
* HSRP operation
* EtherChannel
* DHCP
* Internet connectivity
* Public and internal web services
* ACL policies
* SSH access
* QoS
* Network monitoring
* IP telephony
* FTP
* Syslog
* NTP synchronization
* E-mail

## Project Documentation

The complete technical implementation report is available here:

[Atlas Vitae Enterprise Network – Implementation Report](Documentation/Atlas_Vitae_Enterprise_Network_Implementation_Report.pdf)

## Packet Tracer Simulation

The complete Cisco Packet Tracer simulation is available here:

[Atlas Vitae Enterprise Network – Packet Tracer](PacketTracer/Atlas_Vitae_Enterprise_Network.pkt)

## Project Gallery

Topology diagrams and implementation screenshots are available in:

* [Topology](Topology/)
* [Images](Images/)

## Repository Structure

```text
Atlas-Vitae-Enterprise-Network/
│
├── Documentation/
│   └── Atlas_Vitae_Enterprise_Network_Implementation_Report.pdf
│
├── PacketTracer/
│   └── Atlas_Vitae_Enterprise_Network.pkt
│
├── Topology/
│   └── [topology images]
│
├── Images/
│   └── [implementation screenshots]
│
├── README.md
├── LICENSE
└── .gitignore
```

## Author

**Panzo Capitão Lunfuankenda**

Junior Network Infrastructure Engineer

Interests: Enterprise Networking, Network Security, Telecommunications, Intelligent Networks and Cybersecurity.

## Disclaimer

Atlas Vitae University Hospital is a fictional organization created for network design and simulation purposes. The infrastructure was implemented and validated in Cisco Packet Tracer and does not represent a production hospital network.
