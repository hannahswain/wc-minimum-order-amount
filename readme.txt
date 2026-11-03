=== WC Minimum Order Amount ===

Contributors: fernashes
Tags: woocommerce, order amount, order total, minimum order, cart
Requires at least: 4.5.0
Tested up to: 7.1.4
Requires PHP: 7.4
Stable tag: 2.0
WC requires at least: 3.0
WC tested up to: 11.2.1
License: GPLv3 or later License
URI: http://www.gnu.org/licenses/gpl-3.0.html
Original snippet source: https://docs.woocommerce.com/document/minimum-order-amount/

Set a minimum order amount for WooCommerce, based on the subtotal or the total. Works with the classic pages and the cart and checkout blocks.

== Description ==

This plugin adds the option for a minimum order amount, as well as the option change the notification text for the cart page. Customers can't proceed to checkout if the order doesn't meet the minimum order amount.

It works with the cart and checkout blocks as well as the classic cart and checkout pages.

Under WooCommerce > Settings > General, the Shipping and tax setting lets you choose whether the minimum uses the subtotal (shipping and tax don't count) or the total (shipping and tax count). New installs use the subtotal. Stores that already had a minimum keep using the total until you change it.

Contributions are welcome on [GitHub](https://github.com/hannahswain/wc-minimum-order-amount).

== Installation ==

1. Download the plugin and install it to your `wp-content/plugins` folder, or install the plugin through the WordPress plugins screen directly
2. Activate the plugin through the 'Plugins' screen in WordPress
3. Navigate to **WooCommerce > Settings** and scroll down to the Minimum order settings to configure the settings

== Screenshots ==



== Changelog ==

= 2.0 2026-11-03 =
 * Added: a Shipping and tax setting under **WooCommerce > Settings > General**. Choose "Use subtotal" or "Use total". Stores that already have a minimum keep "Use total", so nothing changes for them. New installs start with "Use subtotal".
 * Fixed: the minimum is now enforced on the cart and checkout blocks. If your store uses the blocks, orders below your minimum are now refused.
 * Fixed: the cart message was empty if the settings had never been saved.
 * Added: compatibility declarations for high-performance order storage and the cart and checkout blocks.
 * Tested with WordPress 7.1 and WooCommerce 11.2.

 = 1.1 2020-11-10 =
 * Tested and bumped version numbers
 * Found an issue with error validation on checkout where the error is shown but checkout could proceed; background: https://wordpress.org/support/topic/wc_add_notice-doesnt-work-on-checkout-page/
 The current workaround is to stop the customer from proceeding past the cart page if order minimum is not met. Removed notification setting for checkout.

= 1.0 2018-08-11 =
 * Initial release

== Upgrade Notice ==

= 2.0 =
The minimum is now enforced on the cart and checkout blocks. Shipping and tax behavior is unchanged for stores with a minimum; you can switch between subtotal and total in WooCommerce > Settings > General.
