---
id: 1712342588-WDOQ
aliases:
  - Credential Policies
tags: []
---

# Credential Policies

## Credential Management
- passwords must not be embedded in application
    - everything must be on server not client
- network communication needs to be encrypted
    - authentication traffic needs to be impossible to see in the clear

## Personnel Accounts
Accounts need to be associated with specific person 
- computer users ID number to identify specific users
- Storage and files need to be private to that user
    - allows multiple accounts on the same system
- Users shoud not have privileged access to the OS
    - least privilege 
- should be default for everyone connecting to the network
    - it should only use admin accoutns when required
## Third-party Accounts
Accounts for to access Third-party systems
- access seperate corporate systems
    - like vendors
- Additional security is valuable
    - 2FA
    - audit security posture of third parties 
- don't allow accoutn sharing
    - all Third-party users should have their own accoutns

## Device accounts
Accounts for mobile devices
- Local security
    - device certificate
    - require screen locks and unlock standards
    - manage through MDM 
- add additional security
    - geography based
    - include additonal auth factors
    - associate a device with specific user

## Serice Accoutns
Used exclusively be services running on the compputer
- not used by a specific user
    - web service 
    - database server
- access rights and premissions need to be set per service 
- commonly use usernames and passwords
    - you'll need to determine best Policies for password updates

## Administrator/root accounts
Elevated acccess to systems
- super user access
- complete control over OS 
    - manage hardware
    - install software
    - manage drivers
- should not be used for normal administration
    - only use when necessary 
- Need to be highly secured
    - strong passwords
    - enable 2FA
    - schedule password changes


