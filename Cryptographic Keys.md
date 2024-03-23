The larger the more secure

**Symmetric**: 
Tend to be 128bit or higher 

**Asymmetric:**
3,072bit or higher is common

**Key Exchange**: 
How to transfer keys without being able to encrypt
- Out of band exchange
	- telephone 
	- courier
	- in person
- In band 
	- Protect the key with other encryption methods
	- Use 


**Real-time encryption/decryption**: 
A client uses a servers public key to encrypt a symmetric key, the server can then decrypt this key and use it to encrypt the data 
- keys need to be changed often

**Diffie Hellman key exchange**: 
Using your own private key along with someone else's public key, they use their own private key along with your public key, this creates an identical symmetric key that you both have without having to share any private keys 


### Web server encryption keys

SSL/TLS uses encryption keys to protect communication to the server 
- the server has a private and public key
	- you send your data encrypted with the public and the server decrypts using it's own private 
- This creates a single point of failure on your servers encryption
- Attackers with access to the private key can rebuild all packets sent 
	- its best to have multiple methods of encryption
**Perfect Forward Secrecy (PFS)**:
A different method of key exchange doesn't use the servers private to transfer a symmetric key
- uses [[Symmetric vs Asymmetric Cryptography#^0be8c2|Elliptic curve]] or Diffie-Hellman ephemeral
- every session is using a different key pair to encrypt the symmetric key of each session
- PFS requires more compute than using the same key pair every time
- more secure 
- Requires browser support
	- common now 

