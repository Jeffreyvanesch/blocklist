# Changelog

All notable changes to this filter list are documented here.
This project follows a **practical, not pedantic** versioning style.

---

## [Unreleased]
### Added
- Scoped Google reliability telemetry, mobile ad metadata, app event collection, and Nexthink tenant telemetry rules.
- Intentional mobiletelemetry.ebay.com important allow rule.

### Changed
- Retired the obsolete Ziggo DNS-suffix mirror and corrected setup documentation.
- Removed the static.xx.fbcdn.net custom block because it serves Facebook interface assets.
- Removed the mayberryhomes.com apex block because it hosts legitimate home-builder content.
- Preserved intentional advertising, analytics, tracking, and allow rules, including existing duplicates pending review.

## [2025-12-12]
### Added
- Geo-independent Amazon Sponsored Ads blocking
  - `amazon-adsystem.com`
  - `axp.amazon-adsystem.com`
  - `/sspa/click` (including `/-/<lang>/sspa/`)
- Vendor-grouped sections (Amazon, Meta, TikTok, ISP)
- Explicit Ziggo / UPC / Horizon TV allow rules
- Consolidated legacy `hosts.txt` entries into DNS rules

### Changed
- Deduplicated Amazon ad domains already covered by core rules
- Moved advertising domains (e.g. `umbelderke.nl`) into Ads section
- Simplified Ziggo / UPC CDN handling via wildcard allows

### Removed
- Redundant per-host CDN entries now covered by wildcard rules
- Conflicting legacy allow rules punching holes in ad blocking

---

## [Initial]
- First public release of the curated master filter list