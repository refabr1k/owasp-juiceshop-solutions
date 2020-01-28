## Login Admin
### Challenge: Log in with the administrator's user account.

Click `Account` > `Login`. Perform a classic SQL injection attack for `Email` input using `' or 1=1 --` (key in anything for password).


## Admin Section
### Challenge: Access the administration section of the store.

You must first login as 'admin' user first, see above.

To find the path for administration section, perform the steps in [Level 1 - Score Board challenge](../master/level%201/score-board.md). You will observe there is a `administration` endpoint. 

Navigate to `http://192.168.247.136:3000/#/administration` to complete the challenge.


## Five-Star Feedback
### Challenge: Get rid of all 5-star customer feedback.

After accessing the `administration` page. Delete the 5-star feedback by clicking the 'thrash bin' icon beside it.