## Deprecated Interface
### Challenge: Use a deprecated B2B interface that was not properly shut down.

Using Chrome `Inspect` > `Sources` > `main-es2015.js`. Search using `Ctrl + F` for keyword `upload`. 

Observe that the `allowedMimeType` actually allows `xml` type files. If you navigate to `Complaint` form and click upload file, you will notice that the only files allowed are `pdf` and `zip` files. 

![](b2b_xml.png)

Choosing `All Files (*.*)` in the upload form and submit a `xml` file to complete challenge. 

Looking at the javascript console shows that there is an [Error code 410 (Gone)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/410) 