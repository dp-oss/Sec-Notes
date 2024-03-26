---
id: 1711411681-XQZD
aliases:
  - Public Key Infrastructure (PKI)
tags:
  - Cryptography
---

# Public Key Infrastructure (PKI)
The process of managing digital certificates 
- policies 
- people 
- hardware 
- software
- procedures 

Can also refer to assosciating public keys to people and devices 
- This is the foundations of trust 

## Key management lifecycle 
- Key generation
    - Create key and choose strength
- Certificate generation 
    - allocate key to user
- Distribution
    - make key availible to user
- Storage
    - Securely store key and authorize proper use 
- Revocation
    - manage keys that are depreciated or compromised 
- Expiration
    - keys have a shelf life 

## Digital Certificate 
A public key combined with a digital signature 
- can contain details about key holder 
- digital signature adds trust 
- Certificate Authority verifies key and adds trust 
- Web of Trust can create trust 
    - this is other users signing keys GPG for example
- can be built into the OS 

## Commerical Certificate Authorities
- Built-in to browser 
- Allow us to purchase certificate which can then be trusted by peoples browsers 
- We create a key and ask to be signed 
    - through CSR Certificate Signing Request 
- need this on webserver to be a trusted website 

## Private Certificate Authorities 
CA built in house at an organization
- Provides signed certificates for internal Infrastructure 
- Needed for large orgs 

## PKI Trust Relationships 
- Single CA 
    - Everyone receives certificates from one Certificate Authority (CA)
Hierarchical
    - Single CA issues certificates to intermediate CAs 
    - this CA is called the Root CA 

## Registration Authority (RA) 
Seperate entity that approves or rejects the issuing of certificates 
- responds to CSRs 
- can handle revocation
- can handle renewal 
- Issues Certificate which is sent to Certificate Authorities

### Common Name (CN) 
FQDN (Fully Qualified Domain Name) on a certificate 
- every website only has one on their certificate 
- Subject Alternative name
    Addtional host names that can be used
    - ex. google.com, www.google.com

### Expiration 
- limit exposure to compromised sites
- 398 days is the limit in modern browsers

### Certificate Revocation Lists (CRL) 
Large list of revoked certificates stored by Certificate Authority 
- can be a very large file
### OCSP (Online Certificate Status Protocol) 
Feature in browsers that can preform checks of specific certificates
- communicates with a OCSP responder via HTTP 
- this is more efficient than dowloading an entire CRL
