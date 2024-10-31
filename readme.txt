=== Newsletter subscription optin module ===
Contributors: nonletter
Donate link: https://www.sendblaster.com/
Tags: sidebar, widget, newsletter, email, bulk email, management
Requires at least: 2.9.0
Tested up to: 5.8.1
Stable tag: 1.2.9
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Plugin for managing subscriptions to a mailing list. It provides a simple form for subscription to your mailing list through single or double opt-in.

== Description ==

This plugin enables you to create simple forms for subscription to your newsletter. It includes a sidebar widget with customizable fields (up to 16) to gather from your users all the information you need for your email marketing campaigns. Users can also use the form to unsubscribe.

From the options pages you can:

* choose whether you require a double opt-in (users must follow a link in an email message, in order to complete subscription)
* specify name and number of text fields in the form
* customize text messages and labels
* manage subscribed email addresses
* donwload PDF file with list of subscribers
* download CSV file with list of subscribers
* choose whether you want to download all subscribers or only new subscribers

= Related features =

(Un)subscription requests can be directly processed by [SendBlaster bulk email software](https://www.sendblaster.com "bulk email software") :

* [download SendBlaster here](https://www.sendblaster.com/free-bulk-emailer-download/ "bulk email software download")

= Plugin Features =

* Subscribe new members
* Unsubscribe existing members
* Stores subscribed email addresses (as a useful backup against mail delivery failures)
* Purges old email addresses
* Customizable sidebar appearance
* Customizable texts and labels
* Adds to your form up to 5 custom fields

= Plugin Options =

* E-mail address for managing subscriptions
* Message to subscriber - subject
* Message to subscriber - content
* Double Opt-in
* Link Love (enable and disable)
* Front side messages
* Front side appearance and custom fields
* Temporary db of newly subscribed members
* Automatic temporary db cleanup


== Installation ==

This section describes how to install the plugin and get it working.

1. Unzip the downloaded archive
2. Upload the script `wpsb-opt-in.php` to the `/wp-content/plugins/` directory
3. Activate the plugin through the 'Plugins' screen in WordPress
4. Use the Settings->Plugin Name screen to configure the plugin
5. Go to `Wp SendBlaster Opt-in` and set the **email address** that you intend to use for managing subscriptions. This should be the same address you have provided in your [bulk email software Manage subscriptions](http://www.sendblaster.com/bulk-email-software/wp-content/manage-subscriptions.gif "manage subscriptions help screenshot") configuration
6. In the `Appearance->Widgets` menu, drag to your sidebar the newly added plugin


== Frequently Asked Questions ==

= I am unable to delete the temporary opted in users. I get this message: Cannot load wpsb-opt-in.php =

The wpsb-opt-in.php file must be in the `/wp-content/plugins/` folder and not in a subdirectory.

= Is it possible to show the form in the body of a page rather than on the sidebar? =

Yes: to have the newsletter widget inside a post you must enable PHP execution inside posts. This can be done, for instance, by installing the PHP Everywhere plugin:

https://wordpress.org/plugins/php-everywhere/

then write this code in your post:

`<?php wpsb_opt_in(); ?>`