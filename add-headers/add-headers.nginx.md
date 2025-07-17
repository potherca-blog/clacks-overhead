# Adding Clack Overhead to Nginx

To add the `X-Clacks-Overhead` header in Nginx, the `add_header` directive in the Nginx configuration file can be used.

1. Locate the Nginx configuration file.
2. Open the configuration file in a text editor with administrative privileges.
3. Add the following line in the `http` block:
   ```nginx
   add_header X-Clacks-Overhead "GNU Robbert Muller";
   ```
4. Save the changes to the configuration file.
5. Restart Nginx to apply the changes by running `service nginx reload`, `nginx -s reload`, `systemctl reload nginx`, or similar command.

At this point the header should be added to all responses served by Nginx. To check, see [the "How to verify" page](../verify-headers/).
