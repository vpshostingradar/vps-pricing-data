# vps-pricing-data

Hand-collected pricing data for 16 VPS, cloud, and managed hosting plans across 13 providers: first-term price, required prepay term, month-to-month price, renewal price, and whether backups, staging, and email are included in the base plan.

Maintained by [VPS Hosting Radar](https://vpshostingradar.com). Re-verified monthly.

## Why this exists

Hosting prices are deliberately hard to compare: introductory rates gated behind 12-to-48-month prepayment terms, renewal rates that are not shown until checkout, and "included" features that turn out to be paid add-ons. This dataset records what each provider actually charges, in one normalised table.

Renewal increases in the current release range from 0% to 502%.

## Files

- `pricing.csv` — the full dataset
- `CHANGELOG.md` — what changed each month

## Methodology

Figures were collected manually from provider pricing and checkout pages on 11 August 2026, in USD, targeting the plan closest to 2 vCPU / 4 GB RAM at each provider. Where that configuration is not offered, the provider's most-promoted entry plan is used and the actual specification is noted.

Renewal rates were read from the pricing card where the provider prints one, and otherwise from the checkout flow or the provider's terms.

A dated screenshot of every pricing page is published alongside the table at
<https://vpshostingradar.com/vps-pricing-index/#evidence>

## Known limitations

- Contabo is priced in euros with VAT included and is excluded from USD comparisons.
- WP Engine does not publish a renewal rate; that figure is provisional.
- RackNerd publishes separate monthly catalog and annual promotional pricing; this dataset uses the monthly catalog rate.
- Backup add-on pricing is incomplete for Linode, Liquid Web, InMotion, Kamatera, and RackNerd.
- Linode/Akamai pricing varies by region; figures reflect North American rates.

## Licence

Free to use, including commercially, under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Attribution appreciated:

> VPS Hosting Radar, "VPS Pricing Index," last verified 11 August 2026. https://vpshostingradar.com/vps-pricing-index/

## Corrections

Spot an outdated or wrong number? [Open an issue](../../issues) — errors are verified and fixed within 48 hours, and the change is recorded in `CHANGELOG.md`.
