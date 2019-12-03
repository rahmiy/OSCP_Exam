---
description: >-
  This is a demonstration article. Thanks to DigiNinja to sharing domains to
  public for training and learning purposes.
---

# 3.1.1.2 DNS Zone Transfer

Link : [https://digi.ninja/projects/zonetransferme.php](https://digi.ninja/projects/zonetransferme.php)

Tutorial link : [https://www.youtube.com/watch?v=kdYnSfzb3UA](https://www.youtube.com/watch?v=kdYnSfzb3UA)

Given the zone transfer is enabled \(due to misconfiguration\)

## Checking if the NS is vulnerable to Zone Transfer

This is not the actual zone transfer attack, we are first checking if could perform the zone transfer for the given NS.

### Example 1- Using "host" : yes vulnerable

![](../../../../.gitbook/assets/image-32.png)

### Example 2- Using "dig" : yes vulnerable

![](../../../../.gitbook/assets/image-31.png)

## Performing Actual Zone transfer

### Example 1 - Using "dig"

![](../../../../.gitbook/assets/image-5.png)

### Example 2- Using nslookup

![](../../../../.gitbook/assets/image-54.png)

