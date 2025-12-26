# ⚠️ Misconfiguration & Exposure Analysis – pfSense Firewall

---

## 🔍 Overview

This document analyzes **firewall misconfigurations and visibility gaps** that can increase susceptibility to DoS attacks when packet-level monitoring and rule-based controls are absent.

---

## 🚫 Lack of Source-Based Firewall Rules

Without explicit source-aware rules, attack traffic may reach internal systems unfiltered.

**Impact**
- State table exhaustion  
- Service degradation  
- Increased attack success  

---

## 🚨 Overly Permissive WAN Policies

Broad allow rules on WAN interfaces expose services unnecessarily.

**Impact**
- Unrestricted inbound traffic  
- Simplified DoS execution  
- Reduced attack containment  

---

## 🧱 Poor Rule Ordering

Improper rule ordering may prevent mitigation rules from triggering.

**Impact**
- Intended blocks bypassed  
- False sense of protection  

---

## 👁️ Absence of Packet-Level Visibility

Relying only on firewall logs without packet capture limits understanding of traffic behavior.

**Impact**
- Incomplete attack analysis  
- Difficulty validating mitigation effectiveness  

---

## 🧠 Root Cause Summary

DoS exposure often results from:
- Weak WAN-side filtering  
- Missing source controls  
- Lack of packet-level monitoring  
- Insufficient validation  

These issues are common in under-hardened firewall deployments.
