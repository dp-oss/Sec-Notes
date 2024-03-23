Encode information to make in unreadable without a key 
- original called plain text 
- encrypted called ciphertext

Encryption is a two way street, can be unencrypted with the correct key

**Confusion 
- ciphertext must be significantly different than plain text 

**Diffusion: 
- changing of one character in plaintext will change many characters of ciphertext 

**Types include:
- PGP 
- ChaCha

Authentication and access control:
- Only those with the keys can access
 Non repudiation
 - publishing with a key means its truly from you
 Integrity
 - data that is tampered will not fit the previous key 
**Cryptanalysis**: 
the art of cracking encryption 



Longer keys are typically more secure
- weak keys can be made stronger by preforming multiple cypher processes 
	- hash the hash of the hash etc.
- This is known as key stretching
- Libraries exist to preform key stretching in your code 


**Lightweight cryptography**: 
Research dedicated to cryptology that uses less compute
- prevalent because of the uprise in [[Embedded Systems#^ade99f|IoT]]


**Homomorphic Encryption (HE)**:
Preforming calculations on data while it's encrypted and store the results encrypted
- allows encrypted data to be computed upon without decryption


[[Symmetric vs Asymmetric Cryptography]]  

[[Cryptographic Keys]]
