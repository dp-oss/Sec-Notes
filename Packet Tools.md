---
id: 1711653130-CXFS
aliases:
  - Packet Tools
tags:
  - Tools
---

# Packet Tools

Tools for packet inspection and analysis 

## Wireshark 
Graphical packet analyzer 
- can view and breakdown network traffic 
- Gathers frames on the network or over the air 
- useful to find patterns in network traffic 
    - identify unknown traffic 
    - or verify that packet filtering and other controls are functioning 
- can decode packets to look at application specific traffic 

## `tcpdump` 
Capture packets from the command line 
- will print the packets to stdout 

## tcpreplay
Can edit and replay packet captures 
- good to test security devices like IPS and NGFW 
- can test and tune IP flow/ NetFlow devices 
    - by sending hundreds of thousands of traffic flows per second 
- can stress test network equipment 
