RESTful API for an uptime monitoring System 

An “uptime monitor” allow users to enters URLs
They want monitored and receive alerts when those 
Resources “go down” and “come back up”.

The app have sign-up and sign-in.

I include functionality for sending an SMS alert to a
user rather than email.

API features:

1- The api listens on a PORT and accepts incoming HTTP request for POST ,GET,PUT,DELETE and HEAD.

2-The api allows a client to connect then create new user,
Then edit and delete that user.

3-The API allows a user to “sign in” which gives them a token that they can use for subsequent authenticated requests.

4-The API allow the users to “sign out” which invalidates the their token.

5-The API allows a signed-in user to use their token to create a new “check”(task).

6-The API allows a signed-in user to edit or delete any of their checks.

7-In the background workers perform all the “checks” at the appropriate times,and send alerts to the users when a check changes its state from “up”  to “down” ,or vice versa.

For sms i use Twilio API.
For Database i user JSON only.

