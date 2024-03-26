---
id: 1711413242-QYKN
aliases:
  - Certificates
tags:
  - PKI
---

# Certificates

## Web Server SSL Certificates 
### Domain Validation Certificate (DV) 
- The DNS domain matches the owner of the certificate 

### Extended Validation Certificate (EV) 
- Additional checks verify the DNS matches the owner 

### Subject Alternative Name (SAN) 
- Allows owner of certificate to add multiple DNS domains to the certificate
- Can create wildcard domains (*.com )
    - this means the certificate can suppourt any domain under this TLD

## Code signing certificate 
Developers create a certificate allowing the OS to verify the software is trusted 
- validates the code is unchanged
- the user can stop an unsigned app from executing offering protection 

## Root Certificate 
A public key certificate identifying the root Certificate Authority 
- root certificate verifies other Certificates from intermediate authorities
- this is extremely important to secure
    - anyone with the root certificate can verify any certificate they want 

## Self Signed Certificates
Certificates signed by an internal CA 
- only for internal use
- common in large organizations 
- All devices need to have the Internal CA installed on them 

## Machine and Computer Certificates 
Certificates installed on devices to authenticate them to internal networks 
- Authorize access
- VPN access etc

## Email Certificates 
Cryptographically signing emails 
- encryption
- digital signatures 
- can create integrity and non repudiation (can't deny sending)

## User Certificates 
A certificate associated with individual user
- elecronic "id" 
- can be additional authentication factor 
- cna integrate into physical ID card




