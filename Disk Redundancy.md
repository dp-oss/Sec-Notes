~  Storing multiple copies or information about the data in order to rebuild it if some is lost 
	  like in a disk failure 

- **Raid**: Redundant Array of Independent Disks 
	- multiple drives can store t he same data 
	- having multiple drives allows for better redundancy 
	- RAID 0: Striping without parity
		- High preforming 
		- losing one drive you lose the data 
		- not redundant 
	- RAID 1: Mirroring
		- Duplicates data 
		- is redundant so its fault resistant
		- requires twice the disk
	- RAID 5: Striping with parity
		- 1 drive used for parity information
		- 1 extra drive needed
		- losing any drive and the data can be rebuilt using parity information 
		- 
