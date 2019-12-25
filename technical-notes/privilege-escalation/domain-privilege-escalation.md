# Domain Privilege Escalation

* privilege escalation just means that if you are not supposed to have admin rights and you doing some stuff got admin rights, this is called privilege escalation.
* In this article we will discuss on authority of admin account

## Normal privilege escalation vs Domain privilege escalation

* Given we have an internal environment that we are try to get into, say "mydomain.org".
* You found the weakest system in the network, which was running some legacy OS and you successfully compromised it.
* But what to do now? You know what ever information is present in that compromised system. But there are a lot of other system in the network. 
* We then try to get the lateral movement to the other machine using the compromised machine.
* This could be achieve in many ways, but lets considered a way where you found some other machine in the same network of that of the compromised machine, and you started targeting those machine from the compromised machine.
* You then found slowly some vulnerabilities and gradually increased your count of compromised machines. But we have to scan every machine, find the vulnerability and know the exploit for that particular machine, which is a time consuming job.
* An alternative way could be, say when we compromised the first machine, we fetched different username and password accounts.
* These usernames have different types of authorization. Like say you found three users 
  * mike
  * john
  * admin\_kim
* Here "mike" account just have local administration privileges, means the account "mike" is only allowed to login to one system i.e. our compromised machine. The account "mike" is useless if we use it to login to other system, even in the same network or any other network machine. So for analogy mike could be an employee.
* Next we have "john" account, which has more access than "mike" account. Using "john" account I was able to access all the system in the same network of that of the compromised machine. The account "john" has more authorization than account "mike". But account "john" was useless for machines on other networks. For analogy john could be manager of mike.
* Next we have admin\_kim, now using this account I was able to access all the machine either in the network or any other network. Which means admin\_kim has more authorization than john and probably the highest authorization possible. For analogy kim could be a administrator who manages all the system in the complete organization. 

**Hence, we say account "admin\_kim" has domain level privileges. And out attack that we did to find out username and password for admin\_kim could be called a domain level privilege escalation.**

**The account "mike" has only has admin rights on one machine. So we call account "mike" is a local administrator privileges. And the attack to fetch the username and password of the account "mike" is called as local privilege escalation.**

