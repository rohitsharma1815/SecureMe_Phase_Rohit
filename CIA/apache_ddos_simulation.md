# Apache DDoS Simulation - Availability Lab

## Objective
Simulate a DDoS attack to test system availability using `hping3`.

## Tools Used
- Apache2
- hping3
- Ubuntu

## Steps

1. **Install Apache**
```bash
sudo apt install apache2
sudo systemctl start apache2
##check website:
open  http://localhost in browser
# install hping3 tool
  sudo apt install hping3
#find your ip
ip a | grep inet
#simulate DDoS
  sudo hping3 -S -p 80 --flood YOUR_IP
 #check system load:
 write top command in bash
 


