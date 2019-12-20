# Windows Privilege Elivation

* Given that we have a victim windows server running running in older versions. We could first find a vulnerability in exploit database against this vulnerable version of windows for privilege escalation.
* Given we have credentials of a normal user with low privileges.
* But this is python script that we got as our exploit.
* But our victim system may or may not have python installed. Hence we first convert this python script to windows executable using "pyinstaller".
* Then we simply execute this malicious .exe with normal privileges.
* After execution we get admin shell.

