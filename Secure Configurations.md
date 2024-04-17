---
id: 1712340600-DRLJ
aliases:
  - Secure Configurations
tags: []
---

# Secure Configurations
No system is secure by default Configurations we need to harden our operating systems and services 

## Web Server Hardening
One of the most common servers on the internet
- publicly facing 
    - this prevecnts potential for access issues
- Secure configuration
    - prevent information leakage
    - premissions
        - run from a non privileged account
    - configure SSL:
        - manage and install certificates
    - Log Files
        - monitor access and error logs

## Operating System Hardening
Many and varied operating systems
- Updates
    - run latest updates and security patches
- User accounts: 
    - min password length/complexity
    - account limitations
    - premissions 
- Network access and security
    - limit network access
- monitor and secure
    - antivirus/malware

## Application Server 
- Programming languages, runtime, libraries
    - usually between server and database
    - middle ware
- very specific functionality 
    - disable unused services 
- Operating System updates
    - security patches
- File Premissions and access controls
    - limit rights to whats required
    - limit access from other devices 

## Network Infrastructure devices 
Switches, routers, firewalls ,IPS etc.
- Purpose built
    - usually embedded os with limited access
- Configure authentication
    - change default credentials 
- Check with manufacturer
    - security updates
    - not updated as frequently as endpoints
