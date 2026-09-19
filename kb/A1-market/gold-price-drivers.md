---
title: "Gold price drivers — what actually explains the move"
aliases: [gold drivers, what moves gold, canonical driver set]
type: concept
node_kind: concept
status: active
domain: gold
source: research-ingest 2026-09-19
confidence: high
last_verified: 2026-09-19
generated_by: research-ingest@v2
derived_from: [raw-research-gold-drivers-2026-09-19]
raw_ref: raw-research-gold-drivers-2026-09-19
valid_from: 2026-09-19
review_by: 2027-03-19
tags: [gold, drivers, macro, evidence]
---

# Gold price drivers

The canonical driver set is **real yields, the dollar, inflation expectations, and risk/uncertainty**, with growth and momentum added by the industry frameworks. The direction of each is settled. The magnitude is not, and the explained share depends almost entirely on the frequency you measure at.

## The single most important table in the evidence base

Chicago Fed, three specifications, same variables, same authors `[corroborated · high · src: raw-research-gold-drivers-2026-09-19#§1.1]`:

| Specification | Sample | R² |
|---|---|---|
| Annual **levels** (real gold on real world GDP, real 10y, inflation expectations, pessimism) | 1971-2019 | **0.87** (DW 0.98) |
| Quarterly **innovations** | 1971Q1-2021Q1 | **0.12** |
| **Daily changes** (10y TIPS + breakeven) | Jan 2003 - Feb 2021 | **0.012** |

The Durbin-Watson of 0.98 on the annual regression is the tell: heavy residual autocorrelation, trending series on trending series. It is not forecasting power `[inferred · moderate · src: raw-research-gold-drivers-2026-09-19#§1.1]`.

**The operative rule for this project.** Anyone quoting "real yields explain gold" without stating the frequency is quoting a different number from the one they think. Our tool operates at minutes to days. The relevant figure at that frequency is **roughly 1%**, not 87% `[inferred · high · src: raw-research-gold-drivers-2026-09-19#§7]`.

## Betas worth holding

- 100bp rise in 10y real yields historically associated with an **18% decline** in the inflation-adjusted gold price, an empirical "real duration" of about 18 years, over 2004-2025 (PIMCO) `[asserted · moderate · src: raw-research-gold-drivers-2026-09-19#§1.2]` [single-source]
- 13-week changes, 2014-2018, gold on 10y TIPS plus a 3-currency dollar index: **R² 0.65**; 100bp on the TIPS yield ≈ **-$173**; 1 point on the dollar index ≈ **-$10** (Murenbeeld, LBMA) `[asserted · moderate · src: raw-research-gold-drivers-2026-09-19#§1.2]` [single-source]
- Daily: TIPS coefficient **-0.011**, breakeven coefficient **+0.027**, both significant at 1%. Gold responds to breakevens roughly 2.5x more strongly than to real yields at high frequency `[corroborated · high · src: raw-research-gold-drivers-2026-09-19#§1.3]`
- Shorter horizon, quantified and tradeable: a 1% rise in TIPS yields is consistent with roughly **-$100/oz** on spot (UBP, May 2026) `[asserted · moderate · src: raw-research-central-banks-2026-09-19#§7.3]` [single-source]

## The industry frameworks, and the gap in them

The World Gold Council runs two tools that are routinely conflated `[corroborated · high · src: raw-research-gold-drivers-2026-09-19#§2]`:

- **GVF / Qaurum** — a forward-looking supply-demand equilibrium model, organised by demand sector. WGC states explicitly it "does not forecast gold price".
- **GRAM** — a return attribution model, roughly 15 underlying variables grouped into **five factors**: economic expansion; risk and uncertainty; opportunity cost (FX); opportunity cost (interest rates); momentum and trends. Opportunity cost is sometimes described as one category and sometimes split in two, which is why the literature refers to both four and five; **five is the form WGC's own published attributions use**.

The driver categories belong to **GRAM**, not to GVF. Conflating the two is the most common error in secondary commentary on WGC research.

**What GRAM says about H1 2026, on the gold industry's own model** `[asserted · moderate · src: raw-research-gold-drivers-2026-09-19#§7.1]`: momentum 24% of return variability, **unexplained residual 30%**, risk and uncertainty 17%, FX 14%, growth 12%, **interest rates 3%**. The most gold-favourable framework available concedes that the opportunity-cost channel is close to inert right now and that the largest single bucket is "we do not know".

**No independent critique or replication of Qaurum or the GVF exists in the peer-reviewed literature or in bank research, as far as repeated targeted searching can establish** `[unverified · low · src: raw-research-gold-drivers-2026-09-19#gaps]`. The only published evaluation was run by the WGC on its own model against a deliberately minimal benchmark. That is a finding, not a citation.

## Where this leaves the product

The honest framing for any explanatory figure the app shows: **it is a share of a very small explained total.** At the horizons a retail gold trader cares about, the published literature leaves most of the variance unexplained, and so does ours. See [[macro-surprise-engine-findings]] for what our own engine measured.

## Related
[[real-yields-and-gold]] · [[dollar-indices-for-gold]] · [[gold-regime-break-2022-2026]] · [[gold-safe-haven-and-inflation-hedge]] · [[gold-event-response]] · [[macro-surprise-engine-findings]] · [[world-gold-council]]
