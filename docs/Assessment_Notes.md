# 🔎 SOC Assessment Notes – pfSense Firewall DoS Mitigation

---

## 🎯 Assessment Objective

This assessment was conducted to simulate a **network-level Denial-of-Service (DoS) attack scenario** and validate the effectiveness of **pfSense firewall rules** using both **firewall telemetry and packet-level network monitoring**.

The focus of this lab was on **firewall rule logic, traffic inspection, and defensive validation**, not intrusion prevention systems or rate-limiting mechanisms.

---

## 🧪 Assessment Scope

✔ WAN-side firewall rule configuration  
✔ Source-based traffic control  
✔ Protocol-specific handling (TCP / ICMP)  
✔ Controlled DoS traffic simulation  
✔ Firewall state and rule counter analysis  
✔ **Packet-level validation using Wireshark**

❌ No IDS/IPS  
❌ No traffic shaping  
❌ No rate limiting  
❌ No production environment  

---

## 🧱 Network Architecture

- Attacker system generating high-volume traffic  
- pfSense firewall positioned inline  
- Target system behind the firewall  
- Wireshark used on relevant interfaces for packet capture  

All attack traffic traversed pfSense, allowing **rule-based filtering and packet-level inspection**.

---

## 🚨 Attack Simulation

A controlled DoS-style traffic flood was generated from the attacker system toward the internal target.

The objective of the simulation was to:
- Generate excessive connection attempts  
- Observe packet behavior during the attack  
- Correlate firewall rule activity with captured traffic  

This traffic was generated **strictly for defensive testing**.

---

## 🧯 Firewall Rule Implementation

Firewall rules were configured on the **WAN interface** to:

- Match traffic from the attacking source  
- Control TCP and ICMP traffic independently  
- Observe state creation and byte counters  
- Block or allow traffic based on rule logic  

Rule ordering was maintained to ensure correct evaluation.

---

## 📊 Validation & Observation

Mitigation effectiveness was validated using:
- pfSense firewall rule counters (states / bytes)  
- Firewall log review  
- **Wireshark packet captures showing traffic reduction or suppression after mitigation**

---

## 📌 Documentation Purpose

This document demonstrates **practical, multi-layer validation of firewall-based DoS mitigation**, combining firewall telemetry with packet-level evidence.
