# 7.3 SQL Injection

## Types of SQL Injection

* Error based SQL Injection \(given we have verbose errors from web application\)
  * like Union Select method.
* Blind SQL
  * First we need to check whether our input affects the output of the SQL query, as error reporting is disabled.
  * Use this method if verbose error are not enabled.
  * We could make use of 
    * sleep\(\) - command execution
    * IF\(MID\(\)\) - conditional command execution
    * into OUTFILE
    * union select

## Check if webapp is vulnerable to SQL Injection

## Given webapp is vulnerable to SQL injection how to extract useful information.

1. **Union Select Method** for gathering more information during SQL Injection
2. **into OUTFILE**
3. **executing sql commands** such as sleep\(5\), user\(\), etc.
