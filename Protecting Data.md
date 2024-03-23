Protecting the data is a primary job task in info sec


**Data Sovereignty 
- data is subject to laws of the country it resides in 
- GDPR (Rules in the EU, EU data must be stored in EU )
- compliance laws may prohibit where you can store and move info

**Data Masking 
- hide some of the data
- IE Password:  \*\*\*\*\*\*\*\*


Data [[Encryption and Cryptography]]

**Data at-rest
- data stored on a device
- ==encrypt this
- apply premissions

**Data in-transit
- Being transmitted through the network
- hard to protect while traveling 
- use Firewall or IPS (Intrusion prevention system)
- Provide transport Encryption(TLS, IPSEC)


**Data in-use 
- actively processing in memory 
- almost always not encrypted because its easier to preform calculation on for the machine 
- attackers will attack RAM to get decrypted info

**Tokenization: ^419803
- Replacing sensitive data with a non sensitive placeholder
- Common to use with credit processing 
- not encryption or hashing - the data is just replaced and not mathematically connected to the original

**Info Rights Management (IRM)
- controls how data is used in documents 
- Restrict data access to unauthorized persons 
- 