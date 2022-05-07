# NoSQL Dos
## Challenge: Let the server sleep for some time
## Category: Injection

1. When viewing product reviews observe the API call `http://127.0.0.1:3000/rest/products/1/reviews`

2. Modify to inject sleep command `http://127.0.0.1:3000/rest/products/sleep(10000)/reviews`