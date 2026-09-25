# ometria.magento2.extension.public

**Purpose**: Public Packagist placeholder that reserves the `ometria_inc/` vendor namespace, so `ometria_inc/module-analytics` cannot be registered by a third party and silently installed when a merchant's `repo.magento.com` credentials do not include the extension. Contains only a `composer.json` (abandoned metapackage, no code) and a README directing merchants to Adobe Commerce Marketplace.

- Ticket: EC-2123 (related: EC-2081, which reserves `ometria/`)
- Real extension: `Ometria/ometria.magento2.extension` (private), distributed via https://commercemarketplace.adobe.com/ometria-inc-module-analytics.html
