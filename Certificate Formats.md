---
id: 1711563706-WEVF
aliases:
  - Certificate Formats
tags:
  - PKI
---

# Certificate Formats

## X.509 
A standard format for digital certificates 


### DER (Distinguished Encoding Rules) 
A set of rules that allow for encoding data
- used with X.509 certificates 
- common with Java certificates 
- binary (not human readable) 
### PEM (Privacy-Enhanced Mail) 
A BASE64 encoded DER certificate 
- can be transfered as text in an email (email may change binary) 
- easy to read 

## PKCS #12
Public key Cryptography Standard 12
- container format used to send many certificates at once 
- store many X.509 certificates 
- often usedd to transfer a private public key pair
- can be password protected 
- .p12 or .pfx file formats

## CER (Certificate) 
Windows format for digital certificates 
- can in encode DER or PEM formats
- common to manage certs in windows 

## PKCS #7 
Public key Cryptography Standard 7 
- .p7b format 
- ascii (human readable) 
- can be transfered over email 
- widely supported 



