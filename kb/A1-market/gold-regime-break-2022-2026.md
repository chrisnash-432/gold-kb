---
title: "The 2022-2026 regime break in gold"
aliases: [regime break, gold regime change, correlation breakdown, 84 to 3]
type: concept
node_kind: concept
status: active
domain: gold
source: research-ingest 2026-09-19
confidence: high
last_verified: 2026-09-19
generated_by: research-ingest@v2
derived_from: [raw-research-gold-drivers-2026-09-19, raw-research-central-banks-2026-09-19]
raw_ref: raw-research-gold-drivers-2026-09-19
valid_from: 2026-09-19
review_by: 2027-03-19
tags: [gold, regime, structural-break, evidence]
---

# The 2022-2026 regime break

Malek's framing on the 2026-09-19 call was that "gold has doubled in value in the last four years, the market regime has changed, we are in a new regime" `[asserted · high · src: raw-malek-convo-2026-09-19#@00:30:30]`. On this he is right, and the evidence is stronger than he probably knows.

## The headline number

RBC Wealth Management, **weekly** gold against 10y TIPS yields `[asserted · moderate · src: raw-research-gold-drivers-2026-09-19#§4.1]` [single-source]:

| Sub-period | R² |
|---|---|
| 1997-2004 | 69% |
| 2005-2021 | **84%** |
| 2022-2023 | **3%** |
| 2024 to Jun 2025 | 7% |

**84% to 3%, weekly.** The single most citable figure in the instability case, and three things must travel with it or it becomes misleading `[inferred · high · src: raw-research-gold-drivers-2026-09-19#§4.1]`:

1. **It is weekly.** Quote the frequency or do not quote the number.
2. **84% is a peak, not a baseline.** The same table gives 69% for 1997-2004 and 7% for 2024 onwards. The relationship was already weaker before, and has partly recovered since.
3. **It is one bank's wealth-management note.** Not primary, not replicated. The corroboration below is qualitative, not numerical.

## Qualitative corroboration from a central bank

The ECB confirms that a breakdown happened. **It does not corroborate the 84%/3% figures**, and publishes no quantitative decomposition of its own.

The ECB, in the *International Role of the Euro* report, June 2025, directly: "Between 2008 and early 2022, gold prices were negatively correlated with real yields... This correlation broke down after Russia's full-scale invasion of Ukraine, suggesting that gold prices have been influenced by other factors, such as geopolitical risk" `[corroborated · high · src: raw-research-gold-drivers-2026-09-19#§4.2]`.

Supporting: central banks took **over 20% of global gold demand in 2024** against roughly 10% on average in the 2010s; Türkiye, India and China jointly added more than 600 tonnes since end-2021. And the detail that does the most explanatory work: **"in five of the ten largest annual increases in the share of gold in foreign reserves since 1999, the countries involved faced sanctions in the same year or the previous year"** `[asserted · high · src: raw-research-gold-drivers-2026-09-19#§4.2]`.

## Academic confirmation, with a different break date

Demajo (University of Malta dissertation, Sept 2025), monthly VAR with DXY control `[asserted · low · src: raw-research-gold-drivers-2026-09-19#§4.3]` [single-source, supervised masters dissertation, not refereed]:

| Period | TIPS(-1) coefficient | Significance | Model R² |
|---|---|---|---|
| 2010-2019 | -0.0660 | t ≈ -3.92 | 0.325 |
| 2020-2024 | -0.0153 | **insignificant** | 0.280 |

**This dates the break to 2020. The ECB and RBC date it to early 2022. That disagreement is unresolved and is itself a finding** `[contested · moderate · src: raw-research-gold-drivers-2026-09-19#§4.3]`.

## The counter-evidence that should stop this becoming dogma

Two things cut against a strong structural-break reading `[inferred · moderate · src: raw-research-gold-drivers-2026-09-19#§4.5]`:

1. **Jermann's nonlinearity.** The gold/real-rate elasticity is roughly 4x weaker at high rate levels for purely structural reasons. 2022-2026 was a high-rate regime. Some, possibly much, of the measured breakdown may be nonlinearity rather than regime change. See [[real-yields-and-gold]].
2. **It has wandered before.** Murenbeeld, writing in 2018, already observed gold and the 10y TIPS yield "parting ways since late 2017", long before Ukraine.

**The honest reading: the relationship is real, sign-stable, and unstable in magnitude, with the instability occasionally total for multi-year stretches** `[inferred · high · src: raw-research-gold-drivers-2026-09-19#summary]`.

## Why this matters more than it looks

It is a direct argument for the product, and a direct argument against one version of the product.

- **For:** if a relationship that held at 84% can go to 3%, a tool that re-estimates continuously and tells the user when a relationship has stopped working is genuinely valuable. Nothing on the retail market does that.
- **Against:** it means any model shipped with fixed coefficients will be wrong within a few years and will not announce it. Whatever we build must carry its own expiry date. See [[macro-surprise-engine-findings]] for how our engine already handles this with a sealed holdout.

## Market context for reading any of the above
Gold spot $4,383.45/oz on 18 Sep 2026, up ~19% YoY. All-time high $5,608.35 set January 2026, so roughly a 22% drawdown by September `[asserted · moderate · src: raw-research-gold-drivers-2026-09-19#§0]`. **Any correlation estimate ending before 2026 has not seen that round trip.**

## Related
[[real-yields-and-gold]] · [[gold-price-drivers]] · [[central-bank-demand-and-de-dollarisation]] · [[macro-surprise-engine-findings]] · [[volatility-filters-and-macro-overlays]]
