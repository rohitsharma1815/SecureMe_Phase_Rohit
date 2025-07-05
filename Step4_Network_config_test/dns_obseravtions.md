# 🌐 DNS Test Observations

This document captures DNS resolution tests performed between a Kali Linux guest and a Windows host system, focusing on successful and failed lookups to analyze DNS behavior


---

## ✅ Test 1 – DNS Working (Linux VM)

### 🔹 Command Used:
```bash
dig google.com

; <<>> DiG 9.20.9-1-Debian <<>> google.com
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 61326
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 512
;; QUESTION SECTION:
;google.com.			IN	A

;; ANSWER SECTION:
google.com.		256	IN	A	142.251.221.110

;; Query time: 4 msec
;; SERVER: 49.205.171.194#53(49.205.171.194) (UDP)
;; WHEN: Sun Jul 06 03:54:12 IST 2025
;; MSG SIZE  rcvd: 5

sudo nano /etc/resolv.conf
# Replaced with:
nameserver 1.2.3.4

dig google.com

 Observation:
Dig fails with timeout or unreachable message.

No IP resolution occurs.

Demonstrates DNS server unreachability.