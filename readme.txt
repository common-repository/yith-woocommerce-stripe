=== YITH WooCommerce Stripe ===

Contributors: yithemes
Tags: stripe, simple stripe checkout, stripe checkout, credit cards, online payment, payment, payments, recurring billing, subscribe, subscriptions, bitcoin, gateway, yithemes, woocommerce, shop, ecommerce, e-commerce
Requires at least: 5.3
Tested up to: 5.6
Stable tag: 2.0.17
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

The YITH WooCommerce Stripe plugin let you add a new payment gateway based on Stripe.com

== Description ==

Stripe is a WooCommerce extension, that allows you to add a new payment gateway into your e-commerce website and gives your
users the possibility to pay directly by credit card through Stripe.com checkout.

Stripe is available in the United States, Canada, the UK, Australia, Belgium, France, Germany, Ireland, The Netherlands
and more – see [What countries does stripe support?](https://stripe.com/global)

Stripe advantages:

*   "Proven fraud protection", stripe actively works to protect your business from fraudulent charges and monitors suspicious transactions.
*   "Act locally, work globally", work with international customers right out of the box while still getting paid in your preferred currency.
*   "Operations, simplified", handling billing support and disputes is easy with Stripe — address issues with a few clicks, or automate it.
*   "Battle-tested systems", [high availability](https://status.stripe.com/), transparent uptime reporting, and always ready for high transaction throughput.
*   "Seamless security", stripe provides security and compliance without the headaches.

Please, read the the **[official plugin documentation](http://yithemes.com/docs-plugins/yith-woocommerce-stripe)** to know all plugin features.

== Installation ==

1. Unzip the downloaded zip file.
2. Upload the plugin folder into the `wp-content/plugins/` directory of your WordPress site.
3. Activate `YITH WooCommerce Stripe` from Plugins page

= Configuration =

YITH WooCommerce Stripe will add a new settings tab called "Stripe", into Woocommerce -> Settings -> Checkout -> Stripe. Here you are able to configure all the plugin settings.
You need to register an account to [Stripe.com](https://stripe.com/) and set the API key in the plugin settings.
You can get the API keys from [your stripe dashboard](https://dashboard.stripe.com/account/apikeys).

== Frequently Asked Questions ==

= Does this plugin support Stripe Checkout? =
Yes it does! After user has compiled all information on checkout page, you will be redirect to payment page where there is the Stripe Checkout button and pay.

= Which countries does Stripe support? =
Stripe is available in many countries and is constantly expanding to more. To see if your country is supported, visit the [Stripe Global page](https://stripe.com/global).

= Does Stripe require that my site have an SSL certificate? =
Yes, an SSL certificate should always be used with Stripe. All pages that include a payment form should be prefixed with https://, not http://. See [Stripe’s SSL page](https://stripe.com/help/ssl) for more information.


== Screenshots ==

1. The payment method on checkout page
2. Pay page
3. Stripe.com Checkout panel
4. Settings

== Changelog ==

= 2.0.17 - Released on 09 December 2020 =

* New: support for WooCommerce 4.8
* Update: plugin framework
* Update: Stripe PHP library to 7.66.1

= 2.0.16 - Released on 12 November 2020 =

* Update: plugin framework
* Fix: avoid notice caused by missing YITH_WCSTRIPE_SLUG constant

= 2.0.15 - Released on 11 November 2020 =

* New: support for WordPress 5.6
* New: support for WooCommerce 4.7
* Update: plugin framework
* Update: Stripe PHP library to 7.62.0
* Tweak: added minified versions of the scripts
* Dev: removed deprecated .ready method from scripts

= 2.0.14 - Released on 16 October 2020 =

* Update: plugin framework
* Tweak: workaround to make Checkout mode work when Gift Cards are applied to the order

= 2.0.13 - Released on 30 September 2020 =

* New: Support for WooCommerce 4.6
* Update: plugin framework
* Dev: added new filter yith_stripe_cancel_url

= 2.0.12 - Released on 18 September 2020 =

* New: Support for WooCommerce 4.5
* Update: plugin framework
* Update: Stripe PHP library to version 7.52
* Update: API version to 2020-08-27

= 2.0.11 - Released on 14 August 2020 =

* New: Support for WordPress 5.5
* New: Support for WooCommerce 4.4
* Update: plugin framework
* Update: Stripe PHP library to version 7.47.0
* Tweak: added check over YITH_DOING_RENEWS constant on is_available method of the gateway
* Fix: remove HTML tags of product description in Stripe checkout mode
* Dev: added new parameter to filter yith_wcstripe_checkout_session_detailed_line_items

= 2.0.10 - Released on 10 June 2020 =

* New: Support for WooCommerce 4.2
* Update: plugin framework
* Update: Stripe PHP library to version 7.37.0
* Dev: added yith_wcstripe_capture_charge_params filter

= 2.0.9 - Released on 08 May 2020 =

* New: Support for WooCommerce 4.1
* New: added line details for Stripe Checkout
* Update: plugin framework
* Update: Stripe PHP library to version 7.31.0
* Fix: issue with free item when creating Checkout session
* Fix: issue with short description of the item when creating checkout session
* Dev: added filter yith_wcstripe_checkout_session_detailed_line_items to disable line details on Stripe Checkout
* Dev: added yith_wcstripe_session_param filter

= 2.0.8 - Released on 18 March 2020 =

* Update: plugin framework
* Fix: empty settings panel

= 2.0.7 - Released on 14 March 2020 =

* New: support for WordPress 4.0
* New: support for WooCommerce 4.0
* New: support for API 2020-03-02
* Update: Stripe PHP library to version 7.27.2
* Update: plugin framework

= 2.0.6 - Released on 24 December 2019 =

* New: support for WooCommerce 3.9
* Update: plugin framework
* Update: Stripe library to version 7.14.2
* Update: Stripe API to version 2019-12-03
* Fix: Removed usage of Stripe\Exception\ApiErrorException::factory; using new Exception instead

= 2.0.5 - Released on 12 December 2019 =

* Update: Plugin framework

= 2.0.4 - Released on 29 November 2019 =

* Update: Notice handler
* Update: Plugin framework

= 2.0.3 - Released on 07 November 2019 =

* New: support for WordPress 5.3
* New: support for WooCommerce 3.8
* New: support for API 2019-11-05
* Update: Plugin framework
* Update: StripePHP library

= 2.0.2 - Released on 30 October 2019 =

* Update: Plugin framework

= 2.0.1 - Released on 06 September 2019 =

* Fix: error on session creation when user is guest (thanks to Paul & Maurice)

= 2.0.0 - Released on 05 September 2019 =

* New: support to latest API version (2019-08-14)
* New: support to SCA-ready payment methods only
* New: support to new version of Stripe Checkout
* Update: internal plugin framework
* Update: Stripe php library to version 7.0.0
* Fix: undefined variable err on gateway error reporting method
* Delete: dropped support to legacy payment method (as suggested by Stripe)

= 1.9.3 - Released on 12 August 2019 =

* New: WooCommerce 3.7.0 RC2 support
* Update: internal plugin framework
* Fix: calculate cart totals before sending it to stripe, to make stripe checkout work with gift card
* Dev: added method to API class, to update cards

= 1.9.2 - Released on 13 June 2019 =

* Update: internal plugin framework
* Dev: New filter yith_wcstripe_charge_params

= 1.9.1 - Released on 23 April 2019 =

* Update: internal plugin framework

= 1.9.0 - Released on 11 April 2019 =

* New: WooCommerce 3.6 support
* New: added check over site url, to set Test Mode when plugin is enabled on a staging installation
* Tweak: improved error reporting system
* Update: internal plugin framework
* Update: dutch translation

= 1.8.1 - Released on 11 February 2019 =

* New: WooCommerce 3.5.4 support
* Update: internal plugin framework
* Update: Stripe php library to version 6.29.3

= 1.8.0 - Released on 19 December 2018 =

* New: WordPress 5.0 support
* New: WordPress 3.5.2 support
* New: support to latest API version (2018-11-08)
* Tweak: check over configurable properties in update_subscription method
* Update: internal plugin framework
* Update: dutch translation
* Dev: added filter yith_wcstripe_error_message_order_note to let third party code filter error messages stored in order notes

= 1.7.2 - Released on 24 October 2018 =

* New: WooCommerce 3.5 support
* Tweak: updated plugin framework

= 1.7.1 - Released on 15 October 2018 =

* Fix: wrong links on admin page
* Fix: restored plugin panel under YITH menu
* Update: italian translation

= 1.7.0 - Released on 09 October 2018 =

* New: added WordPress 4.9.8 compatibility
* New: added WooCommerce 3.5-RC compatibility
* New: updated Stripe API version to 2018-09-24
* New: updated plugin framework
* New: added pt_PT translation (thanks to Ricardo A.)
* Tweak: removed create_function for php 7.2 compatibility
* Tweak: removed usage of deprecated WC function from gateway class
* Fix: order total when paying from order-pay endpoint
* Fix: SSL error notification on admin pages
* Fix: invalid Stripe API version
* Dev: added yith_wcstripe_gateway_us_icons filter
* Dev: added yith_wcstripe_gateway_default_icons filter
* Dev: added yith_wcstripe_gateway_icon filter
* Dev: added yith_wcstripe_use_plugin_error_codes filter to show original API error messages
* Dev: added yith_wcstripe_error_message filter to let third party code filter error messages

= 1.6.0 - Released on 28 May 2018 =

* New: WooCommerce 3.4.0 support
* New: WordPress 4.9.6 support
* New: updated plugin fw
* New: GDPR compliance
* New: Stripe library 6.7.1 (Requires API update on Stripe Dashboard)
* Dev: added filter yith_wcstripe_gateway_enabled to programmatically enable/disable Stripe Gateway
* Dev: added filter yith_wcstripe_gateway_id to let developers filter gateway ID (Use this filter at your own risk; after filtering gateway ID you will need to configure gateway again)

= 1.5.0 - Released on 08 February 2018 =

* New: WooCommerce 3.3.1 support
* New: WordPress 4.9.4 support
* New: updated Stripe library to 6.0 revision
* New: updated plugin-fw library

= 1.4.0 - Released on 09 January 2018 =

* New: WooCommerce 3.2.6 support
* New: updated plugin-fw to version 3.0
* New: updated Stripe library to 5.8 revision
* Fix: check on captured flag on payment_complete
* Dev: added yith_wcstripe_environment filter
* Dev: added yith_wcstripe_metadata filter to let third party developers change metadata sent to Stripe servers

= 1.3.0 - Released on 04 April 04 =

* New: WordPress 4.7.3 compatibility
* New: WooCommerce 3.0.0-RC2 compatibility
* New: added italian - ITALY translation
* Tweak: added check over gateway existence
* Tweak: updated Stripe library to 3.23.0
* Tweak: changed text domain to yith-woocommerce-stripe
* Dev: added yith_stripe_locale filter to change locale used in hosted checkout

= 1.2.9 - Released on 31 May 2016 =

* Added: Support to WC 2.6 beta 3

= 1.2.7.1 - Released on 11 April 2016 =

* Fixed: missing files causing warnings

= 1.2.7 - Released on 06 April 2016 =

* Fixed: fatal error with Stripe\Error\API
* Fixed: wrong cart total on hosted checkout
* Fixed: internal server error if the import is lower then .50 cent

= 1.2.5 - Released on 16 February 2016 =

* Fixed: stripe library loading causing fatal error in some servers

= 1.2.4 - Released on 19 January 2016 =

* Added: compatibility with WooCommerce 2.5
* Added: language support for "Stripe checkout" mode
* Updated: Stripe API library with latest version

= 1.2.3 - Released on 14 December 2015 =

* Fixed: no errors for wrong cards during checkout

= 1.2.2 - Released on 10 December 2015 =

* Added: compatibility to multi currency plugin

= 1.2.0 - Released on 12 August 2015 =

* Added: Support to WooCommerce 2.4
* Updated: Plugin core framework
* Updated: Language pot file

= 1.1.0 - Released on 22 April 2015 =

* Added: support to WordPress 4.2

= 1.0.4 - Released on 21 April 2015 =

* Updated: Languages pot catalog

= 1.0.3 - Released on 15 April 2015 =

* Updated: Stripe API
* Fixed: minor bugs

= 1.0.2 - Released on 04 March 2015 =

* Updated: Plugin core framework

= 1.0.1 - Released on 03 March 2015 =

* Fixed: minor bugs

= 1.0.0 =

* Initial release
