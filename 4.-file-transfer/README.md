---
description: >-
  I have a problem  with remembering information that is very specific. So I
  have created a list of file transfer methods. I have not made any distinction
  of either windows or Linux.
---

# 6. File Transfer

Link : [https://burmat.gitbook.io/security/hacking/one-liners-and-dirty-scripts\#file-transfers](https://burmat.gitbook.io/security/hacking/one-liners-and-dirty-scripts#file-transfers)

Link : [https://www.hackingarticles.in/compressive-guide-on-file-transfer-post-exploitation/](https://www.hackingarticles.in/compressive-guide-on-file-transfer-post-exploitation/)

## List of different ways for transferring a file

1. File Transfer protocols
   1. FTP
   2. SFTP
   3. TFTP
   4. SCP
2. Using HTTP Protocol
3. Using file download method
   1. BITSAdmin \(windows, client only\)
   2. PowerShell \(windows, client only\)
   3. VBS HTTP
   4. Perl HTTP
   5. CERTUTIL
   6. base64
   7. curl \(client only\)
   8. wget \(client only\)
4. Tools
   1. HFS tool - file transfer across different platforms.
   2. Using Meterpreter
5. Using PHP file server

## Using Netcat

It is a simple netcat file transfer command

{% tabs %}
{% tab title="Sender side" %}
```text
nc 172.18.39.103 5000 < file.txt
```
{% endtab %}

{% tab title="Receiver side" %}
```text
nc -lvp 5000
```
{% endtab %}
{% endtabs %}

## Using file Download method

To transfer file using Download method, first we need to **set up a web server**.

{% tabs %}
{% tab title="python" %}
```text
python -m SimpleHTTPServer 8000
```
{% endtab %}

{% tab title="apache2" %}
```text
service apache2 start
cp file.txt /var/www/html/
```
{% endtab %}
{% endtabs %}

### Using curl

{% tabs %}
{% tab title="curl file transfer method" %}
```text
curl -O http://172.18.39.103/file.txt
```
{% endtab %}
{% endtabs %}

### Using wget

{% tabs %}
{% tab title="wget file transfer method" %}
```text
wget http://172.18.39.103/file.txt
```
{% endtab %}
{% endtabs %}

## Using PHP file server

{% tabs %}
{% tab title="Server side" %}
```text
php -S 0.0.0.0:80
```
{% endtab %}

{% tab title="Client side" %}
> You could use any file download method to download file.
{% endtab %}
{% endtabs %}

![](../.gitbook/assets/image-13.png)

![](../.gitbook/assets/image-39.png)

