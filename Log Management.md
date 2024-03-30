---
id: 1711756144-XWEM
aliases:
  - Log Management
tags: []
---

# Log Management

## Syslog 
Standard for sending logs  
- Usually sent to a centeral loggin server 
    - Integrated into [[SIEM]]
- Each log entry is labeled: 
    - Facility Code(Program of origin)
    - and severity level
- Syslog daemon options: 
    - Rsyslog - "Rocket-fast System for log processing" 
    - Syslog-ng - Popular syslog daemon with additional filtering options
    - NXLog - Collection from different log types

## Journalctl 
A method for querying binary logs in linux 
- Logs are stored in binary 
    - optimized for storage
    - not human readable
- Journalctl let's us read them 

## Bandwith Monitors 
Percentage of network use over time 
- can be collected in many way
    - SNMP
    - NetFlow
    - SFlow
    - IPFIX
- helps identify fundamental issues 
## Metadata 
Data describing a data source 
- Email
    - Headers 
    - sending servers 
    - destination address 
- Mobile
    - Type of phone 
    - GPS location
- Web
    - OS
    - Browsertype 
    - IP address 
- Files 
    - Name
    - Address
    - Phone number
    - title 

## NetFlow 
Standard for gathering network statistics 
- well established 
    - plays well with many vendors 
- Probes 
    - watches network communications 
- Collector 
    - receives the data from probes and aggrigates 
- Usually a seperate reporting app Integrated with the collectors 

## IPFIX IP flow information Export
Newer netflow based standard 
- flexible support for data 
- newer than netflow v9
-  templated are used to describe data to be collected 

## sFlow (Sampled Flow) 
Only a portion of the network traffic used to gather statistics 
- requires less resources 
- Usually embedded in infrastructure
    - swithces
    - routers 
    - Sampling occurs usually in hardware/ASICs
- Relatively Accurate
- useful for high traffic applications and video streaming

## Protocol Analyzer Output 
Breakdowns of all packets coming accross the network
- identify unkown traffic 
- filter packets to find specific ones 
- security controls 
- plain language description of application data 
- see: [[1711653130-CXFS|Packet Tools]]

