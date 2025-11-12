enable
configure terminal
hostname LAB-214A-SW
service password-encryption
banner motd # AUTHORIZED ACCESS ONLY #
enable secret CiscoCCNA7
interface vlan 1
description *Management VLAN for LAB 214-A*
ip address 192.168.1.157 255.255.255.240
no shutdown
exit
ip default-gateway 192.168.1.158
line console 0
password CiscoCCNA7
login
exit
line vty 0 4
password CiscoCCNA7
login
transport input telnet
exit
end
write
