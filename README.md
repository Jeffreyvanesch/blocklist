A curated, vendor-aware DNS filtering list for AdGuard Home, AdGuard DNS, and uBlock-compatible engines.

This list focuses on blocking advertising, tracking, and sponsored content infrastructure while explicitly allowing ISP and platform backends required for services such as Ziggo / UPC / Horizon TV.

✨ Design Goals

Readable & maintainable

Vendor-grouped (Amazon, Meta, TikTok, Google, Microsoft, etc.)

DNS-safe (no cosmetic rules unless explicitly marked)

ISP-aware (required Ziggo / UPC services explicitly allowed)

Minimal overblocking

Works alongside AdGuard default filters (no duplication wars)

🔧 Supported Engines

✅ AdGuard Home

✅ AdGuard DNS

✅ uBlock Origin (network rules only)

❌ Not intended as a cosmetic-only filter

📌 What This List Blocks

Amazon Sponsored Ads

amazon-adsystem.com

aax-* ad infrastructure

/sspa/click sponsored redirects (geo-independent)

Meta (Facebook / Instagram)

Ad delivery, tracking, SDK endpoints

Specific Meta advertising and tracking hostnames

TikTok Ads & Analytics

Ads, analytics, logging endpoints

Specific TikTok advertising and tracking hostnames

Legacy Ad / Tracking Networks

DoubleClick, Outbrain, Adnxs, Criteo, etc.

Converted from older hosts.txt format

🧩 What This List Explicitly Allows

Ziggo / UPC / Horizon TV

Platform backends (dmdsdp.com, ziggogo.tv)

CDN and API endpoints

Feedback / UX tooling

Mopinion

Usabilla

Required vendor backends

Microsoft (MSN / telemetry used by ISP apps)

Nuance speech services

All allows are marked with $important

🚫 What This List Does NOT Do

❌ Cosmetic hiding (Amazon tiles, Reddit promoted posts)

❌ UI element removal

❌ Replacement for AdGuard default DNS filters

❌ IP-based blocking

Note: Cosmetic issues (e.g. Instagram GIFs, Reddit ads) should be handled by uBlock Origin cosmetic rules, not DNS.

🧠 Recommended Setup
AdGuard Home / DNS

✅ AdGuard DNS filter (default)

✅ AdAway / mobile hosts filter

✅ This master list

Browser

uBlock Origin (or AdGuard extension)

Cosmetic filters for:

Amazon Sponsored blocks

Reddit Promoted posts

Instagram embeds

🔄 Update Strategy

This list is manually curated

Focuses on structural ad infrastructure, not churn domains

Updated when:

Vendors change ad routing (e.g. Amazon /sspa)

ISP behavior changes

Real-world breakage is observed

The obsolete Ziggo DNS-suffix mirror (master-ziggoNL.txt) has been retired. Use blocklist.txt.
