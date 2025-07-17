# Adding Clack Overhead to Apache

To add the `X-Clacks-Overhead` header to Apache, the `Header` directive can be added to the Apache configuration file or the `.htaccess` file.

After setting up the header, [verify it works](../verify-headers/).

## Apache Configuration

1. Locate the Apache configuration file.
2. Open the configuration file in a text editor with administrative privileges.
3. Add the following line within in the global server configuration:
   ```apache
   Header set X-Clacks-Overhead "GNU Robbert Muller"
   ```
4. Save the changes to the configuration file.
5. Restart Apache to apply the changes by running `systemctl restart apache2`, `apache2ctl restart`, `service apache2 restart`, or similar command.

## `.htaccess` File

1. Create a file named `.htaccess` in the root directory of the webroot, if one doesn't already exist.
2. Add the following line to the `.htaccess` file:
   ```apache
   <IfModule headers_module>
       Header set X-Clacks-Overhead "GNU Robbert Muller"
   </IfModule>
   ```
 4. Save the changes to the `.htaccess` file.

A server restart is usually not needed for these changes to take effect.
