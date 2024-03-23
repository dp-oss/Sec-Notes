
EAP: Extensible Authentication Protocol 
- Many different ways to authenticate
-  integrates with 802.1X 

IEE 802.1X
- Port based network access control (NAC)
- Used with database of usernames/passwords
- Supplicant: Client
- Authenticator: Provides network Access
- Authentication Server: Stores authentication credentials 

EAP- FAST : Flexible Authentication via Secure Tunneling
- auth over encrypted channel 
- uses a shared secret 
- Supplicant and Auth Sesrver authenticate over the TLS tunnel 

PEAP: Protected Extensible Authentication Protocol 
- Encapsulates EAP in a TLS tunnel like FAST 
- Client doesn't use a certificate 
- Integrates with Microsoft and CISCO 
- Can be used with 

EAP TLS: EAP over TLS 
- requires digital certificate on the Auth server and all other devices 
- Complex implementation
	- need Public Key infrastructure 
	- must manage certs 
	- not all devices can use certs and thus can't authenticate 

EAP-TTLS: Eap over Tunneled transport Layer Security
- support other auth protocols over tls tunnel 
- Requires a single digital cert on the Auth server 
- Can be used with any other auth method 

RADIUS Federation: Members of one org can auth to another org over the RADIUS server 
- uses 802.1X typically 
