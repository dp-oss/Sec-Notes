---
id: 1711406704-GWTP
aliases:
  - Authentication Management
tags:
  - Authentication
---

# Authentication Management

## Password keys 
Physical device that allows authentication
- usb token 
- **Something you have** 
- doesn't replace other factors
    - can be stolen 
    - use other factors too 

## Password Vaults
Programs that encrypt and store a list of passwords 
- a database of credentials 
- can sync with cloud 
- Use KeePassXC its the best one :) 
- helps create unique credentials for each service 
    - helps limit the scope in the event of breach 
- can be used for personal or enterprise use 

## Trusted Platform Module (TPM)
Hardware that helps with cryptographic functions 
- random number gen
- key gen 
- have persistent memory that stores keys from production
- can securely store keys for encrypted 
- also see [[Boot Integrity]] 

## Hardware Security Module (HSM) 
High end cryptographic hardware to help with crypto functions usually in servers 
- can secure encryption keys 
- crypto accelerators help offload CPU overhead from crypto functions
- Used in large enviornments
- use redundent powersupplies to ensure availibility
    - see [[Power Redundancy]]
- also see [[Mobile Device Security#hsm-hardware-security-module]]

## Knowledge-based Authentication (KBA) 
Using personal knowledge as an authentication factor
- Static KBA 
    Pre configured shared secret
    - think sercurity questions 
- Dynamic KBA 
    Questions are based on identity verification services 
    - what was the street number of your house when you lived in tallahasse florida in 2009 
    - you don't set the questions before


