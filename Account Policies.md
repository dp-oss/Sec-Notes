---
id: 1711406141-JWKA
aliases:
  - Account Policies
tags:
  - Accounts
---

# Account Policies
- Policies can control access to accounts
- can control the authentication process 

## Audits
Periodic audits are important to ensure Policies are being followed and are effective 
- log files can be useful 
Premission Auditing 
- does everyone have correct premissions 
- schedule recertification of premissions 
- [[1711405790-WPES|Principle of Least Privilege]]
Usage Auditing
- are people using what they're supposed to 

## Password Complexity/Length
Strong passwords have sufficient entropy to prevent brute force 
- mix upper case, lowercase, and special chars
- no dictionary words 
- at least 8 characters is best 
- Password history can prevent password reuse

## Account lockout/disablement
After certain conditions are met accounts are locked and prevented from authentication 
- usually too many incorrect login attempts
- important for people leaving the company 
    - dont just delete the account *you may need this data* 
- important for service accounts [[1711405265-NAHM#account-types#service-account|Account Types ❯ Service account]]

## Location based policy 
- can use IP or IP subnet
- can use geolocation see: [[Mobile Device Enforcement#geotagging--gps-tagging]]
- location based rules can block authentication when someone is in another country 
    - "we don't have an office in russia!" 
- can combine with time based policy 
    - no body needs to be working in the lab at 3am EST 
