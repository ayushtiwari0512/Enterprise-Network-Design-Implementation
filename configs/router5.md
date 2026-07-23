ISP#show running-config 
Building configuration...

Current configuration : 1014 bytes
!
version 12.4
no service timestamps log datetime msec
no service timestamps debug datetime msec
service password-encryption
!
hostname ISP
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
 duplex auto
 speed auto
 shutdown
!
interface FastEthernet0/1
 no ip address
 duplex auto
 speed auto
 shutdown
!
interface Serial0/0/0
 ip address 200.0.0.2 255.255.255.252
 clock rate 64000
!
interface Serial0/1/0
 ip address 200.0.0.6 255.255.255.252
 clock rate 64000
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
ip classless
ip route 192.168.0.0 255.255.0.0 200.0.0.1 
!
ip flow-export version 9
!
!
!
banner motd ^C unauthroized access prohibited ^C
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
