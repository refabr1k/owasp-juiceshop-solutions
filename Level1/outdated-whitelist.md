## Outdated Whitelist
### Challenge: Let us redirect you to one of our crypto currency addresses which are not promoted any longer.

Using `JSFinder.py` search for all endpoints. 

```bash
python JSFinder.py -u http://127.0.0.1:3000/

#...
#http://127.0.0.1:3000/order-summary
#http://127.0.0.1:3000/redirect?##to=https://blockchain.info/address/1AbKfgvw9psQ41NbLi8kufDQTezwG8DRZm
#http://127.0.0.1:3000/redirect?
#..

```

Observe that there is a redirect URL, try navigating to it to solve the challenge.

---


### old
Using [@hakluke](https://twitter.com/hakluke/)'s tool [hakrawler](https://github.com/hakluke/hakrawler) we can quickly search all endpoints such as 'redirects' by simply running 

`hakrawler -url http://127.0.0.1:3000 -linkfinder | grep redirect`

There is a particular redirect url used that is `redirect?to=https://blockchain.info/address/1AbKfgvw9psQ41NbLi8kufDQTezwG8DRZm`

Use this redirect from juicebox website to solve the challenge `http://127.0.0.1:3000/redirect?to=https://blockchain.info/address/1AbKfgvw9psQ41NbLi8kufDQTezwG8DRZm`

_Note: Using the `hakrawler` tool made discovery easier, but if not, you can use `Inspect` and view `Sources` looking into the javascript files content `Ctrl + F` the specific keywords that are interesting. I have learnt that alot of juicy stuff are found in javascripts_
