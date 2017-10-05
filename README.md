# c.code
transfer


Switch#show run
Building configuration...

Current configuration : 1294 bytes
!
version 12.2
no service pad
service timestamps debug uptime
service timestamps log uptime
no service password-encryption
!
hostname Switch
!
!
no aaa new-model
switch 2 provision ws-c3750-24p
system mtu routing 1500
ip subnet-zero
!
!
!
!
!
!
!
!
!
spanning-tree mode pvst
spanning-tree extend system-id
!
vlan internal allocation policy ascending
!
!
!
interface FastEthernet2/0/1
!
interface FastEthernet2/0/2
!
interface FastEthernet2/0/3
!
interface FastEthernet2/0/4
!
interface FastEthernet2/0/5
!
interface FastEthernet2/0/6
!
interface FastEthernet2/0/7
!
interface FastEthernet2/0/8
!
interface FastEthernet2/0/9
!
interface FastEthernet2/0/10
!
interface FastEthernet2/0/11
!
interface FastEthernet2/0/12
!
interface FastEthernet2/0/13
!
interface FastEthernet2/0/14
!
interface FastEthernet2/0/15
!
interface FastEthernet2/0/16
!
interface FastEthernet2/0/17
!
interface FastEthernet2/0/18
!
interface FastEthernet2/0/19
!
interface FastEthernet2/0/20
!
interface FastEthernet2/0/21
!
interface FastEthernet2/0/22
!
interface FastEthernet2/0/23
!
interface FastEthernet2/0/24
!
interface GigabitEthernet2/0/1
!
interface GigabitEthernet2/0/2
!
interface Vlan1
 no ip address
!
ip classless
ip http server
ip http secure-server
!
!
control-plane
!
!
line con 0
line vty 5 15
!
end
