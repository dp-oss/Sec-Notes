---
id: 1711654258-EIBL
aliases:
  - Forensic Tools
tags:
  - Tools
---

# Forensic Tools

## `dd`
Create a bit by bit copy of a drive 
- if specifies input and of specifies output 
- example to create a disk image use: 
    - `dd if =/dev/sda of=/tmp/sda-image.img`
- example to restore from a disk image use: 
    - `dd if =/tmp/sda-image.img of=/dev/sda`


*the following section on dd may not be covered in the exam objectives but it is one of my favorite utils so I want to share* 

- can be used with /dev/zero or /dev/urandom to fill a drive with zeroes or pseduo random data 
    - this is useful for clearing data from a drive, multiple passes may even be considered purging (see [[Secure Data Destruction]] for more information on these terms) 
    - example for clearing a drive by filling with pseduo random data: 
        - `dd if=/dev/urandom of=/dev/sda` 
        - the command will stop when the drive is full of data 
- the option `status=progress` is useful to add and will provide information about how far along the command is 


## `memdump` 
Copy information from system memory to stdout 
- exact copy of what's in memory 
- third party tools can be used to parse this data 

## WinHex 
hexadecimal editor for WindowsOS 
- can edit disks, ram and files 
- can clone disks 
- can securely wipe disks 
- many forensic tools 

## FTK imager 
forensic drive imaging tool made by AccessData for the Windows operating system 
-  can support different filesystems 
    - including some with full disk encryption 
        - still need the keys 
- can output in many different formats 


## Autopsy 
Preform digital forensics on a storage device or image file
- can extract many different data types
- can sort extracted data 

## Data Sanitization 
Completely remove data 
- also make it so that data could not be recovered later on 
- clean hard drives for re use or sale 
- see [[Secure Data Destruction#sanitization]] for more details 
