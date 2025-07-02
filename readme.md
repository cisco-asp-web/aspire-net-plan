# Emerging Network Engineer Strategy Plan - WEB ASP


---


## 📚 Table of Contents
- [Emerging Network Engineer Strategy Plan - WEB ASP](#emerging-network-engineer-strategy-plan---web-asp)
  - [📚 Table of Contents](#-table-of-contents)
  - [🧱 PHASE 1: Core Networking – Deep-Level Foundations](#-phase-1-core-networking--deep-level-foundations)
    - [🔧 Core Technologies](#-core-technologies)
    - [🛠 Tools](#-tools)
  - [🛣 PHASE 2: Core Routing \& Network Services – Deep-Level Operations](#-phase-2-core-routing--network-services--deep-level-operations)
    - [🔧 Core Technologies](#-core-technologies-1)
  - [🏢 PHASE 3: Data Center Networking](#-phase-3-data-center-networking)
    - [🔧 Core Technologies](#-core-technologies-2)
    - [🔧 Storage](#-storage)
  - [⚙️ PHASE 4: Telemetry \& Automation](#️-phase-4-telemetry--automation)
    - [🔧 Core Technologies](#-core-technologies-3)
    - [🛠 Tools](#-tools-1)
    - [Github Repo](#github-repo)
  - [🧾 PHASE 5: Infrastructure Awareness (Beyond Protocols)](#-phase-5-infrastructure-awareness-beyond-protocols)
    - [🔧 Core Topics](#-core-topics)
  - [📚 Recommended Books (WIP):](#-recommended-books-wip)
  - [🧠 Recommended AI Tools :](#-recommended-ai-tools-)
    - [🧠 \*\*ChatGPT (OpenAI) / Circuit (Cisco Internal GPT) / Claude / Gemini \*\*](#-chatgpt-openai--circuit-cisco-internal-gpt--claude--gemini-)
    - [🧠 **Notebook LM**](#-notebook-lm)
  - [💻 2. Developer/Engineer-Focused Assistants - Terminal - SSH and RDP Manager](#-2-developerengineer-focused-assistants---terminal---ssh-and-rdp-manager)
    - [🧑‍💻 **Cursor (VS Code AI IDE)**](#-cursor-vs-code-ai-ide)
    - [✍️ **GitHub Copilot**](#️-github-copilot)
    - [💡 **Warp AI Terminal**](#-warp-ai-terminal)
    - [👻 **Ghostty**](#-ghostty)
    - [💻🔐 **Royal TSX**](#-royal-tsx)
  - [📊 3. Diagramming \& Visualization](#-3-diagramming--visualization)
    - [✏️ **Draw io**](#️-draw-io)
    - [🗂️ **Whimsical AI**](#️-whimsical-ai)
    - [🧾 **Miro AI**](#-miro-ai)
    - [🧩 **Excalidraw + GPT Plugin**](#-excalidraw--gpt-plugin)
    - [🧜‍♀️ **Mermaid**](#️-mermaid)
  - [🧪 4. Lab Networking Tools](#-4-lab-networking-tools)
    - [🧪 Containerlab](#-containerlab)
    - [🧪 Netlab](#-netlab)
  - [🔍 5. Traffic Capture \& Analysis](#-5-traffic-capture--analysis)
    - [🦈 Wireshark](#-wireshark)
    - [🦈 EdgeShark](#-edgeshark)
  - [🎓 6. Certifications](#-6-certifications)
    - [🏢 Enterprise Track](#-enterprise-track)
      - [CCNA (Associate)](#ccna-associate)
      - [CCNP (Professional)](#ccnp-professional)
      - [CCIE (Expert)](#ccie-expert)
    - [🧱 Data Center Track](#-data-center-track)
      - [CCNP Data Center](#ccnp-data-center)
      - [CCIE Data Center](#ccie-data-center)
    - [🌍 Service Provider Track](#-service-provider-track)
      - [CCNP Service Provider](#ccnp-service-provider)
      - [CCIE Service Provider](#ccie-service-provider)
    - [🎥 7 - Cisco Live On-Demand Library](#-7---cisco-live-on-demand-library)

--- 

Author: nicmcl@cisco.com

## 🧱 PHASE 1: Core Networking – Deep-Level Foundations

### 🔧 Core Technologies
- OSI Model, TCP/IP Stack
- Cabling :) 
- L2 vs L3
- IPv4 / IPv6 Addressing and Subnetting (manual & CIDR)
- MAC Addressing, ARP / NDP (Neighbor Discovery Protocol)
- Ethernet Framing, MTU, Jumbo Frames
- VLANs, 802.1Q Trunking, Inter vlan connectivity
- Native VLAN Risks and VLAN Hopping
- Unicast vs Broadcast vs Multicast
- MAC Learning, Flooding, and CAM Table Aging
- Spanning Tree Protocols (STP, RSTP, MST)
- STP Tuning: PortFast, BPDU Guard, Root Guard, Loop Guard
- CDP / LLDP for Topology Discovery
- Trunk vs Access vs Routed Ports
- Storm Control and Loop Protection
- LAG
- TCP Vs UDP
- DHCP, DNS, NAT / PAT Concepts
- IPv6 Basics: SLAAC, Link-Local, Dual Stack
- Basic Routing: Prefix, LPM, Next hop, default GW. AD
- Basic Firewalling (Statefull vs Stateless ?)

### 🛠 Tools
- Containerlab
- Wireshark (filters: `stp`, `arp`, `dhcp`, `icmp`, `lldp`)
- Edgeshark
- CLI Practice: `show`, `debug`, `clear`, `ping`, `traceroute`
- Lab Exercises:
  - Trace MAC learning in a 3-switch lab
  - Simulate and resolve an STP loop
  - Trunk misconfiguration scenario
  - DHCP snooping validation
- 


---

## 🛣 PHASE 2: Core Routing & Network Services – Deep-Level Operations

### 🔧 Core Technologies
- Static Routing and Floating Static Routes
- Static vs Dynamic Routing
  - Distance Vector
  - Link State
- RIP (Just understand it exists :) 
- OSPF:
  - Router ID, Cost, DR/BDR Election
  - Areas: Backbone, Stub, Totally Stubby, NSSA
  - OSPF Neighbor States and LSAs
- ISIS: 
  - another Link State protocol
- BGP:
  - iBGP vs eBGP
  - BGP Peerings (loopback, multihop, TTL-security)
  - BGP Attributes: Weight, Local Preference, AS Path, MED, ORIGIN
  - Filtering: Prefix Lists, Route Maps, AS Path Access Lists
  - Path Manipulation: AS-Path Prepending, Next-Hop-Self
  - iBGP Full Mesh, Route Reflectors
- MPLS 
- Administrative Distance and Route Selection
- VRF / VRF-Lite Fundamentals
- Route Redistribution
  - Feedback Loops and Prevention
- Policy-Based Routing (PBR)
- HSRP / VRRP
- IP SLA and Object Tracking
- Access Control Lists:
  - Standard, Extended, Named
  - Placement (Inbound vs Outbound)
  - Implicit Deny and Logging


---

## 🏢 PHASE 3: Data Center Networking

### 🔧 Core Technologies
- Leaf-Spine Fabric Design (Clos Topology)
- VXLAN:
  - VNI, NVE, Flood & Learn vs Control Plane
  - VXLAN Bridging vs Routing
- EVPN:
  - MP-BGP Signaling, Type 2/3/5 Routes
  - Distributed Anycast Gateway
- vPC:
  - Peer Link, Keepalive, Consistency Parameters
  - Orphan Ports and Dual-Active Scenarios
- LISP
- L2/L3 Gateway Placement (Centralized vs Distributed)
- Routing on the Host (BGP from ToR to Server)
- Loop Prevention Techniques (L2 multipath)

### 🔧 Storage
- FC
- ISCSI
- FCoE



---

## ⚙️ PHASE 4: Telemetry & Automation

### 🔧 Core Technologies
- SNMP v2c / v3, Syslog, NTP
- YANG Models (native & OpenConfig)
- NETCONF, RESTCONF, JSON-RPC
- Streaming Telemetry:
  - Model-Driven vs CLI-Driven
  - gNMI/gRPC Basics
- Configuration Templates:
  - Jinja2 for dynamic rendering
  - YAML inventory structure
- Automation Tools:
  - Python (Netmiko, NAPALM, Requests)
  - Ansible (Cisco NX-OS modules)
  - Terraform
- Event-Driven Automation:
  - Embedded Event Manager (EEM)

### 🛠 Tools
- Docker
- Git & GitHub for version control
- Postman (API exploration)
- Telegraf + InfluxDB + Grafana (streaming telemetry stack)
- Python scripts for show commands and push configs
- Lab Exercises:
  - Use Ansible to build a fabric config from templates
  - Telemetry export from NX-OS to Grafana
  - Python script to check BGP state and log deltas

### Github Repo
- [Awesome Network Automation Repo](https://github.com/networktocode/awesome-network-automation)
---

## 🧾 PHASE 5: Infrastructure Awareness (Beyond Protocols)

### 🔧 Core Topics
- **Optics:**
  - Module types: SR / LR / ER / ZR, BiDi
  - QSFP, SFP+, SFP28, DAC, AOC
  - CWDM / DWDM basics
- **Cabling:**
  - OM3 / OM4 / OS2 Fiber
  - Polarity (Type A/B/C)
  - Patch panels, MPO/MTP connectors
- **Hardware:**
  - Modular vs Fixed Switches
  - Airflow (Front-to-Back, Back-to-Front)
  - PSU Redundancy, Fan Trays
- **ASICs:**
  - Buffering strategies (Shared, Dedicated)
  - Pipeline stages (parser, lookup, egress)
  - Low-latency vs deep-buffer ASIC design

- **Virtualization**
  - Vmware
  - Docker
  - Kubernetes
  - EPBF


## 📚 Recommended Books (WIP): 

TBD

## 🧠 Recommended AI Tools : 

### 🧠 **ChatGPT (OpenAI) / Circuit (Cisco Internal GPT) / Claude / Gemini ** 
- Interactive learning, lab simulation support, career guidance
- Great for network concepts, CLI explanation, script analysis
- Supports code, markdown, and diagram planning

**Best For:** Protocol explanation, mentorship conversations, lab logic

### 🧠 **Notebook LM** 
- Supercharge the learning experience
- Create your own notes, sources 
- Summarize
- Create content based on the sources
- Asks questions

**Best For:** Learning :) 

---

## 💻 2. Developer/Engineer-Focused Assistants - Terminal - SSH and RDP Manager

### 🧑‍💻 **Cursor (VS Code AI IDE)**
- AI code assistant for network automation and scripting
- Great for Ansible, Python, Netmiko, RESTCONF work

**Best For:** Teaching automation and infrastructure-as-code


### ✍️ **GitHub Copilot**
- Inline code generation inside VS Code, IntelliJ, etc.
- Good for fast config snippets, JSON/YAML, and playbooks

**Best For:** Supplementing coding lessons

### 💡 **Warp AI Terminal**
- GPT-powered terminal suggestions and command explanations
- Supports Bash, Zsh, etc.

**Best For:** Linux/NetDevOps education; teaching CLI habits

### 👻 **Ghostty**
- Best all around terminal
- Supports Bash, Zsh, etc.

**Best For:** All around terminal (again)


### 💻🔐 **Royal TSX**
- Best SSH / RDP manager

**Best For:** Connecting to your labs using SSH and RDP


---

## 📊 3. Diagramming & Visualization

### ✏️ **Draw io**
- Networking Diagram :) 


### 🗂️ **Whimsical AI**
- Helps generate network diagrams from natural language
- Templates for flowcharts, mind maps, etc.

**Best For:** Visual learners; quick topology planning



### 🧾 **Miro AI**
- Real-time collaboration whiteboard with AI enhancements
- Converts notes into diagrams, generates summaries

**Best For:** Mentoring remote students, planning labs together


### 🧩 **Excalidraw + GPT Plugin**
- Visual sketchpad with GPT-driven diagram generation

**Best For:** Rough network drafts and logical design sessions

### 🧜‍♀️ **Mermaid**
- Diagramming language

---

## 🧪 4. Lab Networking Tools

### 🧪 Containerlab

- A fast and flexible lab orchestration framework that lets you define, deploy, and manage realistic network topologies using containerized and virtualized network operating systems.
- Supports a wide range of NOSes like FRRouting, SONiC, Cisco IOS-XE, Cisco IOS XR, Cisco NX-OS
- Great for topology prototyping, testing, and CI/CD workflows in network automation.

### 🧪 Netlab
- A powerful topology automation tool that simplifies lab creation using YAML files and supports backends like Containerlab, VirtualBox, VMware, and more.
- Excellent for educational use, vendor-agnostic labs, and generating consistent configurations across platforms.
- Complements Containerlab by providing high-level abstraction and multivendor support.

## 🔍 5. Traffic Capture & Analysis

### 🦈 Wireshark
 - The industry-standard GUI tool for packet capture and deep protocol inspection.
 

### 🦈 EdgeShark
- A containerized web-based packet analysis tool, often deployed alongside labs in Containerlab.

---

## 🎓 6. Certifications

Cisco U is an adaptive learning platform that helps you build networking skills through structured learning paths, hands-on labs, and real-world scenarios. Whether you're starting with CCNA or preparing for your CCIE, Cisco U guides you with curated content and progress tracking tailored to your goals.

🔗 [Start learning at Cisco U](https://u.cisco.com)


### 🏢 Enterprise Track

####  CCNA (Associate)
- Covers foundational networking: routing, switching, IP services, security, wireless, and automation.


####  CCNP (Professional)
- Core exam (ENCOR) + concentration (e.g., advanced routing, SD-WAN, wireless).


####  CCIE (Expert)
- Focuses on large-scale network design, advanced troubleshooting, and automation.




### 🧱 Data Center Track

####  CCNP Data Center
- Core technologies: NX-OS, vPC, EVPN-VXLAN, storage networking, and basic ACI.


#### CCIE Data Center
- Covers advanced data center design and operations using NX-OS and ACI.




### 🌍 Service Provider Track

####  CCNP Service Provider
- Focus on routing protocols, MPLS, segment routing, QoS, and automation within SP environments.


####  CCIE Service Provider
- Advanced SP architecture, control plane scaling, traffic engineering, and service automation.


Cisco is actually revamping the Automation/Devnet track. More info about this later on.

### 🎥 7 - Cisco Live On-Demand Library

The [Cisco Live On-Demand Library](https://www.ciscolive.com/on-demand/on-demand-library.html#/) provides free access to hundreds of technical sessions from past Cisco Live events. These sessions cover deep-dives on core technologies, real-world deployment case studies, automation demos, and emerging trends — all presented by Cisco experts and engineers.

Whether you're exploring new topics, reinforcing cert knowledge, or staying current with the latest innovations, the on-demand content is an invaluable resource for continuous learning.