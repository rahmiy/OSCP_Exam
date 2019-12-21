# John the ripper

Given we have hash dump stored in `hashes.txt`

![](../../.gitbook/assets/image%20%2820%29.png)

## Using john.conf

* during password proofing we get a list of string to work with.
* We could add/mutate the list to a more password oriented list like including numbers in every string at the last.
* To do this, we could use john.conf to do it efficiently.
* We just need to and an extra rule.

![](../../.gitbook/assets/image%20%284%29.png)

![](../../.gitbook/assets/image%20%281%29.png)

* `john --wordlist=file1.txt --rules --stdout > mutated.txt`
  * `--rules` : specifies john the ripper to use rules.



