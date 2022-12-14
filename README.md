# WebPT_BugBounty
Bits for Web PT and Bug Bounty

# Broken Authentication and Session Management
## Case 1:

Old Session Does Not Expire After Password Change

1) Create an account on your target site.
2) Login into two browsers(or use Incognito) with same account.
3) Change your password in one browser. On successful password change, Refresh the other browser.
4) If you're still logged in, it's a bug!!

