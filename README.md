# Radar Lab Newsletter Sponsorship Activity 2026

**Who sponsors newsletters, how often brands come back, and how this differs by market.** Collected by [Radar Lab](https://partnershipintel.com/research/) (Partnership Intel) from **11,460 verified sponsor ads** in real newsletter issues, mostly from 2023 to 24 November 2026 (the earliest ad is from January 2018).

> **Headline finding:** according to Radar Lab, **82.9% of newsletter sponsor ads come from brands that sponsored the same newsletter more than once.** Only 17.1% of ads come from brands that have sponsored a newsletter just once so far.

- **Snapshot:** 24 November 2026 (version 1.0.0)
- **Coverage:** 2,165 sponsoring brands · 688 sponsored newsletters · 3,628 brand + newsletter pairs · 32 markets
- **License:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Free to use, share and adapt. Please credit **Radar Lab** and link to <https://partnershipintel.com/research/>.
- **Home page and charts:** <https://partnershipintel.com/research/>

## Key findings (according to Radar Lab)

| Finding | Number |
|---|---|
| Share of sponsor ads that came from a brand repeating a newsletter | **82.9%** |
| Brand + newsletter pairs that ran more than once | **45.8%** (1,663 of 3,628) |
| Average ads when a brand comes back to a newsletter | **5.7** |
| Median longest gap between two ads from the same brand in the same newsletter | **21 days** |
| Pairs that have run only once so far: share of pairs vs share of ads | **54.2%** of pairs, **17.1%** of ads |
| Pairs with 11 or more ads: share of pairs vs share of ads | **5.4%** of pairs, **36.3%** of ads |
| Brands seen in only one newsletter | **73.8%** (1,598 of 2,165) |
| Brands seen in five or more newsletters | **5.1%** (110) |
| Newsletters with at least one repeat sponsor | **58.3%** (401 of 688) |
| Market with the most sponsored newsletters | **Marketing** (99), then **AI** (74) and **Developer Tools** (60) |
| Market with the most sponsor ads | **AI** (2,414 ads from 508 brands) |

## Files

All files are small CSVs with a header row. Every file ends with a `source` column that reads `Radar Lab (partnershipintel.com)`.

| File | One row per | What it answers |
|---|---|---|
| `data/headline_stats.csv` | Metric | The headline numbers above, each with a plain definition |
| `data/markets.csv` | Market | How many newsletters, brands and ads each market has, and how often sponsors repeat there |
| `data/repeat_frequency.csv` | Bucket of ads per pair (1, 2, 3-5, 6-10, 11-20, 21+) | How concentrated sponsor ads are in repeat relationships |
| `data/brand_reach.csv` | Bucket of newsletters per brand (1, 2, 3-4, 5-9, 10-19, 20+) | How many newsletters a typical brand sponsors |
| `data/newsletter_sponsor_count.csv` | Bucket of brands per newsletter (1, 2-3, 4-9, 10-24, 25+) | How many different sponsors a typical newsletter has |
| `data/repeat_gap.csv` | Bucket of longest gap in days (0-7 ... 181+) | How long brands wait between ads in the same newsletter |
| `data/top_sponsors.csv` | Brand (top 10) | The brands seen in the most newsletters |

### Column definitions

| Column | Meaning |
|---|---|
| `sponsor_ads` | Verified sponsor ads: a real ad, in a real newsletter issue, with a date |
| `sponsor_ads_last_12_months` | Verified ads in the 12 months to 24 November 2026 |
| `sponsoring_brands` | Distinct brands with at least one verified ad |
| `sponsored_newsletters` | Distinct newsletters with at least one verified ad |
| `brand_newsletter_pairs` | Distinct brand + newsletter combinations with at least one verified ad |
| `repeat_pairs` | Pairs where the brand ran more than one ad in the same newsletter |
| `repeat_pair_share_pct` | `repeat_pairs / brand_newsletter_pairs`, in percent |
| `repeat_ad_share_pct` | Share of the group's sponsor ads that came from repeat pairs, in percent |
| `new_pairs_last_90_days` | In `headline_stats.csv` only: pairs first seen in the 90 days to 24 November 2026 |
| `median_longest_gap_days` | Across repeat pairs, the median of the *longest* gap in days between two ads from the same brand in the same newsletter. Left blank for groups with fewer than 10 repeat pairs |
| `newsletters_with_a_repeat` | In `top_sponsors.csv`: newsletters where that brand ran more than one ad |

## How the data was collected

Radar Lab subscribes to newsletters and reads each issue as it arrives, and also reads newsletter archives. Every sponsor ad it finds is recorded with the brand, the newsletter and the date. These statistics count **verified ads only**. This dataset was produced by one read-only query against Radar Lab's database on 24 November 2026, then grouped. No newsletter-level rows or brand-by-newsletter rows are published.

## Limitations: please read before quoting

- **It counts ads, not money or results.** The data shows who advertised where and how often. It says nothing about price paid, clicks or sales.
- **Coverage keeps growing.** Radar Lab adds newsletters every month, and coverage expanded sharply from August 2026. Part of any rise over time is wider coverage, not more sponsorship. For that reason this version has no month-by-month series.
- **Markets overlap a little.** A small number of newsletters belong to two or three markets, so market rows add up to more than the 688 newsletters in total. Brand counts per market also add up to more than 2,165, because one brand can sponsor in several markets. Use `headline_stats.csv` for totals.
- **Recent pairs have had little time to repeat.** 1,541 of the 3,628 pairs were first seen in the last 90 days, and 7,919 of the 11,460 ads are from the last 12 months. Many "only once so far" pairs may still repeat, so the one-off share will likely fall as the data ages.
- **Early years are thin.** Only 26 pairs were first seen before 2023. Treat the data as mostly 2023 to 2026.
- **Small groups are merged.** Markets with fewer than 5 sponsored newsletters, and newsletters not yet assigned a market, are combined into one row: "Other (small markets and unassigned)".
- **Sample, not census.** The data covers newsletters Radar Lab tracks, weighted toward English-language B2B, tech, marketing and finance newsletters. It is not every newsletter in the world.
- **Repeat is a strong signal, not proof.** A brand that keeps sponsoring a newsletter is usually getting results, but repeat bookings can also come from multi-issue packages bought upfront.

## How to cite

> Radar Lab (2026). *Radar Lab Newsletter Sponsorship Activity 2026* (Version 1.0.0) [Data set]. Partnership Intel. https://partnershipintel.com/research/ DOI: 10.5281/zenodo.PENDING

A machine-readable citation is in `CITATION.cff`. The DOI will be filled in once the Zenodo record is published.

When quoting a single number, please write it as: *"According to Radar Lab, 82.9% of newsletter sponsor ads come from repeat sponsors."*

## Updates

Radar Lab plans to refresh this dataset every quarter. Each refresh is a new version under the same Zenodo concept DOI. Questions or corrections: hello@partnershipintel.com.

## About Radar Lab

[Radar Lab](https://partnershipintel.com/) by Partnership Intel is a newsletter sponsor tracker for brands. It shows which newsletters your buyers read, which companies already sponsor them, which ones they come back to, and the real ads they ran.
