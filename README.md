# ometria_inc/module-analytics — Packagist name reservation

**This package contains no code.** It exists only to reserve the `ometria_inc/` vendor namespace on Packagist, so that no third party can publish a package under the same name as the official Ometria Magento 2 extension.

## Installing the Ometria extension

The Ometria Magento 2 extension is distributed **exclusively** through Adobe Commerce Marketplace:

https://commercemarketplace.adobe.com/ometria-inc-module-analytics.html

1. Acquire the extension on Marketplace using the Adobe Commerce account whose access keys your project uses.
2. Make sure your project's `auth.json` contains those `repo.magento.com` access keys.
3. Run:

   ```
   composer require ometria_inc/module-analytics
   ```

## If Composer installed this package from Packagist

Composer only falls back to Packagist when `repo.magento.com` does not offer the package to your credentials. This usually means one of:

- `auth.json` is missing (common in CI or container builds where it was not mounted);
- the access keys belong to a different Marketplace account from the one that acquired the extension (e.g. an agency account).

In that case Composer will report that this package is abandoned, and nothing will have been installed into `vendor/`. To fix it:

```
composer remove ometria_inc/module-analytics
```

then correct your `auth.json` and install again as above.
