Computing on-demand over the internet

**Pros:**  
- fast to implement, 
- massive storage capacity, 
- instantly available, 
- elasticity: easy to scale

**Cons**:  
- bandwidth limits, 
- data protections, 
- requires network connectivity

**Infrastructure as a Service (IaaS):** outsourcing equipment
- hardware as a service (HaaS)
- You still manage software and security of software
- ex. Web server provider

**Software as a service (Saas)**: Software you purchase that is acsessible  on command
- data and apps managed by a 3rd party 
- Complete application being offered (like google drive/mail)

**Platform as a service (PaaS):** 3rd party provides a platform to write applications 
- you develop the app and control the data
- 3rd party control everything else 


**Anything as a Service (XaaS):** Any service offered over internet
- Any IT function can be outsourced over the internet


**On Premises:** anything located in the same physical location your organization runs from 

**Off-premises/hosted:** not hosted on your organization's  main location hosted can mean not even on your own hardware 


**==Managed Service Provider (MSP)==**: a cloud service provider that provides general IT support for an organization 
- manages network
- backups/recovery 
- growth management
- **Managed Security Service Provider (MSSP)**: Specific to security functions 

**Cloud Deployment Models**:
- Public: Anyone can use
- Community: Several orgs sharing resources 
- Private: Your own virtualized local data center
- Hybrid: Mix of private and pub

[[Edge and Fog Computing]]


**Designing the Cloud:**


**Thin client:** basic system allowing access to apps running on a server 
- Virtual Desktop Infrastructure VDI 


**[[Virtualization]]**

**[[Containerization]]**

**Monolithic Applications:** One large application that does everything
- large code base 
- hard to make changes 

**Microservices and APIs (Application Programming Interfaces):** separated smaller applications that segment your code communicated with using the API 
- easier to secure
- one service going dark wont take everything out

**Serverless Architecture:** Separating apps into individual autonomous functions, removing OS from the equation
- Function as a Service (FaaS)
- Server logic runs in stateless compute containers
- only calls upon server logic when API is called upon

**Virtual Private Cloud:** (VPC) a pool of resources created in a public cloud 

**Transit Gateway:** A cloud router used to connect different users to resources on VPCs 
- often connected to through a VPN run by your organization

**Resource Policies:** Rules on who can access what in a cloud model
- Assigning permissions 
- lock access to certain regions 
- Allow specific IPs to make API requests 

**Service Integration and Management (SIAM):** software ensuring all different applications from separate cloud providers can function properly 
- view multiple cloud providers in one place 
- will be evolving with org 
- easier to manage

**[[Infrastructure as Code]]**
