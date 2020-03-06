## DOM XSS
### Challenge: Perform a DOM XSS attack with <iframe src="javascript:alert(`xss`)">.

Enter ``<iframe src="javascript:alert(`xss`)">`` at search box.

_Note: There are many ways to weaponize XSS attack. One common example would be to use `alert(document.cookie)` to steal client's session cookie or perform CSRF attack (using victim to execute malicious code/commands on your behalf)_ 
