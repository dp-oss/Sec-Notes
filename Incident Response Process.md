---
id: 1711734755-BVCS
aliases:
  - Incident Response Process
tags:
  - Incident-Response
---

# Incident Response Process

## Security Incident 
An event that effects the security of your organization
- user infected with malware
- ddos 
- leak of confidential information 
- etc. 


## Roles and Responsibilities
### Incident Response Team 
Specialized Group that deals with incidents 
- it managemenet 
- compliance officers 
- technical staff 
- User community 

## NIST SP800-61: Computer Security Incident Handling Guide 
Outlines the lifecycle for handling security incidents 
https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf

- lifecycle: 
    - Preperation 
    - Detection and Analysis
    - Containment, eradication and recovery
    - Post incident activity


## Preperation 
What you should have prepared before an incident even occurs 
- Communication Methods 
    - who and how to contact
- Hardware and software tool for managing incidents 
    - forensic software 
    - cameras 
- Incident Analysis Resources 
    - documentaion
    - network diagrams 
- Mitigation Software 
    - clean OS images 
    - recovery 
- Policies needed for handling incidents

## Detection
Detection poses a significan challenge 
- extensive knowledge is important
- alot of noise and false positives

### Incident Precursors 
Warning signs that an incident may occur in the future
- exploit announcement
- Server Logs
- Direct threaats 

### Incident Indicators 
Signs an attack is underway 
- IPS alerts
    - see:[[Intrusion Prevention]] 
- malware or antivirus alterts 
- Host-based monitor detects configuration changes
    - see: [[Endpoint Protection]] 


## Isolation and Containment
- not a good idea to let things just happen
- Sandboxes
    - isolated operation system
    - run and analyze malware 
    - some malware can detect sandbox and act differently 
    - see [[Sandboxing]]
- some malware can recognize when connectivity is lost and to avoid investigation after it's isolated

## Recovery 
Getting systems back to normal 
- First Eradicate the malware
    - disable breached accoutns 
    - fix vulnerabilities 
- Recover the system
    - restore backups 
    - build from scratch
    - replace compromised files 
    - tighten down perimeter 

### Reconstitution 
- recovery occurs in phases for large systems
- recovery can take months 
- Plans need to be efficient
    - start with quick and high value changes 
        - patches, firewall Policies 
    - later move on to bigger infrastructure changes 

## Lessons Learned 
Learn and improve from security incidents 
- post incident meetings 
- this should occur shortly after recovery to learn the most 
- Questions:
    - What happened
    - did plans work
    - what would you do different 
    - what indicators would show this incident


