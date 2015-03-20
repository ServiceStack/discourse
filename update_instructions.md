## Rebuild container
These are instructions to get the custom discourse instance back to working order.

1. Login to the AWS instance
2. cd /var/discourse
3. sudo ./launcher rebuild app
4. Wait for about 5-10 minutes
5. sudo ./launcher enter app
6. cd /var/www/discourse
7. git checkout master
8. git fetch origin
9. In a browser, navigate to Discourse site
10. Goto /admin/upgrade
11. Update should be pending for latest commit into master of custom source
12. Click update for pending updates
13. Wait for Server to come back (30 seconds)
