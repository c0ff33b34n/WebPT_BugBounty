# WebPT_BugBounty
Bits for Web PT and Bug Bounty

# Broken Authentication and Session Management
## Case 1:

Old Session Does Not Expire After Password Change

1) Create an account on your target site.
2) Login into two browsers(or use Incognito) with same account.
3) Change your password in one browser. On successful password change, Refresh the other browser.
4) If you're still logged in, it's a bug!!

## Case 2:

Session Hijacking (Intended Behaviour)

1) Create and login to your account.
2) Use cookie editor extension and copy all the target cookie.
3) Logout your account and paste the cookie in cookie editor extension.
4) Refresh the page and if you are logged in then it's a bug!! (Session Hijacking)

Impact: If the attacker gets the cookies of the victim it will lead to an account takeover.

## Case 3:

Password reset token does not expire (Insecure Configuration)

1) Create a account in your target website and request for password forget link (don't use it).
2) Login with your old password and change the email to another one.
3) Now use the password link and check if you are able to change your password.
4) If password is changed, it's a bug!! (small one)

## Case 4:

Server security misconfiguration

Lack of security headers -> Cache control for a security page

1) Login and navigate around some pages.
2) Logout the application.
3) Press Alt + Left-arrow.
4) If you are again logged in or can view pages navigated by the user. It's a bug!! (again small one XD) Also check if you are able to change the password.

<loading...>
