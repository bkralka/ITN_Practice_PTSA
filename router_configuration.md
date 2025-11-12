enable
configure terminal
hostname CS-Department
enable secret CiscoCCNA7
security passwords min-length 10
service password-encryption
banner motd #UNAUTHORIZED ACCESS PROHIBITED!#
line console 0
password CiscoCCNA7
login
exit
line vty 0 4
login local
transport input ssh
exit
ip domain-name csdept.local
crypto key generate rsa 
1024
ip ssh version 2
username netadmin secret CiscoCCNA7
interface g0/0
description *Connection to LAB 124-C LAN*
ip address 192.168.1.126 255.255.255.224
ipv6 address 2001:db8:acad:a::1/64
ipv6 address fe80::1 link-local
no shutdown
exit
interface g0/1
description *Connection to LAB 214-A LAN*
ip address 192.168.1.158 255.255.255.240
ipv6 address 2001:db8:acad:b::1/64
ipv6 address fe80::1 link-local
no shutdown
exit
ipv6 unicast-routing
end
write
