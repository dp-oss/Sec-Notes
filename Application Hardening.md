Minimizing the attack surface of an application 

attempting to limit known and unknown attack points or vulnerabilities 

Some mandates require hardening:
- HIPAA
- PCI DSS 

**Open ports and services**: 
Every port open is a possible entry point
- can be done with firewall
	- [[Endpoint Protection#^826789|NGFW]] is even better
- Use Nmap or another port scanner to check which ports are being used 

**Registry**:
Large database in windows that holds configuration for the OS and applications that are installed
- third party tools that can detect changes in the registry after the installation of an applications
- registry can allow people to configure permissions
- good practice to backup the registry before making any changes 

**Disk [[Encryption and Cryptography|Encryption]]**:
Prevents application data from being accessed 
- **Full disk encryption (FDE)**
	- Encrypting everything on the drive 
	- examples include:
			- windows bitlocker
			- File Vault
- **Self-encrypting drive (SED)**: 
	- Hardware based full disk encryption
	- doesnt need management from an OS or any software
	- OPAL storage specification is the standard for this 


**OS Hardening**: 
Minimizing the attack surface of the operating system
- always keep the OS up to date 
	- latest patches and service packs
- User accoutns
	- ensure minimal password lengths 
	- principle of least privilege for all accounts
- Limit network access to only necessary access
- ensure monitoring for malware and virus 

**Patch Management**: 
The process of installing new updates to software and ensuring the system still functions
- important for stability and security 
- Third party apps also need to be updated
- Auto update can be useful for some people but can be bad if you need to test the update for stability before install 
- some OSs have emergency updates for 0day bugs

**[[Sandboxing]]**: 
Running coding in an isolated environment to prevent access to unrelated resources