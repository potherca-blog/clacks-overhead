# Adding Clacks Overhead to Cloudflare

To add the `X-Clacks-Overhead` header in Cloudflare, the "Transform Rules" feature can be used. This allows modifying HTTP headers for responses.

After logging in to the Cloudflare Dashboard and selecting a domain, follow these steps:

1. Select "Overview" from the "Rules" section in the left sidebar.
2. Click the <kbd>+ Create Rule</kbd> button. This will open a menu.
3. In the menu, select "Response Header Transform Rules". This will open the "Transform Rules" page.
4. On the "Transform Rules" page, click the <a>Create a Rule</a> link in the "Add Static Header to Response" section. This will open an input form for creating a new rule. In the input form:
5. Provide a Rule name
6. Select "All incoming requests"
7. Provide the Header name `X-Clacks-Overhead` and the value `GNU Robbert Muller`.
8. After filling in the details, click the <kbd>Deploy</kbd> button.

At this point, the header should be added to all responses served by Cloudflare for the selected domain. To check, see [the "How to verify" page][1] Repeat for other domains as desired.

| Steps 1-3 | Step 4 | Steps 5-8 |
| :-------: | :----: | :-------: |
| ![][2]    | ![][3] | ![][4]    |

[1]: ../verify-headers/
[2]: ../img/cloudflare.add-clacks.01.png
[3]: ../img/cloudflare.add-clacks.02.png
[4]: ../img/cloudflare.add-clacks.03.png
