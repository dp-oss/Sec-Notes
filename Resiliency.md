**Non-persistence**: 
The clouds always changing 
- machines built/torn down frequently

Snapshots allow us to capture current config and data
- this allows you to revert to a known state to fall back 

**High availability**: 
- Redundant doesn't always mean available
- **HA (high availability)**: 
	- Always on and available 
	- Usually means higher cost 

#### **Order of restoration**: 
The order in which you need to restore functions of an application to ensure it functions the same as before 
- **Backup Specific**: 
	-  different for [[Backup Types#^b1f8f4|Incremental]] and [[Backup Types#^b1c3d9|Differential]]


#### Diversity: 
Prevents a single point of failure

- Using different technologies can result in one vulnerability not taking all of your tech down 

- Using different vendors can provide more options for support

- Cryptographic Diversity can prevent failure if one is cracked 

- Diverse Security controls: (can be considered defense in depth)
	- admin
	- physical
	- technical 
	- combine multiple 

