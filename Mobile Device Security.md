---
id: Mobile Device Security
aliases:
  - Mobile Device Security
tags:
  - Mobile
  - Devices
---

# Mobile Device Security


## HSM Hardware Security Module 
A device that handles cryptographic functions for a mobile device 
- Can be on a MicroSD 
- can store priv keys 
- can handle encryption overhead 


## Unified Endpoint Management (UEM) 
Allows us to manage security posture of mobile devices
- an evolution of MDM see: [[Mobile Device Management|mobile Device Management]]


## Mobile Application Management (MAM)
Remotely manage the applications running on endpoints 
- MDM still manages the device itself 
- can monitor the use of applications 
- can detect unauthorized apps 
- can wipe data of specific apps 

## SEAndroid 
Security Enhancements for Android
- Simmilar to to SELinux (Security-Enhanced Linux) 
- Access controls 
- Project from the NSA 
    - SELinux is too 
- Secures kernel, userspace and configuration tools 
- Default since 2013 
- Android daemons are protected (inaccesable by users)
- Changed Discretionary Access control (DAC) to Mandatory (MAC) 
- apps are isolated and sandboxed 
