**Directory Services**: List of all of an organization's users and passwords in a single DB along with permissions

- all authentication requests use the same DB 
  
  **Federation**: Providing access to your network based on the verification done by a third party
- IE sign in with Google 
  
  **Attestation**: Tests that force users to be on hardware provided by an organization not on third party hardware
- means only trusted devices can join the internal network
- harder with scale needs
  
  
  **SMS authentication**: A second factor containing a code is sent to a users cell phone to prove they are who they say they are while logging in
- vulnerable to sim swapping
- SMS can also be intercepted 
  
  **Push Notification Auth**: Server pushes a notification to users mobile device to verify they are who they say they are
- push notifcations can be a security risk but are more secure than SMS if the right app is used
  
  **Authentication Apps**: Pseudo random tokens are generated on a seperate app and used at login to prove you are who you say you are
  
  
  **TOTP: Time based one time password**: A secret key is used along with the time of day using an algorithm to make unique codes to verify you are who you are 
  
  
  **HOTP HMAC-based One-Time password**: Single use passwords are generated for login which each can only be used once 
  
  **Phone Call**: User is receives an automated call which reads off the code for login
- similar vulnerabilities to SMS auth
- sim swapping vulnerability
  
  **Static Codes**: Authentication values don't change and a user just remembers
- example include:
	- Passwords
	- ATM PIN
	  
	  **Smart Card**: Card with integrated circuit allows you to verify who controls the card
- like a credit or debit card
- requires physical access to gain digital access
- Multiple risks so it should be used with other authentication factors 
  
  **[[Biometric Authentication]]**: Using a physical trait to prove identity

 
 **[[Multi-Factor Authentication]]**: Authentication using multiple unique methods to confirm your identity