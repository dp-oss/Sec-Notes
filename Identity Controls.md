---
id: 1711323399-OUNA
aliases:
  - Identity Controls
tags: []
---

# Identity Controls

## Identity Provider (IdP)
Controls identities (authentication as a service) 
- useful for cloud 
- a list of entities 
- commonly used for SSO apps 
- various standars 

## Attributes 
Characteristics used to identify 
- Personal 
    - name 
    - email 
    - phone 
- multiple can be used to identify 

## Certificates 
Digital certs assigned to people or devices to identify them 
- uses PKI 
    - needs a certificate authority CA 
        - CA signs certs 
- Tokens or cards or usb tokens can store certificates 

## SSH keys 
Secure shell (SSH) identification 
- uses public and private keys to authenticate 
- key management is critical 
- managers exist to help with this 
- to create a keypair run 
    ```bash 
    ssh-keygen
    ```

- to copy pair to ssh server run 
    ```bash 
    ssh-copy-id user@host
    ```
- then you can ssh into the server 
    ```bash 
    ssh user@host
    ```
- no password needed 

