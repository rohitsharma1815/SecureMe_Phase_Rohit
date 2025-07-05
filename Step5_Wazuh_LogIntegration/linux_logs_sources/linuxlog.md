# 🐧 Linux Logs Summary

This document highlights key log files from a Linux system (Ubuntu-based), using various tools like `tail`, `cat`, and `journalctl` to analyze system behavior, security, and service activity.

---

## 📁 Key Log Files

| Log File               | Purpose                                   |
|------------------------|-------------------------------------------|
| /var/log/syslog        | General system events and messages        |
| /var/log/auth.log      | Authentication and login attempts         |
| /var/log/dpkg.log      | Software installation logs (via apt)      |
| /var/log/kern.log      | Kernel-related messages                   |
| journalctl             | System-wide logs from services (systemd)  |

---

## 🔐 Sample: /var/log/auth.log

```bash
tail -n 20 /var/log/auth.log

Jul  6 02:34:01 kali CRON[2294]: pam_unix(cron:session): session opened for user root(uid=0) by (uid=0)
Jul  6 02:34:01 kali CRON[2294]: pam_unix(cron:session): session closed for user root
Jul  6 02:35:01 kali sshd[2317]: Failed password for invalid user admin from 192.168.1.15 port 54321 ssh2
Jul  6 02:35:05 kali sshd[2317]: Connection closed by authenticating user root 192.168.1.15 port 54321

Explanation:
This shows:

Scheduled cron jobs running (CRON)

A failed SSH login attempt (important for detecting brute force or unauthorized access)

Closed SSH session
sudo journalctl -xe | head -n 20

Jul 06 03:10:45 kali systemd[1]: Starting OpenSSH server...
Jul 06 03:10:45 kali sshd[2410]: Server listening on 0.0.0.0 port 22.
Jul 06 03:10:45 kali sshd[2410]: Server listening on :: port 22.
Jul 06 03:11:05 kali systemd[1]: Stopping User Manager for UID 1000...
