Bug Submitter: 佟金波

[Password Storage Application v1.0](https://www.sourcecodester.com/php/15726/password-storage-application-phpoop-and-mysql-free-source-code.html) was discovered to contain a cross-site scripting (XSS) vulnerability via the add-fee.php. This vulnerability allows attackers to execute arbitrary web scripts or HTML via a crafted payload injected into the cmddept parameter.

1. vendors: [sourcecodester.com](https://www.sourcecodester.com/php/15726/password-storage-application-phpoop-and-mysql-free-source-code.html);
  
2. Vulnerability location: /psa_php/api.php?action=save
  
[+] Payload:

```java
"><script>alert(1)</script>
```
Please execute the Payload provided above, as shown in the following figure：
![image](https://user-images.githubusercontent.com/115358571/194711505-4720d0bf-0262-40be-9c18-c4d921d52e6a.png)
![image](https://user-images.githubusercontent.com/115358571/194711513-2ee6e7ce-0bf9-450d-95e1-16c466fe3f55.png)
