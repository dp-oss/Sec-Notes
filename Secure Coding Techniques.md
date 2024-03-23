Coding balances time and quality of code 

- code needs to always be tested 

Vulnerabilities will always be found 


**Stored Procedures:** storing code in the database so that the client can't edit the requests for data
- instead of using `SELECT * FROM my_table WHERE my_option=1`
- use: `CALL get_options`
- This allows the `get_options` procedure to be stored in the DB preventing the end user from making calls to the DB

**Obfuscation/Camouflage**: Make human readable code not understandable to humans but still readable to machines ^fe07e8
- instead of 
	- ` echo "Hello World";`
- Use: 
```php
<?php
function SGVsbG8gV29ybGQh($_ = 0) {(
    $___=__FUNCTION__
    )&&
    !$_ and list($_,$__) = array_values(array_filter($___(42), $___)) and
    !$_($__($___)) and
    $___($___); return
    $_
    &42
    ?current(get_defined_functions()):(
    !((
    $_=md5($_))-42*2)or
    !(md5($_ = md5($_))-42/2
    *3)
);};

SGVsbG8gV29ybGQh();
```

**Code reuse:** Old code containing vulnerabilities is used to make a new app

**Dead Code**: Code that used to do something that no longer does

**A SMALLER CODE BASE WILL HAVE LESS VULNERABILITIES** 


**Input Validation**: Ensuring that fields where a user is inputting information, the user can only enter correctly formatted data  ^bb9aa0
- **normalization** is when you correct users input automatically to suit your use ^758d39
- attackers can use a *Fuzzer* to try many different inputs to see what breaks your coad

**Validation Points:**
- Server-side
	-  all checks occur on server
	- protects against maliscious users
- Client-side
	- the app validates on the client side before sending to server
	- can help filter input from legit users before sending
- Common to use both
	- but note that server side is considered more secure

**Memory Management**: Memory allows many opportunities to build vulnerable code
- never trust data input
- [[Buffer Overflows]] can allow a user to write into other areas of memory
	- make sure data matches buffer size
- Built in memory processes can be vulnerable

**Third-party libraries/SDKs**: Extend function of programming language
- these are not written by language maintainers and thus can introduce security risks
- you need to test these extensively 
- balance features needed with risk

**Data Exposure:** 
- You need to ensure its encrypted at rest and in transit


**Version Control**: Allows you to keep track of changes between versions of code
- can be useful for security to compare the changes made to a file over time
- can be a risk for security because 3rd parties may be able to access previous versions

**Software Diversity:** Creating unique binaries with the same function using compiler tricks. 
- Isolates exploits because if there are vulnerabilities on one machine it won't necessarily work on all machines 
- limits attack surface 