# Passing the hash

## Working

* In this technique, there are some requirements
  * username in clear text
  * password in hash format. given the hashed passwords are not salted and remain static between sessions.
* So instead of cracking the hash, we could simply use the hashed password for authentication.

