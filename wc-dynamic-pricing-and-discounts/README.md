# WooCommerce Dynamic Pricing & Discounts — Community Maintenance

Version: 2.5.6  
Date: 2026-01-02

## Summary
- Maintained plugin without altering original functionality.
- Removed non-functional update/licensing mechanisms and broken external links.
- Strengthened compatibility: PHP 8.2+, WooCommerce HPOS.
- Updated metadata: WP tested 6.9; WC requires 9.0; WC tested 10.4.3.
- Assets update: Select2 updated to 4.1.0-rc.0 via CDN; jQuery UI CSS remains 1.13.2.
- UX: removed “Loading user interface” preloader on settings pages to prevent flickering.
- PHP 8.2 compatibility: avoid deprecation notices (string cast in `htmlspecialchars`), translations loading moved to the `init` hook, settings initialization also moved to `init`.
- Visual tweaks:
  - Inputs and selects on settings pages standardized to 34px height for visual consistency.
  - Textareas kept at 46px minimum height (two lines) by default.
  - Select2/selectWoo multiple: consistent visual alignment (container 34px; inline search margin tuned; choice chip vertical offset).

## Compatibility
- WordPress 6.5+ (tested up to 6.9)
- WooCommerce 9.0+ (tested up to 10.4.3)
- PHP 8.0+ (optimized for 8.2+)
- Declared HPOS compatibility

## Installation / Upgrade (Replacing the Original Plugin)
To replace the original plugin without any CLI:
- Download the ZIP from GitHub Releases named `wc-dynamic-pricing-and-discounts.zip`.
- This ZIP already contains the correct root folder `wc-dynamic-pricing-and-discounts`.

Steps (WP Admin):
1. Backup your site.
2. In WordPress admin, go to Plugins → Add New → Upload Plugin.
3. Choose `wc-dynamic-pricing-and-discounts.zip` and click Install.
4. If prompted, confirm replacement/overwrite of the existing plugin.
5. Activate.

Alternative: the versioned ZIP (`wc-dynamic-pricing-and-discounts-<version>.zip`) in Releases works the same way.

Notes:
- Do not use GitHub’s “Source code (zip)” — it won’t have the correct plugin root folder.
- Repository name on GitHub does not affect WordPress installation; only the folder inside the ZIP matters.

## Repository Naming Guidance
- You can name the GitHub repository `wc-dynamic-pricing-and-discounts-by-dead-rightpress` to clarify community maintenance.
- For WordPress installation, only the root folder inside the distributed zip matters. Use `wc-dynamic-pricing-and-discounts` as the zip root folder to replace the original plugin cleanly.
- Keeping the plugin display name as-is avoids confusion in the WP admin list; documentation clarifies that this is a community-maintained fork.

## License / Credits
- Original author rights preserved; this package is community maintenance.
- No functional behavior changes, only maintenance and compatibility updates.
