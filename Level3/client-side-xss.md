## Client-side XSS Protection
### Perform a persisted XSS attack with <iframe src="javascript:alert(`xss`)"> bypassing a client-side security mechanism.
### Category: XSS

We know that there isnt any input validation when creating new users (via `POST /api/Users/` see "Admin registration" challenge). This XSS attack is targeted at the `/administration` page when an administrator logs in and views all registered users, the stored xss payload which is in the email will be rendered.

Using burp, send a `POST /api/Users/` with the following parameter
`{"email":"<iframe src=\"javascript:alert(`xss`)\">","password":"hacker"}` with 2 backslashes to escape the open and close quotes used.

When administrator logins to `/administration` page, the xss will pop.