---
id: 1711239970-WYUU
aliases:
  - Cloud Security Controls
tags:
  - Cloud
---

# Cloud Security Controls

## AZ 
Avalibility Zones 
- zones within a cloud region 
- each zone has independent infrastructure 
- allow apps to be HA (highly availible) 
    - Active/standby or active/active 
- use [[Load Balancing]]


## Resource Policies 
- Identity and access managment (IAM) 
    - who can access what in the cloud 
    - group based ie (Admins/users) 
- Granular policies
    - IP 
    - group 
    -date and time 


## Secrets managment 
Cloud often uses secret keys passwords and certificates 
- difficult to manage 
- seperate services exist to manage secrets and who can access them 
- create a log of who accesses what 

## Integration and auditing 
- Logs need to be consolidated accross various different platforms 
- common to use a [[SIEM]]
- Frequent audits validate security 
