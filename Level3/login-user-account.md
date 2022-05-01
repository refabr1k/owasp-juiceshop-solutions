## Challenge: Log in with x user account

This challenge is exploiting the injection vulnerability at login form found in level 2 challenge. 

By login in with `' or 1=1 -- ` we will be login successfully and notice that the account we loged in via the classic SQL injection payload is user`admin@juice-sh.op`

We know that `--` comments out any other SQL statement in the backend that tries to evaluate if login form eg. user and password = to the one found in database

To clear this challenge, we would exploit this by providing the valid user email address e.g. bender's email

for Login username we use `bender@juice-sh.op' --`  and password field will be any value (this wont be checked because your `--` comments out the SQL statement to check password fields. The underlying statement will be something like 

```sql
select username from user where username='bender@juice-sh.op' -- and password='WhateverPasswordHere_theCheckIsIgnored'
```

