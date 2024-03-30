---
id: 1711744250-KHHL
aliases:
  - Log Files
tags: []
---

# Log Files


## Network Log Files
Logs from switches, routers, APs, VPN concentrators and other ifrastructure devices 
- Changes to network
- routing updates
- Authentication issues
- network security 

## System Log Files
Information about operating systems 
- filesystem
- Authentication 
- Can include security events
    - brute force
    - file changes
- may require filtering 

## Application Log Files
Specific to apps 
- Windows: Event Viewer /ApplicationLog
- Linuxs: /var/log
- can be parsed in a [[SIEM]]

## Security Log Files
Detailed security information
- blocked/allowed traffic flows
- exploit attempts 
- Blocked URLs 
- DNS sinkhole traffic
    - see:[[Honeypots and Deception#DNS sinkhole]] 
- are collected by security devices
    - IPS, firewall, proxy etc. 
- Can be coorelated with other logs in a [[SIEM]]

## Firewall Logs
Detailed info about what traffic has been allowedand blocked 
- WAF can provide further details about application level attacks 
    - sql injection
    - cross site scripting 

## Web log files
Files relating to web server access 
- IP address, web URL
- Access errors
    - non existent files/folders
- exploit attempts

## DNS log files
Logs related to domain resolution
- view lookup requests
- IP of requests
    - also FQDN see:([[1711411681-XQZD#common-name-cn]]) 
    - Known bad URLS 
- C2 servers 

## Authentication Log Files
Accounting of who authenticated and who didn't 
- Account names
- IP
- methods of auth
- Success or failure 
- Multipole attempts 

## Dump files
Storing the contents of memory into a diagnostic files
- devs can use this information 
- Can be done right from windows task manager 
- some apps have their own dump methods 
- see: [[1711654258-EIBL#memdump|Forensic Tools ❯ `memdump`]]

## VOIP and Call Manager Logs
Information regarding calls and communications 
- inbound and outbound call info
- security information
- SIP traffic
    - sesion initiation protocol
    - call setup and management and teardown
    - inbound and outboudn calls 
    - Unusual numbers and country codes 

