---
id: Securing Cloud Storage
aliases: []
tags:
  - Cloud
---

# Securing Cloud Storage 

- important to limit access
- geographical location 
- availability is important as cloud evolves 


## Permissions 
Proper permissions ensure authorization for access 
- some services set public by default 
    - not best practice obviously 
- Identity and Access Management
- Bucket policies 


**DONT PUT IT IN THE CLOUD IF IT DOESNT NEED TO BE THERE** 

## Encryption 
Data in the cloud is more accessible to everyone good and bad
This means data needs to be encrypted at rest 
- Server Side encryption means that its encrypted in the cloud 
- Client side means that its encrypted on the client and then sent to the cloud (in transit too) 
- good key Managment is important for either 


## Replication 
Create multiple copies of data in the cloud in different locations
- good for disaster recovery 
- high availibility 
- see [[Site Resiliency]]
