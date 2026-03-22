# AimaneCouissi_NewsletterConfirmationSuppress

[![Latest Stable Version](http://poser.pugx.org/aimanecouissi/module-newsletter-confirmation-suppress/v)](https://packagist.org/packages/aimanecouissi/module-newsletter-confirmation-suppress) [![Total Downloads](http://poser.pugx.org/aimanecouissi/module-newsletter-confirmation-suppress/downloads)](https://packagist.org/packages/aimanecouissi/module-newsletter-confirmation-suppress) [![Magento Version Require](https://img.shields.io/badge/magento-~2.4.0-E68718)](https://packagist.org/packages/aimanecouissi/module-newsletter-confirmation-suppress) [![License](http://poser.pugx.org/aimanecouissi/module-newsletter-confirmation-suppress/license)](https://packagist.org/packages/aimanecouissi/module-newsletter-confirmation-suppress) [![PHP Version Require](http://poser.pugx.org/aimanecouissi/module-newsletter-confirmation-suppress/require/php)](https://packagist.org/packages/aimanecouissi/module-newsletter-confirmation-suppress)

Suppresses the newsletter confirmation email triggered when a subscribed customer changes their email address, keeping the subscription status unchanged.

## Installation
```bash
composer require aimanecouissi/module-newsletter-confirmation-suppress
bin/magento module:enable AimaneCouissi_NewsletterConfirmationSuppress
bin/magento setup:upgrade
bin/magento cache:flush
```

## Usage

Update a subscribed customer's email address from the storefront (**My Account → Account Information**) or from **Admin → Customers → All Customers**. No newsletter confirmation email is sent for the change. New subscriptions continue to follow Magento's default confirmation behavior.

## Uninstall
```bash
bin/magento module:disable AimaneCouissi_NewsletterConfirmationSuppress
composer remove aimanecouissi/module-newsletter-confirmation-suppress
bin/magento setup:upgrade
bin/magento cache:flush
```

## License

[MIT](LICENSE)
