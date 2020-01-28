## Zero Stars 
### Challenge: Give a devastating zero-star feedback to the store.

Click `Customer Feedback` and fill up the feedback form. Turn on HTTP request interceptor like Burpsuite, modify the POST request `rating` parameter to `0`. Forward the modified request to complete the challenge

eg.
```
POST /api/Feedbacks/ HTTP/1.1
Host: 192.168.247.136:3000
...
{"captchaId":0,"captcha":"-2","comment":"Sucks!","rating":0}
```