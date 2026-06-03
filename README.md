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

<div class="mermaid">
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
</div>

* **Hardware & Software Lifecycle Management:** Led end-to-end tech refreshes for Cisco Catalyst, NX-OS, and ASR hardware—encompassing planning, configuration, deployment, and monitoring tools synchronization.
* **Bulk Policy & Security Automation:** Developed structured automation workflows utilizing CSV datasets to push bulk ACL updates and core OS upgrades via enterprise management tools, drastically reducing human error.
* **Wireless Mobility Optimization:** Engineered robust enterprise wireless troubleshooting matrixes using WLC to diagnose connectivity anomalies and streamline fault-tolerant AP provisions.
* **Proactive Architecture Standardization:** Authored comprehensive troubleshooting SOPs for L1/L2 engineering teams, moving from reactive debugging to data-driven proactive operations based on deep hardware ASIC buffer analysis.

---

## 🤖 Automation Lab

### Palo Alto Networks CLI Automation
Below is an example of the structured PAN-OS CLI automation workflows I design to handle large-scale network objects and static address groups efficiently:

```bash
# Shared Address Object Creation
set shared address 10.216.32.10 ip-netmask 10.216.32.10
set shared address 10.216.32.11 ip-netmask 10.216.32.11

# Static Address Group Enforcement
set shared address-group ci_7063851-corp-dag static 10.216.32.10
set shared address-group ci_7063851-corp-dag static 10.216.32.11
