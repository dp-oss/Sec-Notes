**Stream Ciphers**: 
Data is [[Encryption and Cryptography|encrypted]] one bit or byte at a time
- high speed
- low hardware complexity 
- Often used with [[Symmetric vs Asymmetric Cryptography#^3010f5|Symmetric encryption]]
	- not common with [[Symmetric vs Asymmetric Cryptography#^20a33d|Asymmetric encryption]] 

**Block Ciphers**: 
Data is Encrypted in blocks of bits that are a fixed length
- if data doesn't match block size perfectly padding is added 

**ECB (Electronic Codebook)**: 
Each block is encrypted with the same key
- too simple for most uses
- same blocks will have the same ciphertext

**CBC (Cipher Block Chaining)**: 
Each plaintext block is XORed with the previous ciphertext block
- similar to ECB
- adds randomization 

**CTR (Counter)**: 
Block cipher but uses a counter to encrypt successive values 


**GCM (Galois/Counter Mode)**:
counter mode combined combined with Galois authentication 
- common for SSH or TLS