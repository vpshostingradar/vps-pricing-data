# vps-pricing-data

Hand-collected pricing data for 12 popular VPS and managed cloud hosting providers: first-term price, required prepay term, renewal price, and add-on costs (backups / staging / email).

Maintained by [VPS Hosting Radar](https://vpshostingradar.com) — scenario-first hosting comparisons. Re-verified monthly.

## Why this exists

Hosting prices are deliberately hard to compare: intro rates gated behind 36-month prepay terms, silent renewal jumps, and "features" that turn out to be paid add-ons. This dataset records what each provider actually charges, in one normalized table.

## Files

- `pricing.csv` — the full dataset
- `CHANGELOG.md` — what changed each month

## Methodology

All prices are collected manually from each provider's public pricing and checkout pages, in USD, for the entry plan closest to 2 vCPU / 4 GB RAM (or the provider's most-promoted entry plan where specs differ). "First-term price" is the advertised rate with its required prepay term noted; "renewal price" is the rate shown at checkout or in the provider's terms for subsequent terms.

## License

Free to use with attribution (CC BY 4.0). Please link to https://vpshostingradar.com when using this data.

## Corrections

Spot an outdated number? Open an issue — errors are fixed within 48 hours.
