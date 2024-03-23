- **Physical**
	- devices are physically separate 
	- known as air gapped  
	- web server in one rack and DB in another 
	- Servers must be connected physically to communicate 
	- may not be cost effective 
	- high maintenance (each one needs to be maintained)

- **Logical** 
	- **Virtual Local Area Networks (VLANs)**: Servers are separated logically not physically 
		- communication between vlans requires a direct connection or 3 layer device (router)
	- **Screened Subnet**: a logically segmented layer of the network that can be opened to the public but separtate from the internal network 
		- also known as DMZ 
	- **Extranet**: A private network for partners
		- usually requires authentication 
	- **Intranet**: Private network only accessible from the inside of your network 
		- internal servers for employees only 
		- never made available to public 
		- contains company data 

- **East-west traffic**: Traffic between devices within the same data center
	- fast response times 
- **North-south Traffic**: traffic from outside data center or sent outside data center

- **Zero Trust Policy**: nothing in the network is trusted 
	- all data flows are considered untrusted 
	-  everything subject authentication, encryption and other security controls 
	- a holistic approach to security 

- **Virtual**: [[Virtual Private Networks]]

- Useful for: 
	- performance 
	- security 
		- segment user's from databases

- required for compliance 
	- such as credit cards 
	- 