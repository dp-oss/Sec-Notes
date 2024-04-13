---
id: Identity and Access Services
aliases: []
tags: []
---

# Identity and Access Services

## RADIUS (Remote Authentication Dial-in User Service) 
A common AAA protocol 
- centralizes authentication to a central RADIUS server 

## TACAS (Terminal Access Controller Access-Control System
Another common authentication protocol 
- XTACAS (Extended TACAS) 
    - created by CISCO 
- TACACS+ is the modern standard

## Kerberos
Another authentication protocol 
- uses SSO so users only authenticate once 
- provides mutual authentication 
    - You auth to server and server auths to you 
    - protects agains man in the middle and replay 
- Created in 80s 
- integrated with microsoft AD 
- SSO works by granting user a session ticket when they first authenticate
    - only works with Kerberos devices 

## Selecting one 
- TACAS+: CISCO devices 
- Kerberos: microsoft devices 
- VPN  concentrators often talk to Kerberos server 

## IEEE 802.1X 
Port based network access control (NAC) 
Requires users to authenticate before accessing the network 
- EAP (Extensible Access Protocol) can integrate with this 
- used in conjunction with access database
    - RADIUS,LDAP, TACAS+ 


