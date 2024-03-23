Databases and the data they contain must be protected 

Also taking into account compliance issues
- HIPA 
- GDPR

**[[Protecting Data#^419803|Tokenization]]**: 
Replacing sensitive data with non sensitive place holders

Passwords in a database should not be stored in plaintext instead they should be [[Hashing and Digital Signatures|hashed]]
- all passwords will have the same length message digest so telling them apart by length isn't possible 
- adding a [[Hashing and Digital Signatures#^47cbff|salt]] will prevent rainbow table attacks because even multiple of the same password will have different hashes 







