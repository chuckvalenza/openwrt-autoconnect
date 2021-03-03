# Openwrt captive portal scripts

To create more scripts, capture the POST request(s) from Burp when completing
the captive portal for the first time, then ensure that curl commands in script
mimick those actions.

Copy connect scripts in `/usr/bin`, then add the script to crontab to run
within the timeout.

crontab:

```
*/30 * * * * /usr/bin/ruckus-captive-portal
```

