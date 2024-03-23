**File backups**: 
- files have an archive bit that is set on when it is modified allowing you to know whether or not to back it up 
- Full backups: 
	- Everything you have 
	- High backup time / low restore time
- Incremental:  ^b1f8f4
	- backs up all files changed since last backup
	- Restoring from incremental backups requires both the full and all of the incremental backups afterwards 
	- low backup time/high restore time
- Differential: ^b1c3d9
	-  Backs up all files that have been changed since the last *full* backup 
		- that means each time after a full you run a differential it will be larger 
	- Restoring from differential requires the most recent differential as well as the original full backup
	- Moderate backup time/moderate restore time
- 

**Backup Media**
- **Magnetic Tape**
	- easily shipped and stored 
	- cartridges 
- **Disk**
	- Faster than mag tape
	- cheaper recently
- **Image/Copy**
	- Just an exact replica of a system
	- useful for restorage

**NAS (network attached storage)**: 
- Large array of storage connected to your networks
- File-level Access
	- changing a portion of a file means needing to rewrite the entire file

**SAN (storage area network): 
- Acts like a local storage device 
- Very efficient to read and write 
- Block level access
	- you can change a portion of a file on the disk and only rewrite that one portion

**Cloud based Backups**: 
- backing up local files to a remote device in the cloud
- limited by bandwidth
- **Image**: 
	- Backing up the entire computer as a complete duplicate to the cloud 
	- allows for exact restoration
**Locations**:
- **Offline**: 
	- backed up locally 
	- fast and secure 
	- must be protected/maintained
	- can only be accessed locally 
	- can require offsite storage for disaster recovery 
- **Online**: 
	- backed up over network somewhere else 
	- needs to be encrypted 
	- 