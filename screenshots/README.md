# 📸 Screenshot Reference – pfSense Firewall DoS Mitigation

All screenshots in this directory were captured from a **controlled lab environment** and are included strictly for **documentation and learning purposes**.

Screenshots demonstrate **firewall rule behavior, traffic observation, and packet-level validation**, not production configurations.

---

## 🧱 Firewall Rule Configuration

- **wan-firewall-rules.png**  
  WAN-side firewall rules configured to control inbound traffic during the DoS simulation.

- **rule-order-validation.png**  
  Verification of rule order to ensure correct evaluation and mitigation.

---

## 📊 Firewall Monitoring & States

- **firewall-rule-counters.png**  
  Rule hit counters and state tracking during attack traffic.

- **firewall-log-entries.png**  
  Firewall logs showing blocked and allowed traffic behavior.

---

## 🌐 Network Traffic Observation (Wireshark)

- **pre-mitigation-traffic.png**  
  Packet capture showing high-volume traffic before firewall mitigation.

- **post-mitigation-traffic.png**  
  Packet capture demonstrating reduced or suppressed traffic after firewall rules were applied.

---

## 📝 Notes

- Screenshots do not contain sensitive data  
- IP addresses and hostnames are lab-specific  
- Evidence supports **firewall-based mitigation validation**
