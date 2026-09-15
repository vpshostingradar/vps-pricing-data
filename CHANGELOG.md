# Changelog


## 2026-09-15 — Monthly verification

Every plan re-checked by hand against vendor pricing and checkout pages.
Coverage expands to 19 plans across 15 providers.

**Method change**

Monthly and renewal rates are now recorded as a single figure: the price a plan
reverts to once its advertised introductory term ends. Previously these were two
columns. The practical effect is on SiteGround's shared StartUp plan, where the
advertised-to-post-term multiple is now stated as 6.0x ($2.99 to $17.99) rather
than 8.4x, which compared the advertised rate against the month-to-month rate.

**Corrections to our August data**

- InMotion: the figures previously published ($10.99 to $26.99) do not appear on
  the current VPS pricing page; $10.99 is a shared-hosting tier. The tracked SKU
  is the 4 vCPU / 8 GB VPS at $13.99 to $26.99 on a 24-month term, a 93%
  increase rather than 146%.
- Contabo: the August entry attributed EUR 4.40 to a 12-month term. It is the
  24-month VAT-inclusive effective rate, now recorded as EUR 5.28 against a
  EUR 6.60 list price. The row remains outside all USD comparisons.
- Hostinger: the tracked VPS row moves from KVM 2 (8 GB) to KVM 1 (4 GB), which
  is closer to the 2 vCPU / 4 GB baseline, and the tracked shared row moves from
  Cloud Startup to Web Premium.

**Rows added**

- SiteGround Cloud Jump Start (4 CPU / 8 GB / 40 GB), $100/mo, list pricing.
- Cloudways Autonomous Growth, $99/mo, list pricing.
- ScalaHosting Unmanaged Config #1, $19.95 to $24.95.

**Promotional pricing**

Two plans currently carry one-time introductory offers that the table excludes
by rule and records in a new `Promo` column: Kinsta is giving away the first
month on Single 20 GB, and Rocket.net continues to offer a $1 first month on
Starter. Both rows carry the ongoing rate, $35 and $30 respectively. A $0
advertised rate would make a percentage increase undefined, which is the reason
the rule exists.

**Coverage added**

Backup add-on pricing and included-feature data are now recorded for RackNerd,
Linode, Vultr, ScalaHosting, InMotion, and SiteGround. Source URLs are present
for all 19 rows. Two new columns: `Promo` and `Notes`.

**Still open**

- WP Engine does not publish a renewal rate. The plans page footer states that
  product renewal pricing is subject to change, so the $35 figure carries a
  provisional marker.
- RackNerd's annual special ($59.99/year for 3 vCPU / 60 GB / 7 TB, about
  $5.00/mo) has no stated renewal terms on the specials page or in the terms of
  service, so the table continues to track the monthly catalog rate of $24.59.
- Cloudways was captured on the Micro tier (2 GB / 1 vCPU) this cycle rather
  than the 4 GB baseline. The $54 premium-tier figure is carried forward from
  the 11 August capture, and the managed-layer premium remains stated as an
  approximation rather than a single percentage.
  

## 2026-08-11 — Initial release

First dataset published: 16 plans across 13 providers, covering raw VPS, platform-managed, and premium managed WordPress tiers.

Fields include first-term price, required prepay term, month-to-month price, renewal price, renewal increase, 36-month total cost, and whether backups, staging, and email are included in the base plan.

All figures collected manually from provider pricing and checkout pages on 2026-08-11. Source URL recorded per row. Dated screenshots of every pricing page published at https://vpshostingradar.com/vps-pricing-index/#evidence

Notes on this release:

- Contabo listed but excluded from USD comparisons (euro pricing, VAT included).
- WP Engine renewal rate marked provisional — not published by the vendor.
- Cloudways recorded on the premium CPU tier; the standard tier is lower and will be added next cycle.
