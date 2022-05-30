
# **Coin driver for the Omnipay PHP payment processing library**

<p align="center">
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway/advanced/">
        <img src="https://ps.w.org/woo-altcoin-payment-gateway/assets/icon-128x128.png" alt="codesolz.net"/>
    </a>
</p>

<p align="center">
    <img alt="undefined" src="https://img.shields.io/github/last-commit/tuhin18003/WooCommerce-AltCoin-Payment-Gateway.svg">
    <a href="https://codeclimate.com/github/tuhin18003/WooCommerce-AltCoin-Payment-Gateway">
        <img alt="undefined" src="https://api.codeclimate.com/v1/badges/53342611d39bf5044b5f/maintainability">
    </a>
    <img alt="undefined" src="https://img.shields.io/github/languages/code-size/tuhin18003/WooCommerce-AltCoin-Payment-Gateway.svg"> <br>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="undefined" src="https://img.shields.io/wordpress/plugin/wp-version/woo-altcoin-payment-gateway.svg">
    </a>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="undefined" src="https://img.shields.io/wordpress/plugin/tested/woo-altcoin-payment-gateway.svg">
    </a>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="undefined" src="https://img.shields.io/wordpress/plugin/v/woo-altcoin-payment-gateway.svg">
    </a>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="undefined" src="https://img.shields.io/wordpress/plugin/rating/woo-altcoin-payment-gateway.svg">
    </a>
    <br>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="undefined" src="https://img.shields.io/wordpress/plugin/dm/woo-altcoin-payment-gateway.svg">
    </a>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="undefined" src="https://img.shields.io/wordpress/plugin/dt/woo-altcoin-payment-gateway.svg">
    </a>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="Wordpress Plugin Active Installs" src="https://img.shields.io/wordpress/plugin/installs/woo-altcoin-payment-gateway.svg">
    </a>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img src="https://hitcounter.pythonanywhere.com/count/tag.svg?url=https%3A%2F%2Fgithub.com%2FCodeSolz%2FWooCommerce-AltCoin-Payment-Gateway%2Fblob%2Fmaster%2FREADME.md" alt="Hits">
    </a>
    <br><br>
    <a href="https://codesolz.net">
        <img alt="undefined" src="https://img.shields.io/badge/Created%20By-M.Tuhin-brightgreen.svg">
    </a>
</p>
<h2 align="center">WooCommerce AltCoin Payment Gateway - Wordpress plugin</h2>

# Installation
1. Signup for an account at [Coinbase Commerce](https://commerce.coinbase.com/).
2. Create an API Key by going to the Settings tab in the Coinbase Commerce dashboard.
3. Copy the `coinbase/` folder to your Prestashop `modules/` folder.
4. Login to your Prestashop Back Office, navigate to the Modules tab, go to the "Installed Modules" tab and search for "Coinbase Commerce". Click Install to activate the plugin.
5. Click Configure to go to the settings page of the plugin. Set the API Key, Shared Secret Key from Coinbase Commerce Dashboard.
6. Copy webhook url from settings page of the plugin to Coinbase Commerce DashBoard Settings. 

**NOTE:** There is a setting for "Unsafe" mode on the plugins settings page. This should never be set to "Enabled" on a production website. 
It is only used for making testing easier during development, since it will deactivate any validation of the requests that is send to the webhook, which 
will allow the developer to emulate POST requests to the webhook without generating the `X-CC-Webhook-Signature` header.

# Localization
All text strings, labels and descriptions found in the plugin is

### Description

Coinbase Commerce is the digital payment service that allows merchants to accept payments in a variety of digital currencies like Bitcoin, Bitcoin Cash, DAI, Ethereum, Litecoin, and USD Coin. These payments are received directly into a merchant-controlled wallet.

Features:

* Fast — Go live in minutes, not days
* Free — No fees to accept crypto
* Global — Tap into a global customer base
* No Middlemen — Be your own bank
* Irreversible — Chargebacks are a thing of the past

**Requirements**
-------
* [Gravity Forms](https://www.gravityforms.com/) plugin 2.0 or later.

### Installation

This section describes how to install and setup the Gravity Forms Coinbase Commerce Add-On. Be sure to follow *all* of the instructions in order for the Add-On to work properly.

### Requirements

Requires at least WordPress 4.0, PHP 5.3, [Gravity Forms](https://rocketgenius.pxf.io/c/1212782/445235/7938) 1.9.

### Steps

1. Make sure you have your own copy of [Gravity Forms](https://www.gravityforms.com/). This plugin does not include Gravity Forms.

2. You'll also need a Coinbase Commerce account. To signup visit https://commerce.coinbase.com/

3. Download zip archive from [releases page](https://github.com/coinbase/coinbase-commerce-gravity-forms/releases) and unzip or clone plugin and run `composer install` inside clonned folder

4. Upload the plugin folder gf-coinbase-commerce to your WordPress site /wp-content/plugins folder.

5. Visit the **Plugins** menu in your WordPress dashboard, find `Coinbase Commerce Payments For Gravity Forms` in your plugin list, and click the Activate link.

6. Visit the **Forms->Settings** menu, select the Coinbase Commerce Tab, and add your API Key, Shared Secret Key from Coinbase Commerce Dashboard (https://commerce.coinbase.com/dashboard/settings).

7. Copy Webhook Notification Url from Coinbase Commerce Tab to Settings/Webhook subscription https://commerce.coinbase.com/dashboard/settings

8. Create new Gravity form and add Coinbase Commerce Feed.

### Frequently Asked Questions

**Do I need to have SSL?**  
Yes, for webhook notifications you need SSL.

**Does Coinbase Commerce integrate with other e-commerce platforms?**  
Yes, a list of all offical integrations can be found here: [Coinbase Commerce Integrations](https://commerce.coinbase.com/integrate).

### Changelog

**1.0.0**

* Initial release version

