---
id: 1711566635-VEGU
aliases:
  - Reconnaissance Tools
tags:
  - Reconnaissance
---

# Reconnaissance Tools
Tools for conducting [[Reconnaissance]]  
## traceroute
Determine the route a packet takes to a destination
- `tracert` on windows
- `traceroute` on linux 
- uses ICMP time to live exceeded (TTL) error message to do this 
    - TTL=1 is the first router, TTL=2 is the second router etc.
    - we take advantage of the fact that when a TTL is exceeded routers will drop the packet, so we increase the TTL with each hop to determine each router we go through on the way
- not all devices will reply with ICMP ttl messages 
- Windows uses ICMP echo requests (same as ping) 
    - you will get ICMP ttl messages for hops 
    - and an echo from the final destination 
    - ICMP is commonly filtered 
- you can specify the protocol used to suit your needs 

## nslookup and dig 
Look up DNS information
- `nslookup` 
    - both windows and and unix 
    - deprecated 
    - looks up names and IP
- `dig` 
    - (Domain information Groper) 
    - can be installed on windows 
    - more info than `nslookup` 


## ipconfig and ifconfig 
provides information about a computer's network adapters 
- `ipconfig` in windows
- `ifconfig` on linux 

## ping 
Test reachability by sending ICMP packets
- Internet control message protocol (ICMP) 
- `ping` tests if you can reach the ip of a device 
- `pathping` on windows combines `ping` and `tracert` 
    - will ping the address and provide info about hops along the way

## netstat 
Network Statistics 
- `netstat -a` 
    - shows all active connections to your machine 
- `netstat -b`
    - on windows: shows the windows binary along with the connections
- `netstat -n` 
    - do not resolve the names of IPs

## Address Resolution Protocol 
Determine the MAC address based on local IP
- to do this we use the `arp -a` command 

## Route 
View the devices routing table 
- `route print` in windows
- `netstat -r` in linux

## `curl` 
Client URL (Uniform Resource Locator) 
- request raw data from a website 
- can get webpage, FTP, database, email etc.
- `curl google.com` would send a GET request to google.com and display it's contents in the terminal 

## IP scanning 
Search a network for active devices 
- Scanners can use: 
    - ARP for local
    - ICMP (ping) 
    - TCP ACK 
    - ICMP timestamp requests 

### `hping3` or hping
More specialized ping command that can be used to sent many request types 
- you can ping devices using ICMP,TCP,UDP and much more
- example: `hping3 --destport 80 10.1.10.1` 
- be careful not to accidentally flood the network and DoS 

### Nmap
`nmap` is an advanced network scanner 
- can find devices on network
- scan ports and identify whats open
- Find what OS a device is running
- find what service and version is running on device 
- has scripting 

### `scanless` 
Run port scans from a different host 
- a proxy for port scanning 
- can use many different services and hide your own ip 
- example: `scanless -t example.org -s spiderip` 
    - scans example.org using the spiderip proxy

## `theHarvester`
A tool for gathering [[OSINT - Open Source Intelligence]]
- scrapes information from search engines 
- can brute force DNS 
    - vpn, chat, mail, partner 
- example `theHarvester -d example.com -l 100 -b bing` 
    - this willl find everything related to that domain on bing (100 results) 

## sn1per 
Combines several recon tools into one 
- dnsenum, metasploit, nmap, theHarvester, etc
- can scan both intrusively or nonintrusively 
- can cause DoS so be careful
- example: `sniper -t example.com -m web` 
    - will find information about webservices on that domain


## `dnsenum` 
Enumerate dns information 
- many services and hosts may not be listed in DNS servers 
- for example in google 
- example `dnsenum example.com` 
    - will search dns servers and then it will bruteforce:  
        - changing  the name it's looking up to find other subdomains

## Nessus 
Vulnerability scanner 
- industry leading vuln scanner 
- extensive reporting 
- will find and categorize vulnerabilities on the target 
- can even provide solutions to issues 
- can scan many different IPs or range of IPs and create a Vulnerability Database

## Cuckoo 
A sandbox for malware 
- allows you to test a file in a virtualized enviornment
- can track and trace API calls, and network traffic
- good to determine if an executable is safe 

