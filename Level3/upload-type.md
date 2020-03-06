## Upload Type
### Challenge: Upload a file that has no .pdf or .zip extension.

Click `Complaint` and fill in Complaint form, also select upload file and choose a pdf file. 

Using burp suite intercept http request. Modify `filename=something.png` and `Content-Type: image/png` forwarding the request. 