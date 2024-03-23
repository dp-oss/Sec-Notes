We need to ensure people connecting to a network are authorized to use the network 

Credentials: 
- PSK preshared key (the wifi Password)
- Centralized authentication (802.1X)
    - use normal credentials such as user and pass to authenticate to domain
    - authentication done on connection 

Security modes: 
- Personal connections: PSK 
    - WPA3-Personal / WPA3-PSK: everyone uses the same password but each person has their own session key
- Open System: Anyone can connect 
- WPA3-Enterprise / WPA3-802.1X
    - all users are authentication using a centralized authentication server 
- Captive portal: method of authentication where new users are re-directed to a portal to login 
    - common in coffee shops/ cafes
    - can log you out of session after specified period

WPS: wifi protected setup
- may be a good idea to disable 
    - has a flawed design which can be a security risk 
- offers easy setups
- allows different means of connection
    -  button on accesspoint 
    -  pin code 
    -  NFC 
    -  

[[Wireless Authentication Protocols]] 