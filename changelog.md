# Changelog

All notable changes to this filter list are documented here.
This project follows a **practical, not pedantic** versioning style.

---

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