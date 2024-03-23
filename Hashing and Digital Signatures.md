Uses a one way mathematical function to represent data as a string of text: a **Message digest

==its a one way trip

can be used to verify the integrity of a download
- do this by comparing the hash of the download provided on the website 
- often called a checksum


Can be used for storing passwords,  storing them as a hash means even if the hashed passwords get stolen the thief won't know the actual plain text
- Salt: Random data added to a password when hashing  ^47cbff
	- This prevents people with the same password from being able to access other account because every account will have a unique hash

can be used as a digital signatures 
create a hash of your plain text, encrypt the hash with your private key, this is now a digital signature, sent along with the plain text ^d2510e

the receiver decrypts using your public key, then they have a hash of the plain text, when received along with the plain text they know the message was the one you sent

- authentication 
- non-repudiation
	- tied to someone specific
- integrity

Every single hash should be different

**Collision:**
When two or more messages have the same message digest
- we want to avoid this 

**Types: 
- SHA256
- MD5
	- has problems with collision

