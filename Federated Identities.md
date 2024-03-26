---
id: 1711409970-TDQO
aliases:
  - Federated Identities
tags:
  - Authentication
---

# Federated Identities
Federation is used to provide access using credentials for a different service
- can provide SSO and more 
- Third-parties establish a federated network allowing Authentication between two organizations 
- think "login with google?" 


## Security Assertion Markup Language (SAML) 
A standard for Authentication and Authorization 
- allows Third-parties to gain access
- not designed for mobile 
- The flow:
    1. User requests access to service 
    2. Service returns SAML request which redirects to outside Auth Server
    3. User logs in to outside Auth Server 
    4. Authentication server returns a SAML token
    5. User presents SAML token to the service and can access it 

## OAuth 
An Authorization framework 
- determines what resourcse a user can access 
- created by Twitter, google and other tech giants
- Not used to authenticate
    - OpenID is used for authentication
    - OAuth just provides Authorization
- popular on the modern web
    - think "Runescape would like to access your Google Account"


