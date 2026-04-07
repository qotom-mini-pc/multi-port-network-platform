# Multi-Port Network Platform (2.5G / 10G / SFP+)

## Overview
This project explores a compact multi-interface network platform designed for edge computing, homelab, and network segmentation scenarios.

The system integrates multiple Ethernet interface types in a single device, allowing flexible deployment without relying on separate routing and switching hardware.

---

## Interface Layout

![Multi-port network interface layout](https://www.qotom.net/minipcimg/q31500st-s18/qotom-minipc-q31500st-s18-6.jpg)

The platform combines different network interface types:

- 6 × 2.5GbE (Intel i226-V)
- 2 × 10GbE RJ45 (Intel X540)
- 2 × 10GbE SFP+ (Intel 82599ES)

---

## Design Considerations

### Mixed-Speed Networking
Different interface types can be assigned to different roles:

- 2.5GbE for access devices and VLAN segmentation  
- 10GbE for high-throughput traffic (NAS / servers)  
- SFP+ for fiber or DAC-based uplinks  

---

### System Integration
Combining multiple network layers into one system can simplify deployment compared to traditional router + switch architecture.

---

### Thermal & Stability
Running multiple high-speed NICs in a compact enclosure requires:

- Active cooling
- Efficient airflow design
- Stable long-term operation under load

---

## Use Cases

- Multi-WAN routing
- NAS / storage networking
- VLAN segmentation
- Edge computing node
- Homelab environments

---

## Reference

Additional hardware reference documentation:

- [Hardware Overview](./hardware_overview.pdf)

---

## Notes

This project focuses on system structure and interface design rather than vendor-specific implementation.
