**SRTP**:
Secure Real Time Transport Protocol / Secure RTP/SRTP
- adds security features to RTP
- encrypts conversations with AES
- Authenticates and repudiates
	- uses HMAC-SHA1
		- hash based message authentication using SHA1

**Time Synchronization**: 
NTP(Network Time Protocol) has no default security features leading to the introduction of NTPsec
- includes secure features 


**S/MIME**:
Secure/Multipurpose Internet Mail Extensions
- public key encryption and digital signing of mail content

**Secure POP and Secure IMAP**:
- uses STARTTLS extension to encrypt POP3 and IMAP with SSL

**SSL/TLS**
Secure sockets layer / Transport Layer Security

**HTTPS**:
HTTP over TLS 
- Uses public keys to verify symmetric keys which were encrypted using the private keys of the server you're attempting to communicate with
- uses Asym to transfer symm keys 
- Offers security and speed

**IPsec**:
Internet Protocol Security 
- secure OSI layer 3 
- authenticates and encrypts every packet sent 
- provides Confidentiality and integrity 
The two cores: 
- Authentication Header (AH)
	- Provides integrity 
- Encapsulation Security Payload (ESP)
	- Provides encryption

**File Transfer**: 
- FTPS:
	FTP over SSL 

- SFTP:
	SSH File Transfer Protocol 
	- Provides file system functionality 


**LDAP**: 
Lightweight Directory Access Protocol
	a protocol for reading and writing to directories over an IP network 
- organized set of records like a phone directory
- modern version of DAP 
- LDAP is the protocol used to update X.500 direcotries 
**LDAS**: 
LDAP over SSL

**SASL**:
Simple Authentication and security Layer 
- provides authentication layers for use in different applications 

**SSH**: 
Secure Shell
- encrypts terminal communication
- replaced Telnet and FTP 
- can communicate with other terminal and transfer files all encrypted 

**DNS**: 
Domain name system
- Originally had no security
	- dns could be easily poisioned
**DNSSEC**:
Domain name security extensions
- Validates origin using Public Key Cryptography


**SNMPv3**:
Simple Network Management Protocol v 3
- Added encryption to queries sent to routers and switches 
- Integrity means the data can't be tampered with 
- Authentication verifies the source of the data 
- Modifying routers and switches can be done over browser
	- ensure you use HTTPS
**DHCP**
Dynamic Host Configuration Protocol 
	Assigns local IPs to network devices 
- not secure inherently
- outdated
	- security needs to be put in place by using switch configuration rules 

