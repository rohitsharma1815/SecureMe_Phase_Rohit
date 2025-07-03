## ip configurations on windows
Windows IP Configuration


Ethernet adapter Ethernet:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Local Area Connection* 11:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Local Area Connection* 12:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Ethernet adapter VMware Network Adapter VMnet1:

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : fe80::83df:1738:58d2:48de%19
   IPv4 Address. . . . . . . . . . . : 192.168.45.1
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . :

Ethernet adapter VMware Network Adapter VMnet8:

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : fe80::f765:5155:6a7:1d32%13
   IPv4 Address. . . . . . . . . . . : 192.168.139.1
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . :

Wireless LAN adapter Wi-Fi:

   Connection-specific DNS Suffix  . :
   IPv6 Address. . . . . . . . . . . : 2406:b400:35:5541:3d63:b690:3624:15b
   Temporary IPv6 Address. . . . . . : 2406:b400:35:5541:6d2e:aa0c:199b:1579
   Link-local IPv6 Address . . . . . : fe80::c768:13b3:b6bb:c532%22
   IPv4 Address. . . . . . . . . . . : 192.168.0.103
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . : fe80::3e64:cfff:fe31:25fa%22
                                       192.168.0.1

Ethernet adapter Bluetooth Network Connection 2:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :
## ip configurations on linux
 ifconfig
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 192.168.139.128  netmask 255.255.255.0  broadcast 192.168.139.255
        inet6 fe80::20c:29ff:fe2d:b46c  prefixlen 64  scopeid 0x20<link>
        ether 00:0c:29:2d:b4:6c  txqueuelen 1000  (Ethernet)
        RX packets 214381  bytes 304201701 (290.1 MiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 46646  bytes 7088921 (6.7 MiB)
        TX errors 0  dropped 74 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 1962  bytes 168708 (164.7 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 1962  bytes 168708 (164.7 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

