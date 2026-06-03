# David Sung | Staff Network Engineer

Welcome to my infrastructure portfolio. I am a professional Staff Network Engineer with nearly 20 years of total IT industry experience, specializing for over 10 years in enterprise networking, hybrid cloud architectures, and network automation.

---

## 🛠️ Technical Expertise

* **Core Networking:** Cisco ACI Fabric, VXLAN, BGP Routing Policies, OSPF, EIGRP, Cisco SDA/DNA
* **Security & Firewalls:** Palo Alto Networks (PAN-OS), Object/Policy Automation, Zero Trust Governance
* **Automation & IaC:** Python, Ansible, Netmiko, Netbox, CI/CD Integration
* **Wireless & Mobility:** Cisco WLC/AP (CAPWAP), Aruba, Meraki Wireless

---

## 🚀 Key Professional Milestones

### Enterprise Infrastructure Operations & Tech Refresh

```mermaid
graph TD
    subgraph MGMT [1. Management & Security Automation]
        direction LR
        EMC[SMART EMC Platform] -->|CSV Mapping| Bulk[Bulk ACL & OS Upgrade]
        AAA[AAA / SNMP Controls] --> Sec[Device Hardening]
    end

    subgraph INFRA [2. Cisco Infrastructure Lifecycle]
        direction LR
        ASR[ASR WAN] --> NX[Nexus Core] --> Cat[Catalyst LAN]
    end

    subgraph WIRELESS [3. Wireless Mobility]
        direction LR
        WLC[Wireless Controller] --> AP[CAPWAP AP Swap & Site Assign]
    end

    subgraph OPS [4. Day-2 Ops & Asset Control]
        direction LR
        INC[On-Call Outage / INC Tickets] --> Visio((Update Site Visio))
    end

    %% Flow links
    Bulk --> INFRA
    INFRA --> WIRELESS
    INFRA --> OPS
