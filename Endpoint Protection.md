The endpoint is the user's access point 

Protecting is multi-faceted
- Referred to as defense in depth 

**Anti-Virus and anti-malware**:
Designed to stop a broad array of malware using a known list of malicious signatures 


**Endpoint detection and Response (EDR)**: 
Uses other methods to search for malicious software 
- behavioral analysis
- Machine Learning 
- Process Monitoring 
Can often find the root cause of malicious activity
Can automatically respond to threats 


**[[Data Loss Prevention (DLP)]]**:
Detects and prevents the leak of sensitive data from an organization 
- often requires multiple solutions 
- orgs often use cloud based systems so those need to be defended too 


**Next-generation Firewall (NGFW)**: 
Operates in the OSI application layer  ^826789
- can view data in every packet sent over IP 
- Also referred to as deep packet inspection
- Allows for broad controls over security policies 
- Can feature [[SSL and TLS inspection]]


**Host-based firewalls**: 
Firewalls run on the endpoints 
- Allow or disallow traffic on an applications specific level
- Can block specific OS processes 
- Can view in the clear data because it's on an endpoint 

**Host based Intrusion Detection System (HIDS)**: 
Uses logs to identify and stop attacks 

**Host based Intrusion Prevention System (HIPS)**: 
Recognize and block known attacks as they occur
- often built into antivirus/malware
-  signatures 
- heuristics
-  behavioral analysis
	- buffer overflow
	- registry updates
	- writing files to the windows folder 
- full access to all data in the clear on a system
- 