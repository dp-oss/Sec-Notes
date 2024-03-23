[[Secure Coding Techniques| Secure Coding]] is a balance of time and quality 

- the QA team will test the code to find vulnerabilities and bugs 


Whenever a user inputs data you must practice [[Secure Coding Techniques#^bb9aa0|Input validation]] and [[Secure Coding Techniques#^758d39|normalization]]
- attackers can use fuzzer tools to input lots of random data to determine what inputs produce what outputs 

**Fuzzing**:
Inputting Random data into an application to find unexpected behaviors 
- Dynamic analysis, or fault injection, robustness testing etc. 
- automated
- time intensive 
- resource intensive
- many use high-probability tests to check specific common outputs that frequently break code 

**Secure Cookies**:
Cookies are information stored by your browser, typically for a limited time 
- used for personalization and tracking as well as session management
- Secure cookies will only be sent over HTTPS
- best practice is to never store sensitive information in a cookie 

**HTTP Secure Headers**: 
Webserver configuration to restrict or allow specific functions of the browser 
- can force the use of HTTPS 
- can only allow Scripts, stylesheets, or images from the local site 

**Code signing**: 
A digital signature added to applications by their developer to ensure the code hasn't been changed
- first a certificate authority signs the dev's public key
- then the dev signs the code with a private key
- for internal applications you should sign with you own certificate authority 

**Allow list/ Deny List**: 
Lists of software that your company allows or deny execution of
- can be setup by administrators for all endpoints
- can be based on application hashes 
- can be based on code certificates 
- can be based on the applications directory path
- can be based on network zone 

**Static Code Analyzers**:
automated way of testing code for vulnerabilities 
- **Static Application Security Testing (SAST)**
- can identify buffer overflows, db injection, etc.
- every find must be examined and find
- can have false positives
- useful for large code bases

[[Application Hardening]]


