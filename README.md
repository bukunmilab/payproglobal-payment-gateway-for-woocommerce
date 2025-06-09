# PayProGlobal for WooCommerce

![WooCommerce](https://img.shields.io/badge/WooCommerce-Compatible-blue?logo=woocommerce)
![WordPress](https://img.shields.io/badge/WordPress-6.0+-blue?logo=wordpress)
![License](https://img.shields.io/badge/License-Commercial-red)

A **PayProGlobal** payment gateway integration for WooCommerce, supporting one-time payments and recurring subscriptions.

## Features
- ✅ **Seamless Checkout**: Redirect customers to PayProGlobal for secure payments
- 🔄 **Subscription Support**: Works with WooCommerce Subscriptions (recurring payments)
- 🔐 **Secure Webhooks**: Handles payment confirmations, refunds, and subscription events
- 🛠 **Product Mapping**: Map WooCommerce products to PayProGlobal Product IDs
- 📊 **Order Sync**: Automatic status updates for charges, refunds, and chargebacks
- 🧪 **Test Mode**: Test payments without processing real transactions

## Installation
1. Upload the `ppg-for-woocommerce` folder to `/wp-content/plugins/`
2. Activate the plugin via **WordPress Admin → Plugins**
3. Configure under **WooCommerce → Settings → Payments → PayProGlobal**

## Configuration
### Gateway Settings
- Enable/disable the payment method
- Set title/description shown at checkout
- Configure test/live modes
- Add API keys (Secret Key, Dynamic Settings Key/IV)

### Product Setup
1. Edit a WooCommerce product
2. Under **Product Data → General**, enter:
   - **PPG Product ID** (required for all products)
   - **PPG Subscription ID** (if different from product ID, for subscriptions)

## Webhook Setup
1. In PayProGlobal, set the IPN URL to:  
   `https://yourdomain.com/wc-api/ppg_callback`
2. Ensure your server allows inbound POST requests to this endpoint

## Requirements
- WordPress 6.0+
- WooCommerce 7.0+
- PHP 7.4+
- WooCommerce Subscriptions (optional, for recurring payments)

## Support
For assistance, contact:  
📧 support@loquisoft.com  
🌐 [https://loquisoft.com](https://loquisoft.com)

---

**License**: Commercial (Proprietary)  
**Author**: [Loquisoft](https://loquisoft.com)  
**Version**: 1.0
