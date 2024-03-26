# Mobile Device Enforcement


## Appstores 
- Third Party Appstores can contain insecure apps 
- not all apps are appropriate for work enviornment

## Rooting/Jailbreaking
Gaining root level access to a mobile device 
- usually using custom firmware 
- can allow you to circumvent access controls 
- Makes MDM pointless can go behind controls 

## Carrier Unlocking 
Unlocking device from use with it's original cellular network provider 
- may be illegal in some countries 
- carrier may allow after contract is over 
- carrier subsidizes cost of device and thus wants to force you to use the network 
- could potentially circumvent MDM 
- Preventing may not be possible on a BYOD 

## Firmware OTA Updates 
Updates to device provided automatically over the network 
- Security patches 
- OS updates 
- MDM can control whether the updates are pushed down or not 
    - test before the updates 


## Camera use 
The use of the camera may not always be appropriate 
- Can be controlled by the MDM 
- can be based on geofencing 


## SMS/MMS 
Short or Multi Media message service 
- can be the source of a phishing attack known as SPIM spam over instant messenger 
- MDM can enable or disable 


## External Media 
Data stored on portable devices that can be moved from one device to another 
- flash drive 
- sd card 
- external drive 
- mdm can disable the use of these to prevent data loss 


## USB OTG 
USB on the go 
- connect two mobile devices directly over USB - Common on android 
- no external storage needed 

## Recording / Microphone 
- can be a legal liability 
    - each state has different laws 
        - third or first party state 
- can be disabled through MDM 
    - geofencing 

## Geotagging / GPS tagging 
Storing location data as metadata along with a file 
- location where a picture is taken 
- every document could contain geotagged info 
- this could be security and privacy risk 

## WiFi Direct / ad hoc 
Connecting two devices directly over WiFi 
- no access point needed 
- common for IOT devices 
- common vulnerablity to circumvent the security normally enabled on an AP 

## Hotspot / tethering 
Turning a mobile device into a wireless access point 
- extend cellular network to other devices 
- may require additional cost 
- can provide inadvertent access to internal networks 

## Payment 
NFC can be used to transfer small ammounts of data including purchases 
- apple / google pay 
- typically requires authentication 
