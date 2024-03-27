---
id: 1711566002-TAKX
aliases:
  - Certificate Concepts
tags:
  - PKI
---

# Certificate Concepts

## Online and Offline CAs 
- the compromise of a CA would be extremely dangerous
    - attacker can sign whatever they want or create new certs 
- to prevent we distribute the load
    - one Root CA offline and several intermediate CAs 

## OCSP stapling 
Online Certificate Status Protocol 
- stapling means the OCSP status from a local CA is added into the SSL/TLS handshake\
- so that clients don't have to check for revoked certs at CA every time 

## Pinning 
Adding the certificate inside the application 
- the app then checks the certificate in the server during runtime 
- if the certs don't match the app can stop running 

## PKI trust relationships 
- Single CA 
    - Everyone receive certificates from one authority
- Hierarchical 
    - single CA issues certs to intermediate and leaf CAs 
- Mesh 
    - Cross certifying CAs 
    - they verify one another 
    - difficult to scale 
- Web-of-trust
    - alternative to traditional PKI 
    - Users sign the certs of oneanother 
    - if someone you trust trusts someone else then you can trust the other person 
- Mutual Authentication
    - Client authenticates to server and server authenticates to client

## Key escrow
Trusted third party holds decryption keys 
- need trust 
- need proper process and procedures to control access 

## Certificate Chaining 
- Chain of trust: 
    - List of all certs between server and the root CA 
- any certificate between the SSL certificate and the root cert is a chain certificate 
- web servers need to be configured with the proper chain or users will get an error

