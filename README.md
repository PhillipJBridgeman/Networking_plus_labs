# Network+ Lab Portfolio

A practical networking lab portfolio built while preparing for the **CompTIA Network+ N10-009** certification.

This repository documents my progress through networking fundamentals, Cisco Packet Tracer exercises, troubleshooting scenarios, and small network designs. The goal is not simply to store lab files, but to demonstrate how I plan, configure, test, document, and improve networks.

> **Current focus:** Cisco Packet Tracer labs, IPv4 addressing, subnetting, switching, routing, wireless networking, network services, security, and troubleshooting.

---

## Project Goals

This repository is designed to help me:

* Apply Network+ concepts in realistic lab environments
* Build repeatable troubleshooting habits
* Practice documenting technical work clearly
* Create evidence of hands-on networking knowledge
* Prepare for infrastructure, IT support, application support, NOC, and cloud roles
* Connect networking theory to my Windows Server, Linux, Azure, and production support experience

---

## Repository Structure

```text
network-plus-labs/
├── README.md
├── 01-network-fundamentals/
├── 02-ip-addressing-and-subnetting/
├── 03-switching-and-vlans/
├── 04-routing/
├── 05-network-services/
├── 06-wireless/
├── 07-network-security/
├── 08-monitoring-and-troubleshooting/
├── 09-capstone-labs/
├── diagrams/
├── notes/
└── templates/
```

Each completed lab should normally contain:

```text
lab-name/
├── README.md
├── lab-name.pkt
├── topology.png
└── evidence/
```

---

## Lab Documentation Standard

Each lab is documented using the same structure:

1. **Objective** — What the lab is intended to demonstrate
2. **Scenario** — The business or technical situation
3. **Topology** — Devices, connections, and addressing
4. **Implementation** — Configuration steps and commands
5. **Validation** — Tests used to confirm the design works
6. **Troubleshooting** — Problems found and how they were resolved
7. **Lessons Learned** — What the lab reinforced
8. **Files** — Packet Tracer file, screenshots, and supporting notes

This format makes each lab understandable without opening Packet Tracer first.

---

## Featured Labs

| Lab                               | Skills Demonstrated                                              | Status  |
| --------------------------------- | ---------------------------------------------------------------- | ------- |
| Basic LAN Connectivity            | End devices, switches, cabling, IPv4 configuration, ping testing | Planned |
| IPv4 Addressing and Subnetting    | CIDR notation, network IDs, host ranges, broadcast addresses     | Planned |
| VLAN Segmentation                 | VLAN creation, access ports, segmentation, connectivity testing  | Planned |
| Inter-VLAN Routing                | Router-on-a-stick or Layer 3 switching concepts                  | Planned |
| DHCP Services                     | Address pools, gateways, DNS settings, client validation         | Planned |
| Static and Dynamic Routing        | Route configuration, path verification, troubleshooting          | Planned |
| Wireless Network Design           | SSIDs, security settings, coverage and client connectivity       | Planned |
| Network Troubleshooting Challenge | Layered diagnosis using commands and evidence                    | Planned |
| Small Business Network            | Integrated switching, routing, DHCP, security, and documentation | Planned |

Statuses will be updated as labs are completed.

---

## Tools and Technologies

* Cisco Packet Tracer
* Git and GitHub
* Visual Studio Code
* Windows 11
* Ubuntu Linux
* PowerShell
* Bash
* Wireshark
* Windows Server lab environment
* Draw.io or similar diagramming tools

---

## Skills Being Developed

### Networking

* IPv4 and IPv6 addressing
* Subnetting and CIDR
* Ethernet standards and cabling
* Switching and VLANs
* Routing fundamentals
* DHCP, DNS, NAT, and NTP
* Wireless networking
* Network security controls
* Monitoring and troubleshooting
* Network documentation

### Technical Practice

* Translating requirements into a network design
* Testing connectivity systematically
* Recording configuration decisions
* Separating symptoms from root causes
* Writing clear technical documentation
* Using Git to track lab progress

---

## Validation Approach

A lab is not considered complete until its expected behaviour is verified.

Typical validation methods include:

```text
ping
tracert / traceroute
ipconfig / ifconfig / ip
arp
nslookup
show ip interface brief
show running-config
show vlan brief
show interfaces
show ip route
```

Validation screenshots and command output may be stored in the lab's `evidence` folder.

---

## Progress Roadmap

### Phase 1 — Foundations

* Network devices and functions
* Ethernet and cabling
* OSI and TCP/IP models
* IPv4 and IPv6 addressing
* Subnetting

### Phase 2 — Network Implementation

* Switching
* VLANs
* Trunking
* Routing
* DHCP and DNS
* Wireless networking

### Phase 3 — Operations and Security

* Monitoring
* Baselines
* Access controls
* Segmentation
* Secure protocols
* Troubleshooting methodology

### Phase 4 — Capstone Work

* Small office network
* Multi-VLAN business network
* Network failure and recovery scenario
* Documented troubleshooting challenge

---

## Example Lab Entry

```markdown
# VLAN Segmentation Lab

## Objective

Create separate VLANs for Administration and Support while preserving
connectivity within each department.

## Scenario

A small organization wants to reduce unnecessary broadcast traffic and
separate departmental devices.

## Addressing

| VLAN | Department | Network |
|---|---|---|
| 10 | Administration | 192.168.10.0/24 |
| 20 | Support | 192.168.20.0/24 |

## Validation

- Devices in VLAN 10 can communicate with other VLAN 10 devices.
- Devices in VLAN 20 can communicate with other VLAN 20 devices.
- Cross-VLAN communication fails until routing is configured.

## Lessons Learned

VLANs create separate Layer 2 broadcast domains. Communication between
VLANs requires a Layer 3 routing function.
```

---

## Commit Style

Commits should describe meaningful progress rather than generic file changes.

Examples:

```text
Add initial switched LAN Packet Tracer lab
Document IPv4 subnetting validation steps
Add VLAN 10 and VLAN 20 configuration
Fix incorrect default gateway in DHCP lab
Complete inter-VLAN routing troubleshooting notes
```

---

## About This Repository

I am an IT professional based in Winnipeg with experience in customer service, technical support, databases, application development, Windows, Linux, and production system administration. This repository supports my continued development in networking and cloud infrastructure.

My longer-term goal is to combine networking, systems, databases, application support, and Azure skills in a technical role where I can help plan, support, troubleshoot, and improve business technology.

---

## Notes

* These labs are created for learning and portfolio purposes.
* Packet Tracer simulations may simplify behaviour found in production networks.
* Configurations will be revised as my knowledge and troubleshooting methods improve.
* No employer, customer, production credential, or confidential network information is stored in this repository.

---

## Contact

**Phillip Bridgeman**

* Portfolio: [phillipbridgeman.ca](https://www.phillipbridgeman.ca/)
* LinkedIn: Add your LinkedIn profile URL here
* GitHub: Add your GitHub profile URL here
