# Sudo Logging - Accountability Lab

## Objective
Track privileged actions through sudo command logs.

## Tools Used
- `sudo`, `/var/log/auth.log`

## Steps

1. **Add User to Sudo Group**
```bash
sudo usermod -aG sudo alice
