# 🧯 pfSense Firewall – Denial-of-Service (DoS) Mitigation Lab

This repository documents a **network security lab focused on mitigating Denial-of-Service (DoS) style attacks using pfSense firewall rules**, validated through **firewall telemetry and packet-level analysis with Wireshark**.

The project demonstrates how **stateful firewall rules on the WAN interface** can be used to identify, control, and suppress abnormal traffic patterns generated during a simulated DoS attack.

---

## 🎯 Project Objective

The objective of this project was to:

- Simulate a controlled DoS-style traffic flood
- Deploy pfSense as an inline firewall
- Configure **WAN-side firewall rules** to mitigate attack traffic
- Understand **block vs pass** rule behavior
- Monitor firewall state tables and rule counters
- Validate mitigation effectiveness using **Wireshark packet captures**
- Practice real-world firewall-based defensive validation

---

## 🧪 Environment Overview

| Component | Description |
|--------|-------------|
| Firewall | pfSense Community Edition |
| Attacker System | Linux-based system generating high-volume traffic |
| Target System | Internal host behind pfSense |
| Monitoring Tools | pfSense logs & counters, Wireshark |
| Mitigation Method | Firewall rules (no shaping / no IDS) |

---

## 🧱 Network Architecture

Attacker System → pfSense Firewall → Internal Target


All attack traffic was forced to traverse pfSense, allowing **rule-based inspection, state tracking, and mitigation**.

---

## 🧭 Defensive Workflow Demonstrated

1️⃣ Generate controlled DoS-style traffic  
2️⃣ Observe traffic behavior pre-mitigation  
3️⃣ Configure WAN-side firewall rules  
4️⃣ Apply protocol-specific controls (TCP / ICMP)  
5️⃣ Validate rule hits and state behavior  
6️⃣ Capture packets using Wireshark  
7️⃣ Confirm traffic reduction or suppression  

---

## 🔎 Key Security Concepts Demonstrated

- Stateful firewall operation  
- WAN interface hardening  
- Source-based traffic control  
- Rule order importance  
- Block vs Pass semantics  
- Packet-level validation of defenses  

---

## ⚠️ Ethical & Usage Notice

- All testing was conducted in a **controlled lab environment**
- No production or internet-facing systems were targeted
- Traffic generation was intentional and authorized
- Project is intended strictly for **defensive learning**

---

📌 *This repository is part of my cybersecurity portfolio and demonstrates hands-on experience with firewall-based DoS mitigation and network traffic analysis.*



