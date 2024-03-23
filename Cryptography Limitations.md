not a perfect solution 
- not all implementations are the same 
every situation is different 


**Speed**: 
[[Encryption and Cryptography|Crypto]] adds overhead and can impact speeds
- Ensure you have enough compute to support encryption
- increased load

**Size**: 
When using [[Stream and Block Ciphers|Block Ciphers]] encrypting less than a block will increase its size to the size of the block 
- 8 bytes will become 16 if using AES

**Weak [[Cryptographic Keys|Keys]]**: 
- Larger keys are more difficult to brute force 

**Time**: 
Crypto and hashing increases wait times which may frustrate users 
- larger files take longer 
- [[Symmetric vs Asymmetric Cryptography#^20a33d|Asymm]] is slower than [[Symmetric vs Asymmetric Cryptography#^3010f5|symm]]
- 

**Longevity**: 
As CPUs increase in power brute force becomes far easier 
- good practice to retire keys 


**Predictability and entropy**: 
Randomization is crucial 
- hardware RNG can be predicted 
- a passphrase needs to sufficiently random

**Key Reuse**: 
Reuse of keys reduces complexity 
- if the keys compromised everything else is 
- [[Embedded Systems#^ade99f|IoT]] devices often have their keys embedded in firmware
	- meaning compromises will allow attacks on anything running that firmware 

**Resource vs sec constraints**: 
devices with limited compute don't have overhead to encrypt
- real-time applications can't be delayed 
- 