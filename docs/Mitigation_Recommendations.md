# 🛡️ Mitigation & Hardening Recommendations – pfSense Firewall

---

## 🚩 Firewall Rule Hardening

✔ Apply explicit WAN-side firewall rules  
✔ Restrict traffic based on source and protocol  
✔ Separate TCP and ICMP handling  
✔ Maintain strict rule ordering  

---

## 📊 Monitoring & Validation

✔ Monitor firewall state tables regularly  
✔ Review rule hit counters during anomalies  
✔ **Use Wireshark to validate traffic behavior before and after mitigation**

---

## 🧱 Defensive Architecture

✔ Keep firewall inline between threat sources and targets  
✔ Reduce exposed services  
✔ Apply least-privilege network access  

---

## 🧠 Operational Best Practices

✔ Test firewall rules under simulated attack conditions  
✔ Correlate firewall logs with packet captures  
✔ Document mitigation logic and validation steps  

---

## 📌 Summary

Effective DoS mitigation requires **correct firewall rules combined with packet-level validation**, ensuring defensive controls work as intended.
