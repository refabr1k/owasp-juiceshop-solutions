## Forged Feedback
### Challenge: Post some feedback in another user's name.
### Challenge: Post a product review as another user or edit any user's existing review.

### Category: Broken Access Control

Intercept request when submit a Contact form. Observe that there is a parameter that includes username

```json
{
	"UserId":21,
	"captchaId":31,
	"captcha":"29",
	"comment":"sup (***ter@test.com)",
	"rating":3
}
```

Modify `(***ter@test.com)` to another username and submit.


Similar for the other challenge where you can post review as another user. Just simply change the `author` value 

```json
{
	"message":"Great!",
	"author":"hacker@test.com"
}
```


# How to fix? 
- implement server-side input validation