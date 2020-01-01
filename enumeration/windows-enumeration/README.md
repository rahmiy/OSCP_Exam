# Windows Enumeration

### Enumerate user and user privileges

* cmd prompt
  * net user
  * whoami /all

### Enumerate OS version

* cmd prompt
  * systeminfo

### print file contents

* type file1.txt

### Search for files and folders with Admin privileges writable by other users

![](../../.gitbook/assets/image%20%2835%29.png)

![](../../.gitbook/assets/image%20%2831%29.png)

![](../../.gitbook/assets/image%20%2841%29.png)

## Accesschk

to know what kind of accesses specific users or groups have to resources including files, directories, Registry keys, global objects and Windows services.

## Creating a new user with admin rights

{% embed url="https://operating-systems.wonderhowto.com/how-to/create-admin-user-account-using-cmd-prompt-windows-0125689/" caption="reference" %}

```text
net user /add [*username] [password]
net localgroup administrators [username] /add
```

