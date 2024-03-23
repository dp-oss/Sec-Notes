 Secure Sockets Layer / Transport Layer Security Inspection 
- Examining the encrypted information being sent to your computer 
- SSL Uses a list of certificate authorities CAs that your browser trusts 
- browser checks that website has signed certificate from a CA on the list then decrypts the data 


To inspect we create an internal CA installed on all local computers which can allow them to communicate through a firewall/proxy we control which decrypts the SSL and re-encrypts before sending it back to our users 

this allows us to decrypt information before its returned to our users 
to prevent intrusions/malware from breaching the firewall because its encrypted in transit
