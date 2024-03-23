Control inbound and outbound network traffic
- control the flow of traffic in and out
- can block content 

**Network-based firewalls**: Filter traffic by port number and app
- can encrypt traffic for [[Virtual Private Networks]] between sites 
- Layer 3 devices (router)
	- NAT network address translation

**Stateless Firewall**: Doesn't keep track of traffic flowing 
- every packed is examined regardless of history 
- traffic sent outside a session will traverse stateless
- firewall can't determine what is a response to a specific request 

**Stateful firewall**: Remembers the state of a session 
- if the flow of traffic is valid the responses will be allowed 
- creates a session table to remember the state of traffic 

**UTM/ All in one security appliance**: Unified threat management (web security gateway)
- more features than regular firewall
	-  url inspection
	- malware inspection 
	- spam filter 
	- router switch
	- firewall 
	- IDS/IPS
	- VPN 
	- Bandwith Shaper
	- etc 

**NGFW Next generation firewall**: OSI Application layer device 
- can see all data in every packet 
- URL / content filtering 
- Intrusion prevention systems 

**Web application firewall WAF**: Applies rules to http/https firewalls 
- allow or deny based on the input 
	- can prevent injection attacks 
	- or XSS 
- Major focus in PCI DSS (payment standards) 

**Firewall rules**: whats allowed or blocked by a firewall 
- Access control list (ACL)
	- categories include :
		- ip 
		- port 
		- time of day
		- app 
	- rules follow a logical path 
		- typically top to bottom 
		- the first rules are followed first 
	- implicit deny 
		- traffic that doesnt violate a rule but doesn't match any allowed is blocked by default 



- open source firewalls provide more traditional functionality 
- closed source are more focused on application specific traffic, purpose built for it's functionality 

- Hardware  firewalls are more efficient 
- software firewalls are easier to install anywhere 


- Appliance based firewalls provide the fastest throughput 
- host-based firewalls can be application specific because they're on the endpoints
- virtual firewalls can provide east-west security on the network (across the same datacenter )


