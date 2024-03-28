---
id: 1711651150-QKBR
aliases:
  - File Manipulation Tools
tags:
  - Tools
---

# File Manipulation Tools

## `cat` 
Concatenate
- prints the contents of a file to stdout
- output can be redirected 
- `cat file1.txt file2.txt` prints the contents of both files
- `cat file1.txt file2.txt > both.txt` outputs the contents of both files into both.txt 


## `head` 
Prints the first contents of a file to stdout 
- `-n` specifies number of lines
- `head -n 5 file.txt` prints the first five lines of file.txt

## `tail` 
Prints the last part of a file to stdout 
- `-n` specifies number of lines
- `tail -n 5 file.txt` prints the last five lines of file.txt

## `grep` 
Find a string within a file/files 
- will return the lines where the string appears to stdout 
- usage: `grep PATTERN [FILE]` 

## `chmod` 
Change mode of a file system object
- read, write, and execute r,w,and x respectively 
- can use octal notation
    - Premissions are set using a base 8 system
    - 0 = none
    - 1 = execute 
    - 2 = write only
    - 4 = read only
    - 1 + 2 + 4 = 7 = all premissions
    - These numbers can be combined to create any set of premissions 
- can be set for owner(u), group(g), others(o), or all(a) 
    - we set 3 numbers in octal ex. 744 
        - 1. User
        - 2. Group 
        - 3. All 
- example usage: `chmod 744 file.txt` 
    - full premissions for the user/owner of the file
    - read only for the group 
    - read only for everyone else 
- can also use letters to denote premissions 
    - example `chmod a-w file.txt` 
        - all other users no writting to file.txt
    - example `chmod u+x file.sh` 
        - owner of file.sh can execute 

## `logger` 
Add entries to sytem log
- usually syslog 
- ex. `logger "This info will be in syslog"` 
    - will print this information into syslog
- helpful to add logging into custom scripts 
    - or log an important system event 

