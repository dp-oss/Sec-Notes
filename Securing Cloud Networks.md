---
id: 1711319000-IINH
aliases:
  - Securing Cloud Networks
tags:
  - Cloud
---

# Securing Cloud Networks
Networks are used to connect different Cloud Components 
- connect users to the cloud 
    - can be vpn 
- connect cloud apps to one another
    - this can be east west (same data center) 
    - or north south (different data center) 


## Virtual Networks 
Clouds contain virtualized network devices
- severs 
- databases 
- routers 
- switches 
These are configured the same as physical hardware 
- the difference is that in the cloud they're on demand 
- rapid elasticity means that this hardware is created as needed 

## Public and Private subnets 
- Private 
    - all internal IPs 
    - connection over VPN 
    - not accessable from internet 
- Public 
    - external IPs 
    - accessible from internet 
- Hybrid 
    - Can contain both private and public subnets 


## Segmentation
Seperation of different components and services 
- adds security between components of an app 
- ex. seperate database from frontend 
- can be enhanced with security tech
    - WAF (Web application firewall)
    - Next Gen Firewall (NGFW) 
    - IPS (Intrusion Prevention System)
    - See:[[Secure Networking]] 

## APIs
API implementation can introduce security risks 
- to audit this we inspect API requests to ensure nothing is unnecesary 
