# VLAN Routing Lab (Router-on-a-Stick)

This Packet Tracer project demonstrates how to configure basic VLANs and enable communication between them using **Router-on-a-Stick** technique.

## 🧱 Topology Overview

- 🖥️ 2 PCs in different VLANs:
  - PC-0: VLAN 10 → IP: 192.168.1.10
  - PC-1: VLAN 20 → IP: 192.168.2.10
- 🔀 1 Cisco Switch (2960)
- 🌐 1 Router (with subinterfaces on Gig0/0)

## 🔧 Configuration Summary

- VLAN 10 and VLAN 20 were created on the switch.
- Switch ports Fa0/1 and Fa0/2 assigned to respective VLANs.
- Fa0/3 on the switch configured as **trunk port**.
- Router's Gig0/0 interface configured with:
  - Subinterface `Gig0/0.10` → 192.168.1.1 (for VLAN 10)
  - Subinterface `Gig0/0.20` → 192.168.2.1 (for VLAN 20)
- PCs have static IPs and default gateways pointing to router subinterfaces.
- Inter-VLAN routing tested successfully using `ping`.

## 📁 Files

- `vlan-routing-lab.pkt`: Main Packet Tracer file

## 🎯 Objectives

- Practice creating VLANs
- Learn how Router-on-a-Stick enables inter-VLAN communication
- Understand trunking and subinterface configuration

## 🧠 Skills Practiced

- VLAN segmentation
- Trunk port setup
- Subinterface routing
- Troubleshooting ping issues

---

🔁 _Created by Ali | GitHub: alasgarragimov_
