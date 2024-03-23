The boot process is a high value target on systems 
- it allows attackers to maintain control on the device and keep it compromised 

Protecting the boot process is vital 
Security is based on trust 

Trust starts at a hardware level

- **Hardware Security Module (HSM)**
- These are difficult to change or avoid for attackers 

 **Trusted Platform Module (TPM)**: 
 Hardware chip that helps with encryption functions 
 - can be installed separately or integrated into the motherboard
 - processes RNG, and key generation 
 - Contains persistent memory that can store a specified key without changing it
 - Has versatile memory to store keys 
 - Password protected
	 - has brute force protection too 

**UEFI BIOS Secure Boot**: 
A part of the specification of UEFI ensuring you're booting into the correct bios/os
- BIOS has the manufacturers public key to verify all updates are valid 
- Secure boot verifies the bootloader is signed with trusted certificate to ensure that the correct OS is being booted 

**Trusted Boot**: 
When the bootloader verifies the certificate of the operating systems kernel before loading them 
- next the kernel verifies other components of startup such as drivers 
- next **ELAM Early Launch anti Malware** verifies signatures of other drivers 

**Measured Boot**:
Automated way to determine that a computer doesn't contain malware after boot 
- UEFI stores hash of all the firmware in the **TPM** and checks against all the hashes to ensure nothing has changed 
- Remote attestation sends the systems hashes to a Attestation server which receives the hashes after **TPM** cryptographically signs them for verification

