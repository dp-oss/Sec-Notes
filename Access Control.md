---
id: 1711410863-QEDU
aliases:
  - Access Control
tags: []
---

# Access Control

## Authorization
The process of ensuring the approved rights are exercised by users 

## Mandatory Access Control (MAC) 
Access control through clearance levels which are assigned to all objects
- Users are assigned clearance levels which allows them to access certain objects 
- common in gov, or med 
- everything controlled by admins 

## Discretionary Access Control (DAC) 
Authorization is set by the 'owners' or creators of objects 
- common in many OSs especially windows  
- flexible but potentially weak in security 

## Role-based Access Control (RBAC) 
Roles are assigned to everyone in an organization which determine access
- admins provide access based on the users role 
- windows does this through group policy 

## Attribute-based Access Control (ABAC) 
Authorization based on a specific often complex set of attributes
- can be based on the data type, time of day, ip etc. 

## Rule-based Access Control
Generic term for Authorization based on specific rules 
- admins are set by the admins 
- rules can be object specific 
    - Network has its own rules 
    - documents and spreadsheets another 
- EX. Lab network only accessible at certain times
    - or document can only be accessed in google docs 

## File System Security 
Access control built into file systems of OSs 
- sometimes called Access Control list ACL 
- can be managed centerally or Discretionarily by users 
- can have encryption built in to enforce accesss control 
- ex. groups in linux 

## Conditional Access 
Allows admins to set specific conditions to authorize access or apply controls 
- allow or block access
- require MFA 
- provide limited access 
- Admins can build complex rules in modern systems 

## Privileged Access Management (PAM) 
The management of elevated access 
- admins and root 
- Privileged accounts are stored in central vault
    - they are handed out temporarily as needed 
- Advantages:
    - Centralized passwords
    - enables automations 
    - helps auditing

