# 🐧 Linux Logs Summary

**System**: Kali Linux Virtual Machine  
**Log Date**: 1 July 2025  
**Log Location**: `/var/log/syslog` and `/var/log/auth.log`

---

## 🔧 System Log (`/var/log/syslog`)

### Last 20 Lines (Tail)
Jul 1 14:00:23 kali systemd[1]: Started Update UTMP about System Boot/Shutdown.
Jul 1 14:01:12 kali systemd[1]: Starting Daily apt upgrade and clean activities...
Jul 1 14:01:12 kali systemd[1]: Finished Daily apt upgrade and clean activities.
Jul 1 14:03:25 kali gdm3: GdmDisplay: display lasted 0.654 seconds
Jul 1 14:05:40 kali kernel: [ 1.200123] audit: type=1400 audit(1625147134.342:2): apparmor="STATUS" operation="profile_load"
Jul 1 14:06:15 kali systemd[1]: Reached target Graphical Interface.
ul 1 14:12:54 kali sshd[1023]: Accepted password for kali from 192.168.1.10 port 54321 ssh2
Jul 1 14:12:54 kali sshd[1023]: pam_unix(sshd:session): session opened for user kali by (uid=0)
Jul 1 14:15:09 kali sudo: kali : TTY=pts/0 ; PWD=/home/kali ; USER=root ; COMMAND=/bin/apt update
Jul 1 14:15:09 kali sudo: pam_unix(sudo:session): session opened for user root by kali(uid=0)
Jul 1 14:16:02 kali sudo: pam_unix(sudo:session): session closed for user root