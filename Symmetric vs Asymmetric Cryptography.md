**Symmetric Encryption**:
Encryption using a single shared key ^3010f5
- the same key used to encrypt needs to be shared to decrypt the data
- Known as secret key algorithm
- Hard to scale 
	- How to distribute a key when you can't encrypt it yet? 
- Very fast to use 
	- less overhead 
- Often combined with asymmetric encryption



**Asymmetric Encryption**:
Encryption using two or more mathematically related keys. A private and a public key ^20a33d
- also known as Public Key cryptography 
- Private key
	- like symmetric this is yours and kept private 
- Public key
	- can be given to anyone else and shared
- Only the private key can decrypt data that has been encrypted with the public key
- The private key can't be derived from the public key 
- both keys are built at the same time 
- plaintext is encrypted with the public key and can only be decrypted using the private key
- requires more compute 

Asymmetric encryption is used to create symmetric keys by combining your private keys with another public and your public combined combined with another private key

**Elliptic curve cryptography (ECC)**: 
The use of elliptic curves instead of large prime numbers to produce private and public keys  ^0be8c2
- this uses less compute than using large primes 
