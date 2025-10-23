Wordpress sites can be notoriously fragile and hard to work with, but luckily there’s a straightforward process to getting a Booker instance embedded.

1. Install the WPCode plugin
The WPCode plugin is a safe way to inject custom code snippets without having to muck about in the theme’s functions.php file — there lies danger, or so the internet says.

Select Plugins from the side menu
Search for WPCode
Install and activate the plugin
If you refresh, you should now see a new menu item: Code Snippets

2. Adding the Booker scripts
Click on Code Snippets in the menu; a sub-menu will open.
Select Header & Footer
In the Footer section, paste all necessary Booker scripts. They should look something like this:
<link rel="stylesheet" href="https://ottawa-valley-farm-to-fork.booker.tech/build/booker-launcher.css">

<script type="module" src="https://ottawa-valley-farm-to-fork.booker.tech/build/booker-launcher.esm.js" data-stencil-namespace="booker-launcher"></script>

<script nomodule="" src="https://ottawa-valley-farm-to-fork.booker.tech/build/booker-launcher.js" data-stencil-namespace="booker-launcher"></script>
Make sure to save your changes.

3. Adding the actual Booker launcher to a page
From the side menu, select Pages, and on the next page, select the specific page to which you want to add a Booker.
In the page editor, find the specific content block you want to edit. By default, the block’s editor might be set to visual; instead, select the text option.
In the code field, paste your launcher code, for example:
<ttc-booker-launcher bkr-id="65661799d24ab6adcf1354c8" product-id="65661cccd24ab6adcf135fb2"><a href="#!" style="background:#68925D; color:#ffffff; padding:12px 16px; text-decoration:none; border-radius:8px;">Book Now</a></ttc-booker-launcher>
That's it!
