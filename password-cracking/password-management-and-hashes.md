# Password Management and Hashes

* We store passwords not in clear text but in hash format.
* During authentication, the password input by user is first hashed, and this hash is compared with the previously stored password hash in the database. If match is successful user is authenticated.
* Hashes are fixed length string, irrespective of the input string size, the size of the output hash is always fixed.
* You could identify and differentiate most of the hashes, seeing some identifying traits.

### Below are the list of hashing techniques used in common distributions

* Linux
  * d
  * d
  * d
* Windows
  * windows 7 : asd
  * windows 10 : 
* 
## Windows Password Management

* Windows stores password in security account manager \(SAM\).
  * from windows NT upto windows 2003
* Lan manager hashes \(LM hashes\)
  * weak
  * long passwords are splitted and hashed separately.
  * the password is converted to uppercase characters before being hashed.
  * no salts.
* NT Lan manager hashes \(NTLM hashes\)

