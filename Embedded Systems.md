Hardware designed for a specific function 
- possibly operating as a part of a bigger system

- built with only the singular task in mind 

**SoC (System on a chip)**: Multiple components running on a singular computer chip
- very common with embedded
- ex. raspberry pi 
- small in form factor 
- usually lower power memory 
- can contain Cache / flash memory or both
- difficult to upgrade hardware 
- limited off-the-shelf security options 


**Field-programmable gate array (FPGA)**: 
- Integrated circuit that can be configured after manufacturing 
	- an array of logic blocks 
	- programmed in the field 
- Problems dont require hardware replacements because they're reprogramable 

### SCADA

^f30610

Supervisory Control and Data Acquisition System 
- Large-scale, multi-site **Industrial Control System (ICS)**

Computers used to manage equipment 

Distributed control over systems 
- real time data 
- control 
Segments physical equipment from the network 


### **IoT (Internet of things)**: 

^ade99f

Smart devices and sensors which connect to the internet 
- light switches 
- thermostat 
- health monitors 
- video doorbells 
**OFTEN HAVE WEAK SECURITY!!** 

**Specialized devices**: 
Medical Devices 
- often use older OSs since they can't be upgraded 
Vehicles 
- Internal electronic controls in most modern vehicles 
Aircraft
- Importang to avoid DoS
- Outage would be baddd
Smart Meters: 
- Monitor utilities in many homes 

**VoIP Voice over Internet Protocol**: 
- Alternative to POTS plain old telephone service 
- complete embedded system
- every VOIP device is a computer so it is vulnerable to some degree 

**HVAC**: 
Heating ventilaiton and Air Conditioning
- A complex science 
- often combined with fire safety systems 
- Can be managed from computers so it can be vulnerable 
- Not often built with security in mind 

**Drones**: 
Flying Vehicle ^30bd1b
 - Can be autonomous 
 - May be controlled from the ground 
 - US requires federal liscenses 
 - Contain security and fail safe features 


**Printers, scanners and fax**: 
Sometimes referred to as MFD or multi function devices 
- getting more complex
- may store images of scanned documents locally 




 **RTOS (Real-Time Operating System)**:

An operating system with a deterministic processing schedule
- no waiting for multiple proccesses 
- industrial, automotive and military applications

Can be sensitive to security issues 

**Surveillance Systems**: 
- Monitor audio and video
	- contain embeded systems in cams/mics
- Must be kept secure only authorized access
- May be physically difficult to change out hardware 


[[Embedded Systems Communication]]


[[Embedded Systems Constraints]]

