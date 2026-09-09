# FIFE Landing Page Changelog

## 2026-09-03 — Structured data (JSON-LD SoftwareApplication)
- Added Schema.org `SoftwareApplication` JSON-LD in the `<head>` with:
  - `name`, `alternateName`, `applicationCategory` (LifestyleApplication), `operatingSystem` ([iOS, Android])
  - `description`, `image`, `url`, `downloadUrl` (App Store + Google Play)
  - `author` and `publisher` as Organization with `logo` and `sameAs` (Instagram, TikTok)
  - `offers` with `price: 0`, `priceCurrency: GBP`, and note about optional Creator subscription
  - `featureList` array covering Discover, UCHE, Library, Feed, and shopping lists
- Added Schema.org `WebSite` JSON-LD for the landing page itself with `name`, `url`, `description`, and `publisher` linkage.
- Both schemas are wrapped in `@graph` under a single `application/ld+json` script for clean, valid structured data.
- Note: `landing/index.html` has moved to `fife-site/index.html` (GitHub Pages deployment root).

