R1HO#show running-config 
Building configuration...

Current configuration : 2203 bytes
!
version 12.4
no service timestamps log datetime msec
no service timestamps debug datetime msec
service password-encryption
!
hostname R1HO
!
!
!
!
!
!
!
!
no ip cef
no ipv6 cef
!
!
!
!
!
!
!
!
!
!
no ip domain-lookup
!
!
spanning-tree mode pvst
!
!
!
!
!
!
interface FastEthernet0/0
 no ip address
 ip nat inside
 duplex auto
 speed auto
!
interface FastEthernet0/0.10
 encapsulation dot1Q 10
 ip address 192.168.10.1 255.255.255.0
 ip access-group 100 in
 ip nat inside
 standby version 2
 standby 10 ip 192.168.10.254
 standby 10 priority 110
 standby 10 preempt
!
interface FastEthernet0/0.20
 encapsulation dot1Q 20
 ip address 192.168.20.1 255.255.255.0
 ip nat inside
 standby version 2
 standby 20 ip 192.168.20.254
 standby 20 priority 110
 standby 20 preempt
!
interface FastEthernet0/0.30
 encapsulation dot1Q 30
 ip address 192.168.30.1 255.255.255.0
 ip nat inside
 standby version 2
 standby 30 ip 192.168.30.254
 standby 30 priority 110
 standby 30 preempt
!
interface FastEthernet0/1
 no ip address
 duplex auto
 speed auto
 shutdown
!
interface Serial0/0/0
 ip address 10.0.0.1 255.255.255.252
 ip nat inside
 clock rate 64000
!
interface Serial0/1/0
 ip address 200.0.0.1 255.255.255.252
 ip nat outside
!
interface Serial0/2/0
 no ip address
 clock rate 2000000
 shutdown
!
interface Serial0/3/0
 no ip address
 clock rate 2000000
 shutdown
!
interface Vlan1
 no ip address
 shutdown
!
router ospf 1
 log-adjacency-changes
 passive-interface FastEthernet0/0
 passive-interface FastEthernet0/0.10
 passive-interface FastEthernet0/0.20
 passive-interface FastEthernet0/0.30
 network 192.168.10.0 0.0.0.255 area 0
 network 192.168.20.0 0.0.0.255 area 0
 network 192.168.30.0 0.0.0.255 area 0
 network 10.0.0.0 0.0.0.3 area 0
!
ip nat inside source list 1 interface Serial0/1/0 overload
ip classless
ip route 0.0.0.0 0.0.0.0 200.0.0.2 
!
ip flow-export version 9
!
!
access-list 1 permit 192.168.0.0 0.0.255.255
access-list 100 deny ip 192.168.10.0 0.0.0.255 192.168.20.0 0.0.0.255
access-list 100 permit ip any any
!
banner motd ^C unauthorized access prohibited ^C
!
!
!
!
line con 0
 password 7 0822455D0A16
 login
!
line aux 0
!
line vty 0 4
 password 7 0822455D0A16
 login
!
!
!
end
