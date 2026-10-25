# Scento Fragrance Index — European perfume decant demand (Oct 2025–Sep 2026)

The Scento Fragrance Index is Scento's open dataset of what Europe buys in perfume decants: the most-bought perfumes and houses overall, by country, by gender style, niche versus designer, decant size mix, price tiers and Middle Eastern houses, plus a quarter-by-quarter view.

- Source and homepage: https://www.scento.com/perfume-industry-statistics
- Quarterly edition with charts: https://www.scento.com/blog/scento-fragrance-index-quarterly
- Window: October 2025 to September 2026 (time zone Europe/Bucharest)
- Generated: 2026-10-08T07:49:26.509Z
- Publisher: Scento, https://www.scento.com

## Files

| File | Contents |
|---|---|
| `scento-fragrance-index.csv` | The full index as one long table, exactly as published at https://www.scento.com/data/scento-fragrance-index/latest.csv (406 rows) |
| `scento-fragrance-index.json` | The same index as published JSON (with the method text), https://www.scento.com/data/scento-fragrance-index/latest.json |
| `datapackage.json` | Frictionless Data descriptor |

CSV columns: `metric`, `group`, `key`, `label`, `rank`, `perfume`, `house`, `country`, `period`, `share`, `index`, `is_scento_house`, `suppressed`.

## Method

Scento analysis of its own paid orders placed between October 2025 and September 2026 (Europe/Bucharest time), shipped to customers across Europe. Every figure is a share, a rank or an index computed from perfume decants (0.75, 2, 5, 8 and 30 ml) that customers paid for.

Each decant unit a customer paid for counts once, whatever its size. Rankings order perfumes by decant units. Shares are each group’s part of all paid decant units in the window.

Excluded:
- Cancelled and deleted orders
- Orders without a captured payment, free PR and press kits, and replacement shipments for lost parcels
- Test, synthetic and staff orders, and orders placed by the Scento team
- Gift-card-only orders and gift-card lines
- Free items: welcome gifts, perks, rewards and promotional samples
- Full bottles, accessories (atomizer cases, eye patches) and pre-built gift sets that are not a single perfume
- Automatic shipments of the legacy per-perfume subscription, where the perfume could be assigned rather than chosen

Rounding: Shares are rounded to the nearest whole percent, or to the nearest half percent below 10%, so rounded shares need not add up to 100. Indices are rounded to whole numbers and computed from unrounded shares.

Suppression: Any figure that would rest on too few orders to be stable is withheld and shown as null; a ranked perfume must also clear a minimum number of separate orders, and a country’s top 10 is shown only when all ten places clear it.

Trend: Trend indices compare the second half of the window (April 2026 to September 2026) with the first half (October 2025 to March 2026) = 100. Quarterly indices use the first quarter that clears the order threshold as 100.

The index publishes shares, ranks and indices only, never order or unit counts.

## Licence and attribution

Creative Commons Attribution 4.0 International (CC BY 4.0), https://creativecommons.org/licenses/by/4.0/ — free to use with credit to Scento.

Cite as: Scento Fragrance Index, https://www.scento.com/perfume-industry-statistics, October 2025 to September 2026.
