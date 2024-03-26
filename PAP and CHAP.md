---
id: 1711407383-QCFO
aliases:
  - PAP and CHAP
tags:
  - Authentication
---

# PAP and CHAP
Clients on the public internet need to authenticate into our local network using VPNs, we send the authentication request to a AAA server to approve or deny 

## PAP (Password Authentication Protocol) 
A basic method of authentication used in older OSs 
- in the clear! no encryption 
    - the application would need to provide encryption 
    - because of this PAP is weak
- designed in the dialup days 
- often times the app will encrypt the password but not the username 

## CHAP  (Challenge Handshake Authentication Protocol)
- Threeway Handshake 
    - CHAP server sends a challenge message 
    - cliente responds with Password  challenge hash
    - server evaluates password and challenge hash 

## MS-CHAP
Microsofts version of CHAP 
- uses DES ecnryption which is deprecieated 
    - this means it's weak
- we don't really use this anymore
