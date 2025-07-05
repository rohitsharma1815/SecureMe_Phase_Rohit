# 🧪 Ping Results Table

This document records the results of ping tests between the Windows host and the Ubuntu Linux VM.

---

## 🔁 Test Matrix

| Test No. | Source         | Target         | Command                       | Result     | Screenshot           |
|----------|----------------|----------------|-------------------------------|------------|----------------------|
| 1        | Windows Host   | Linux VM       | `ping 192.168.100.10`         | ✅ Success | `ping_success.png`   |
| 2        | Linux VM       | Windows Host   | `ping 192.168.100.20`         | ✅ Success | `ping_success.png`   |
| 3        | Linux VM       | Invalid IP     | `ping 192.168.100.254`        | ❌ Failed  | `ping_fail.png`      |
| 4        | Linux VM       | DNS name test  | `ping google.com`             | ✅ Success (if DNS ok) | *(Optional)*         |
| 5        | Linux VM       | DNS test fail  | `ping google.com` (bad DNS)  | ❌ Failed  | `ping_fail.png` (if DNS) |

---

## 🧾 Notes

- **Test 1 & 2** validate that both systems are on the same subnet (`192.168.100.0/24`).
- **Test 3** simulates a failed ping to a non-existent IP (useful for troubleshooting).
- **Test 4 & 5** reflect DNS-dependent behavior and connectivity to the outside world.
- Screenshots were taken using the system screenshot tool (`Snipping Tool` / `Flameshot` / `gnome-screenshot`).

---

📁 File path:  
`SecureMe_Phase1_YourName/Step4_Network_Config_Test/ping_results_table.md`
