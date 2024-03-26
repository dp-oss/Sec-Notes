---
id: Mobile Device Management
aliases: []
tags:
  - Mobile-Devices
---

## Mobile Device Management (MDM)

Manage company and user owned devices 
- many companies have a BYOD bring your own Device ^112b2d
- Policies on applications and data
- Can control the entire device or merely a partition
- can set rules for access like pin code or screen lock 


Application Management: 
- not all apps are secure 
- Use an allow list in the MDM to determine what apps can be installed 
- Time/effort: 
    - new apps need to be vetted before adding to the list

Content Management: 
Mobile Content Management (MCM) 
- Set policies on where files can be stored 
- who may view 
- protect data from outsiders 
- can include [[Data Loss Prevention (DLP)|data Loss Prevention (DLP)]]
- ensure encryption of sensitive data 
- managed from MDM


Remote Wipe: 
Remove all data from device when lost 
- managed through the MDM
- uses the mobile network to wipe over the internet 
- always keep backups 


Geolocation: 
Can track users within feet using [[Mobile Networks|GPS]]
- can be disabled but may limit function of phone 
- can be managed through MDM 
Geofencing: 
Enable or disable certain features dependent on location
- examples include: 
    - disable camera in the office 
    - disable login to device outside of the country

Screen Lock: 
- All mobile devices should be locked when not in use 
- MDM can be configured to erase device after too many failed login attemps 
- MDM can define a lockout policy that locks users out 


Push Notifications: 
Informations automatically sent to the device "pushed" 
- MDM can control which Notifications will appear 
- sensitive data can appear on lock screen important to disable this sometimes 


Passwords and PINs 
- MDM has full control 
    - can reset passwords if forgotten 
- Biometrics can be used to unlock device 
    - useful in some settings 
    - forbidden in others 
    - see: [[Biometric Authentication]]


**Context aware authentication**: 
Combines multiple factors together to determien whos trying to authenticate to a device 
- IP 
- GPS 

**Containerization**: 
Create seperate areas on a mobile device to segment user data from company data
- important for BYOD 
- important during offboarding
    - remove company info but not personal data 


**Full device encryption (FDE)**: 
Encrypting the entire mobile device 
- can be controlled by MDM 
- choose how strong the encryption is
    - stronger encryption will take up more battery 
- backup decryption keys 
    - often backed up to the MDM 

[[Mobile Device Security]]
[[Mobile Device Enforcement]]
