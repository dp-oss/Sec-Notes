---
id: Wireless Cryptography
aliases: []
tags: []
---


- users need to be authenticated before connecting to a wireless network 
- all data transmitted wirelessly needs to be encrypted 
- verify the integrity of information

Types include: 
- wpa2
    - wifi protected access II 
    - CCMP block Cipher mode 
        - uses AES to encrypt
        - CBC-MAc to check integrity
- wpa3
    - wifi protected access III
    - uses GCMP block Cipher mode
    - Stronger than wpa2
    - uses AES to encrypt
    - GMAC used to check integrity


- WPA2 suffers from PSK brute force vulnerability
    - attacker can listen to the 4way handshake and capture the hash 
    - using the hash they can determine the PSK or pre shared key with brute force

- Due to this wpa3 changed the PSK auth process
    - creates a shared key without sending accross network 
    - this means perfect forward secrecy
    - no fourway handshake to catch the hash and brute force 
- Accomplished through **Simultaneous authentication of Equals (SAE)** 
    - simmilar to diffie helman


[[Wireless Authentication Methods]]

