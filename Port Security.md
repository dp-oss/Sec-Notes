Goal is to maintain physical security of the network switch to maintain uptime and availability

- **Broadcasts**: Information sent from one person to all other connected to the network 
	- limited scope: can only broadcast to the same domain
	- can be limited with the use of VlANs 
	- can add up quickly 
	- can be maliscious 
	- IPv6 doesn't have these 
		- uses multi casts instead 
	- switches can control broadcasts, limiting their scope 
		- can limit by number 
		- can monitor the rate of broadcasts 

- **Loop Protection**: looping is when two networks are connected to each other sending traffic back and forth forever 
	- 802.1D standard created to prevent this 
		- known as spanning tree protocol 
		- ports are blocked to prevent loop back
		- spanning tree can detect outages and change routing to allow different flow of traffic
			- preventing down time
		- spanning tree takes time to determine which port should forward frames 
			- **BPDU guard**: Bridge Protocol Data Unit 
			- if a BPDU frame is sent then the interface is disabled preventing frames 

- **DHCP Snooping**: Tracks Ip on a 2 layer device (switch)
	- certain routers, DHCP servers and routers are trusted 
	- filters out the rest like a fire wall 

**MAC Filtering**: Allows admins to allow or disallow traffic based on the MAC or physical address of the device it's coming from 
- the problem is no layer 2 security to prevent people from snooping on the network to find the allowed addresses and change their MAC to match 