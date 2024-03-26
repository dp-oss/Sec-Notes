---
id: 1711405265-NAHM
aliases:
  - Account Types
tags:
  - Accounts
---

# Account Types

## User accounts 
Associated with a specific individual 
- OS uses an identification number 
- Files can be made private to the user
- do not have privileged access to the OS 
- this is what most users should be using 
    - even admins for most of their work 

## Shared Accounts 
Used by more than one person 
- hard to audit 
    - non repudiation (people can deny an action) 
- password management is difficult 
- hard to provision privileges 
- best practice **DONT USE THESE** 

## Guest accounts 
Shared account with limited access 
- can't change settings 
- no password usually 
- can be security risk
    - privilege escalation vulnerabilities 
- not default enabled 

## Service account 
Account used by background services that need access to certain files
- not interactive 
- can set premissions for each service 
    - [[Principle of Least Privilege]]
- commonly use uesrname and passwords
    - change the defaults 
    - set policy for PW updates 

## Privileged Accounts
Accounts with elevated access 
- complete system access 
- admin/root
- should only be used when necessary 
    - [[Principle of Least Privilege]]
- needs to be highly secured 
    - 2FA 
    - strong pass 
    - change pass frequently
