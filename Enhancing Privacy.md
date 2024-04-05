---
id: 1712346516-RHCY
aliases:
  - Enhancing Privacy
tags: []
---

# Enhancing Privacy

## Tokenization
Replacing Sensitive data with a non-sensitive place holder 
- this is common with credit card processing
    - if an attacker captures card info they can't use it elsewhere
    - temporary token is used during payment
        - links to card number but isn't the card nuber
- is not hashing 
- is not encryption
- no mathmatical relation between data with token
- no cpu overhead

## Data minimization
Collect and retain only the data that is necessary
- Included in many regulations
    - HIPAA
    - GDPR 
- do you really need my phone number and adress? 
- internal data use sshould be limited
    - only access data required for completing a task

## Data masking 
Obfuscation of data
- hide some of the original 
- Protects PII 
- Finacnial Details
- data can still exist in storage 
    - but is hidden from view
- like only showing the last 4 of card number on receipt
- Many techniques
    - shifting
    - shuffling
    - masking with blank characters
    - encrypting 

## Anonymization
Make it impossible to identify individual data from a dataset
- allows data use without privacy concers
- many techniques
    - hashing
    - masking
    - etc
- Convert detailed data by removing sensitive data points and only keeping the metrics you need
- impossible to convert back to original data
- no way to associate with user

## Pseudo-anonymization
Pseudonymization
- replace personal information with pseudonyms
- often used to main statistical relationships
- May be reversed 
    - hide data for daily use
    - convert back for other processes
- can be done through random name replacement
- can use consistent replacements
    - the same name corresponds to the same pseduonom


