# CSP Bypass
## Challenge: Bypass the Content Security Policy and perform an XSS attack on a legacy page within the application. 
## Category: XSS

1. The `username` field has filtering in place that removes part of the `<script>` string. e.g.  

```
<script>alert(`xss`)</script>
```

becomes
```
lert(`xss`)</script>
```


However, this could be bypassed. Use this to bypass the filter  

```
<<script>ascript>alert(`xss`)</script>
```

2. Observe from Developer tools (Console) that the Content-Security-Policy blocked the loading of scripts. This is the reason why the XSS did not pop. 

![](screens/xss-csp.png) 

Observe that the Image URL you upload is directly reflected and whitelisted in the CSP header response. Whatever is being used in the Image URL field will be 'injected' into the CSP header

![](screens/xss-csp-header.png)

3. To bypass the CSP, add the `'unsafe-inline'` into CSP to allow script from being run. The payload will be `http://test.png; script-src 'unsafe-inline' 'self' 'unsafe-eval'`. Once upload, refresh to trigger the XSS

![](screens/xss-csp-bypassed.png)