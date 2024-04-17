---
id: 1712190705-UBUW
aliases:
  - Managing Evidence
tags:
  - Forensics
---

# Managing Evidence

## Integrity 
Ensuring the data is unchanged (CIA Triad) 
- hashing 
    - cryptographically verify integrity 
    - digital footprint 
    - see [[Hashing and Digital Signatures|hashing and Digital Signatures]]
- Checksums 
    - relatively simple integrity check
    - not designed to replace a hash
    - protects against changes in transit
- Provenance
    - documentation of authenticity 
    - chain of custody for data handling 
    - uses blockchain technology (see [[Blockchain|blockchain]])

## Preservation 
Handling and protecting the data 
- isolate and protect 
- create a copy or an image 
- analyze later without alterations 
- Live collection is important
    - data may be encrypted if the system is powered down 
- best practices will ensure admissibility in court 

##  E-discovery
Electronic discovery in the legal process 
- gathering of data required by legal process
- works in conjunction with digital forensics 

## Data recovery 
Extracting missing data without affecting integrity 
- process can vary 
    - deleted
    - hidden
    - hardware/software corruption
    - physical damage 

## Non-repudiation
Proof of integrity as well as the origin of the data 
- data is unchanged and comes from the sender 
- authenticity is genuine with high confidence 
- **Message Authentication Code (MAC)**
    - only the two parties who are communicating back and forth can verify Non-repudiation
- Digital Signatures
    - Non-repudiation can be verified publicly 

## Strategic Intelligence/counterintelligence
- Focuses on key threat activity for a domain 
- can come from internal threat reports, third party, or open source 
- determine threat landscape baesed on trends
### Strategic counterintelligence (CI) 
Prevent hostile intelligence operations
- then begin your own intelligence on the threat
