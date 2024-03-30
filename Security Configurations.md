---
id: 1711765775-OHBA
aliases:
  - Security Configurations
tags: []
---

# Security Configurations
## Configuration Changes
- Firewall rules 
    - manage application flows
    - block dangerous apps 
    - see: [[Firewalls]]
- Mobile Device Manager (MDM) 
    - enable or disable phones and tablets 
    - regardless of physical location
    - see [[Mobile Device Management]]
- Data Loss Prevention (DLP) 
    - Block the transfer of PII 
    - see [[Data Loss Prevention (DLP)]] 
- Content/URL filtering 
    - block access to untrusted sites
    - Block malicious sites 
    - large blocklists share URLs of suspicious sites 
- Updating or Revoking certificates 
    - managing the certificates on the device can verify trust 
    - revoking a certificate can remove network access 

## Isolation
Moving device into an area where it can't access other resource s
- Network Isolation
    - isolate to remediation VLAN
    - can't communicate with other devices 
- Process Isolation 
    - limit application execution
    - can stop malicious activity but still allow remote management 

## Containment 
- application containment 
    - each app runs in it's own sandbox
    - limits interaction between host OS and apps 
- Containment can limit the spread of multi-device security events 
- see: [[Sandboxing]]

## Segmentation 
Seperating portions of the network
- prevents unauthorized movement
- limits the scope of a breach

## SOAR 
Security Orchestration, Automation, and Response
- integrates multiple third party tools 
- Runbooks: 
    - Linear checklist of steps to preform
    - Step-by-step approach to automation
- Playbook:
    - A broad process
    - combination of Runbooks
