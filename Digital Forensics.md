---
id: 1711766407-SUHF
aliases:
  - Digital Forensics
tags: []
---

# Digital Forensics
Collecting and protecting information relating to a security event
- See: [[Forensics Data Acquisition]] for more on collecting data

- RFC 3227 Guidlines for Evidence Collection and Archiving 
    - set of best practices 
    1. Acquisition
    2. Analysis 
    3. Reporting 

## Legal Hold 
A legal technique to preserve relevant information 
- initiated by legal council 
- A hold notification instructs custodians to hold data
- Seperate repository for Electronically Stored Information (ESI) 

## Video 
A moving record of the event
- capture screen information 
- security camera footage 
- Video must be archived to reference later

## Admissibility 
Wether or not data can be used in a court of law
- Not all data can be used legally 
- Legal authorization can prevent what can be gathered 
- Laboratories
    - proper science principles need to be used in analysis 
- Technical and Academic Qualifications of experts may be questioned in court 

## Chain of Custody 
Documentation of control over evidence
- Document everyone who contacts the evidence 
- everything is labeled and catalog 
- hashes can be used for this 

## Recording Time Offsets 
Information about time of access to a file
- affected by timezone
- Filesystems handle this differently 
    - FAT is stored in local time
    - NTFS is stored in GMT 
- Record the time offsets from the OS itself 
    - can be checked in windows registry 

## Event logs
System logs can be crucial
- Export and store for future reference 
- can be parsed or filtered 
- Log storage: 
    - linux: /var/log
    - Windows: Event Viewer 
- see: [[1711744251-KHHL|log Files]] and [[1711756144-XWEM|log Management]] for more 

## Interviews 
Interviewing Users can provide valuable information
- should be done quickly 
- not all witnesses are accurate 
- need to be documened 

## Reports
Document forensic finding
- summary: high level overview
- detailed explanation of data Acquisition 
    - step by step methods 
- The findings: analysis of data
- Conclusion what can be drawn from the analysis


