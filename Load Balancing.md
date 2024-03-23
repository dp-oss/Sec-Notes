Distributing web traffic between different servers 

- creates fault tolerance
	- if one server fails the other take over

- can offset TCP overhead from servers
- offsets SSL overhead from servers as well 
- can offer caching services for common responses from servers 
- Can provide Prioritization to increase QoS
- Content switching
	- application specific load balancing
#### Scheduling
- **Round Robin**:
	- each server selected in tern
- **Weighted round-robin**:
	- Prioritize the server use
- **Dynamic Round-robin**:
	- monitor loads and distribute to the lowest 

**Affinity**: 
Making sure a user is always distributed to the same server 
- this is required for some applications 
- known as session persistence
- tracked through IP and session IDs

 **Active Passive**:
-  some servers are active while others are on standby 
-  if an active fails a passive takes over
