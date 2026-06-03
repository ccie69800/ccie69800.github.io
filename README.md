# ccie69800.github.io
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
