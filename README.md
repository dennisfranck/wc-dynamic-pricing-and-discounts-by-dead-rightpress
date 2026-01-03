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

## Installation / Upgrade

**[Download Latest Version (ZIP)](https://github.com/dennisfranck/wc-dynamic-pricing-and-discounts-by-dead-rightpress/releases/latest/download/wc-dynamic-pricing-and-discounts.zip)**  
*(Use the link above. Do not use "Source code" from GitHub)*

**Steps:**
1. Go to **Plugins → Add New → Upload Plugin**.
2. Upload the downloaded ZIP file.
3. Click **Install Now**.
4. If prompted, confirm to **Replace current with uploaded**.

## Repository Naming Guidance
- You can name the GitHub repository `wc-dynamic-pricing-and-discounts-by-dead-rightpress` to clarify community maintenance.
- For WordPress installation, only the root folder inside the distributed zip matters. Use `wc-dynamic-pricing-and-discounts` as the zip root folder to replace the original plugin cleanly.
- Keeping the plugin display name as-is avoids confusion in the WP admin list; documentation clarifies that this is a community-maintained fork.

## License / Credits
- Original author rights preserved; this package is community maintenance.
- No functional behavior changes, only maintenance and compatibility updates.
