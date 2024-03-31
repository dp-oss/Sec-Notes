**VPN**: A means of sending encrypted data over a public network 

differ from [[Proxy Servers]]

**Concentrator**: Encryption/decryption device
- often in the firewall 
- communicates with software on endpoints 

- many deployment options 

**Remote Access VPN**: A VPN to access a private network from other insecure networks 


**SSL VPN (Secure Sockets Layer)**: Uses SSL/TLS protocol to communicate over tcp port 443 
- usually no firewall issues since 443 is common port 
- No need for big VPN clients 
- can be used to authenticate users 
	- doesn't requires digital certs 
- can be run from a small client or even a web client

**HTML5 VPN**: HTML5 api suppourts Web cryptography 
- can be used to create a SSL VPN connection directly from the browser 

**Full Tunnel VPN**: Everything sent by users is sent directly to VPN concentrator 
- this includes data meant for websites that are outside of the target network 

**Split Tunnel VPN**: Admins decide which data is sent through the concentrator 
- for example only data intended for internal net is sent through concentrator 

**Site to site VPN**: Use of concentrators to communicate from remote sites to the main corporate network 


**L2TP Layer 2 tunneling protocol**: Connecting 2 sites together over a layer 3 network as if they're the same network 
- commonly used with IPsec 


**IPsec**: Internet Protocol Security, security for OSI layer 3
- all packets are encrypted and signed 
- IPsec headers and trailers are added on to packets 
- Transport mode 
	- data is encrypted but the IP header is not 
- Tunnel Mode 
	- a new IP header is assigned and the OG IP Header and the data are encrypted 
- **Authentication Header (AH)**: The packet is hashed and a integrity check value (key) is shared and the hash is sent in an AH header along with the packet 
	- doesn't protect the data but does verify that it is unchanged 
- **Encapsulation Security Payload (ESP)**: Encrypts and authenticates the data 
	- data is sent encrypted along with an AH and an ESP header as well as an integrity check value 