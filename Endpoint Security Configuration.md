---
id: 1711765376-PVYA
aliases:
  - Endpoint Security Configuration
tags: []
---

# Endpoint Security Configuration
Endpoints are devices that the end user ueses
- PC
- tablet
- phone
- laptop etc.

## Application Approve/Deny lists
Any app can be dangerous, security team makes policy to limit the execution of unknown apps 
- Approve list: 
    - nothing runs thats not approved
    - very restrictive 
- Deny lists: 
    - nothing on the deny list can be run 
    - Anti-virus anti-malware will stop apps from running
- Quarentine:
    - Anything suspicous is moved to a secure area 
- hashes of executables can be compared to those on the approve/deny lists 
- Certificates from specific publishers can be selected on the allow lists 
- Path to the executable can be allowed or denied
    - setting premissions to these folders can allow you to control exactly what can run on a system
- Network zones can be used to determine what can run 

also see: [[Endpoint Protection]]
