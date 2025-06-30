# Audit Log Analysis - Audit Lab

## Objective
Analyze failed login attempts and implement automated detection.

## Tools Used
- `/var/log/auth.log`, `fail2ban`, `auditd`

## Steps

1. **Trigger Failed Logins**
```bash
su - invaliduser
# Or wrong SSH password
