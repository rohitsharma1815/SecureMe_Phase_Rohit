# User Auth Configuration - Identification & Authorization

## Objective
Create users and configure file/directory permissions using Linux access control.

## Tools Used
- `useradd`, `passwd`
- `chmod`, `chown`

## Steps

1. **Create Users**
```bash
sudo useradd alice
sudo useradd bob
sudo passwd alice
sudo passwd bob
#create a shared dIRECTORY
sudo mkdir /shared_data
sudo chown alice:bob /shared_data
sudo chmod 770 /shared_data
 #set file permissions
 sudo touch /shared_data/confidential.txt
sudo chown alice /shared_data/confidential.txt
sudo chmod 640 /shared_data/confidential.txt

