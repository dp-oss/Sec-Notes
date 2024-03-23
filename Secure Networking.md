Domain Name resolution (DNS) ip translating to domain name

**Domain Name System Security Extensions (DNSSEC)**
- Validate DNS Responses using [[Symmetric vs Asymmetric Cryptography#^20a33d|Public key encryption]]
- origin authentication (where it came form)
- data integrity 
- To do so DNS record are signed by a trusted third party

**DNS sinkhole**: Resolving malicious domains to a different location to prevent end users from accessing those malicious domains 
- can enable logging to determine who's infected 
- can allow for content filtering to determine what can be accessed on the network 

**Out-of-band management**: a separate interface for management (usually serial port) that allows for management of network devices 
- can access devices if the network isn't working 


**QoS**: Quality of service, different use cases have different requirements from the network
- VoIP needs real time to be clear
- database needs to be interactive 
- We prioritize applications to ensure QoS 



**IPv6 security**: 
- more addresses means harder to scan ports / ip 
- No need for **NAT**: network address translation
- No **ARP** or **ARP Spoofing**
- New attacks will appear 
	- neighbor cache exhaustion 

**Taps and port mirrors**: Can intercept network traffic 
- Physical taps can monitor traffic 
	- can be used by admins or threat actors
- Port mirrors are software taps  ^d54fcc

**Monitoring services**: constantly monitor the network and identify threats 
- experts at SOC security operations center 
- can be 24/7
- can help maintain compliance 

**FIM**: File Integrity Monitoring 
- monitor files that shouldn't be changed 
- Windows SFC (System file checker)
- Linux - tripwire 
- Many IPS solutions 


[[Firewalls]]
[[Network Access Control]]


**Jump servers**: highly secure device used to provide access to secure areas of the network
- very important to lock down a high risk security concern 

**Hardware security module (HSM)**: manage and control encryption in large environments
- can backup private keys 
- offload overhead of cryptography on web servers 

**Sensors and collectors**: aggregate network info in one place 
- logs are collected on each device ie firewall, ids/ips (sensor) and aggregated by the collector 
- can be sent to SIEM