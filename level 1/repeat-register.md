## Repetitive Registration
### Challenge: Follow the DRY principle while registering a user.

Intercept HTTP request for registering a new user. Modify the values using burpsuite such that the values `password` and `passwordRepeat` are different. Forward the request.

```
...
"password":"hacker","passwordRepeat":"hacker1"
...
```


_Note: The correct solution seem to be_
1. Enter a 5 character password_
2. In the repeat password input, key in the same 5 character and observe that as you reach the 5 character there would be a prompt that says `Passwords do not match`
3. Now return to password input and change the pass to something totally different and observe that there are no prompts that show that passwords do not match.
source: https://bkimminich.gitbooks.io/pwning-owasp-juice-shop/content/appendix/solutions.html_
