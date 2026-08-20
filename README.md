# vps-pricing-data

![Last verified](https://img.shields.io/badge/last%20verified-2026--08--11-brightgreen)
![License](https://img.shields.io/badge/license-CC%20BY%204.0-blue)
![Plans](https://img.shields.io/badge/plans-16-lightgrey)
![Providers](https://img.shields.io/badge/providers-13-lightgrey)

Hand-collected pricing data for 16 VPS, cloud, and managed hosting plans across 13 providers: first-term price, required prepay term, month-to-month price, renewal price, and whether backups, staging, and email are included in the base plan.

Maintained by [VPS Hosting Radar](https://vpshostingradar.com/vps-pricing-index/). Re-verified monthly.

## Key findings (2026-08-11)

- Renewal increases across the 16 plans range from **0% to 502%**.
- **Eight of 16 plans never raise prices at renewal.** For usage-billed infrastructure this falls out of the billing model; for two managed hosts it appears to be a deliberate choice.
- **The advertised price is a prepayment price.** SiteGround advertises $2.99/mo, but the same plan billed month-to-month is $24.99 — 8.4x, before any renewal exists.
- Reaching the lowest advertised rate can require prepaying up to **48 months** ($383.52 upfront in one case).
- **The managed-platform layer roughly doubles the bill** versus renting the same instance directly: a DigitalOcean 4 GB / 2 vCPU instance is $24/mo direct and $54/mo through Cloudways on the premium CPU tier.
- Counterintuitively, the plan with the most aggressive prepayment demand has the **lowest three-year total cost** ($287.64), because a 48-month commitment outruns a three-year window entirely.

## Why this exists

Hosting prices are deliberately hard to compare: introductory rates gated behind 12-to-48-month prepayment terms, renewal rates that are not shown until checkout, and "included" features that turn out to be paid add-ons. This dataset records what each provider actually charges, in one normalised table.

## Files

- `pricing.csv` — the full dataset
- `CHANGELOG.md` — what changed each month

## Methodology

Figures were collected manually from provider pricing and checkout pages on 11 August 2026, in USD, targeting the plan closest to 2 vCPU / 4 GB RAM at each provider. Where that configuration is not offered, the provider's most-promoted entry plan is used and the actual specification is noted.

Renewal rates were read from the pricing card where the provider prints one, and otherwise from the checkout flow or the provider's terms.

A dated screenshot of every pricing page is published alongside the table at
<https://vpshostingradar.com/vps-pricing-index/#evidence>

## Known limitations

Published with the gaps visible rather than smoothed over.

- Contabo is priced in euros with VAT included and is excluded from USD comparisons.
- WP Engine does not publish a renewal rate; that figure is provisional.
- Cloudways is recorded on the premium CPU tier; the standard tier is lower and not yet captured.
- RackNerd publishes separate monthly catalog and annual promotional pricing; this dataset uses the monthly catalog rate.
- Backup add-on pricing is incomplete for Linode, Liquid Web, InMotion, Kamatera, and RackNerd.
- Linode/Akamai pricing varies by region; figures reflect North American rates.
- Three plans ship 8 GB rather than the 4 GB baseline; they are comparable on pricing behaviour, not hardware.

## Licence

Free to use, including commercially, under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Attribution appreciated:

> VPS Hosting Radar, "VPS Pricing Index," last verified 11 August 2026. <https://vpshostingradar.com/vps-pricing-index/>

## Corrections

Spot an outdated or wrong number? [Open an issue](https://github.com/vpshostingradar/vps-pricing-data/issues) — errors are verified and fixed within 48 hours, and the change is recorded in `CHANGELOG.md`.
