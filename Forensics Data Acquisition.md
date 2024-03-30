---
id: 1711767259-KKOB
aliases:
  - Forensics Data Acquisition
tags: []
---

# Forensics Data Acquisition
Aquiring data for forensic investigations 

( see [[Forensic Tools]] for more specifc details on data collection tools ) 

## Order of Volatility 
Some data persists for longer than others 
- In order of Volatility: 
    - CPU registers and cache is very volatile
    - Router table, ARP cache, Process table, Kernel Stats, Memory 
    - Temp file systems 
    - disk
    - Remote logging data 
    - physical configuration and network topology 
    - archival media 

## Disk 
- Coppy everything on a storage drive 
- prepare drive to be imaged
    - power system down to prevent changes
    - remove storage device 
- Connect to imaging device 
    - usualyy write-protected
- Forensic Clone: 
    - Bit for bit coy 
    - preserves all data (even deleted) 
## Random Access Memory (RAM) 
Can be a difficult targe to capture 
- constantly changing 
- Create a memory dump 
- can contain important data
    - browser/command history 
    - clipboard
    - encryption keys

## Swap/pagefile
Used by different OSs that is usually used to swap information out of RAM when out of memory 
- can contain portions of applications 
- contains similar data to memory dump 
## Operating System
Alot of information can come from OS files and data
- core files and libraries can be compared to known good files 
- usually captured in drive image
- logged in users
- open ports
- currently running processes
- attached devices 

## Mobile devices 
- capture methods exist to make forensic backups 
- transfer image over USB
- data: 
    - phone calls 
    - contacts 
    - texts
    - images 
    - apps 
    - etc. 

## Firmware 
Extract the firmware of a device to help understand exploits 
- rootkits and exploited hardware
- can show real-time data being sent to and from device 
- platform specific 
    - certain product/models have different firmware

## Snapshots 
A point in tmie system image
- often used with VMs 
- can show incremental updates 
- often done between updates 
- contains all files and information about a VM 

## Cache 
Temporary storage used to increase preformance 
- many types: 
    - CPU 
    - Disk 
    - Internet browser 
- can contain specialized data 
- some data may never be used 
- browser caches are often long lived 
    - can show URLS 
    - and page components 

## Networks 
- network connections
- packet captures
- inbount and outbound sessions 
- Capture of raw network data and storage is common in larger networks 
- Firewalls and IPS can provide this data 

## Artifacts
Digital items left behind in storage
- sometimes just a trace 
- Locations: 
    - logs
    - flash memory 
    - prefetch cahce
    - recycle bin 
    - browser bookmarks and logins 
