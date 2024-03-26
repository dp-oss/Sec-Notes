---
id: 1711319656-NJIM
aliases:
  - Securing Compute Clouds
tags:
  - Cloud
---

# Securing Compute Clouds
Compute clouds are the IaaS component responsible for computing calculations 
 - see: [[Cloud Models]]
- examples include Amazon EC2, Google GCE and Azure Virtual machines 

It's important to manage access to these computing engines 
- Firewalls can be used to control traffic flows in and out 
    - Layer 4: TCP or UDP port control 
    - Layer 3: Individual IP addresses, IPv4 or IPv6


## Dynamic Resource Allocation
Provision resources based on what's needed for applications 
- referred to as Rapid Elasticity when automated 
    - allows you to pay only for what's needed 
- Requires ongoing monitoring 


## Instance Awareness
Security controls based on what data is contained in application flows 
- Example: policies preventing PII from being uploaded to public cloud 


## Virtual Private Cloud Endpoints
Allows private access to cloud applications for internal use 
- keeps internal resources private 
- allows internal private subnet to access resources in other clouds without public connectivity 

## Container Security 
Containers can be as vulnerable as other deployment methods
- it can help to use container specific OSs 
    - minimal or hardened OSs
- Group like containers together 
    - this can focus security posture 
    - this can limit the scope of intrusions


