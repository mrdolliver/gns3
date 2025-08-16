# GNS3 Lab Topology

This repository contains lab files, documentation, and network diagrams for experimenting with **GNS3** network simulations.

## Lab Topology

```
Internet
    |
 pfSense
(Firewall/VPN)
    |
┌────────┴────────┐
|                 |
Cisco IOSv1      Cisco IOSv2
(R1 - HQ)        (R2 - Branch)
|  \              /   |
|   \            /    |
Linux Host   WAN Emulator   VyOS Router
(Traffic)     (WAN delay)    (ISP)
```

## Components

- **pfSense** → Firewall & VPN gateway  
- **Cisco IOSv1 (R1 - HQ)** → HQ router  
- **Cisco IOSv2 (R2 - Branch)** → Branch router  
- **Linux Host** → Traffic generator/test host  
- **WAN Emulator** → Adds latency/bandwidth constraints  
- **VyOS Router** → Simulated ISP edge

## Usage

1. Open the GNS3 project file in GNS3.  
2. Import required appliance images (pfSense, Cisco IOSv, VyOS, Linux).  
3. Start devices and test connectivity.

---
✍️ Maintained by [mrdolliver](https://github.com/mrdolliver)

