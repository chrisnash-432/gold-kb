---
title: "Real yields and gold — the mechanism, the tenor, the nonlinearity"
aliases: [real yields, TIPS, opportunity cost, real rates]
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
tags: [gold, real-yields, TIPS, mechanism]
---

# Real yields and gold

## The mechanism

Gold pays no coupon and costs money to store and insure. The cost of holding it is therefore the **real** yield forgone on the nearest risk-free alternative, because gold's own expected nominal return already carries expected inflation. A nominal yield rise driven purely by higher inflation expectations should leave gold roughly unaffected or help it; a rise driven by higher real yields should hurt it `[corroborated · high · src: raw-research-gold-drivers-2026-09-19#§6.1]`.

**This is why regressing gold on nominal yields produces an unstable, frequently wrong-signed coefficient.** The nominal yield is approximately TIPS plus breakeven, the two coefficients have opposite signs, and the breakeven coefficient is about 2.5x larger in absolute terms. Which one dominates depends on the sample `[inferred · high · src: raw-research-gold-drivers-2026-09-19#§6.1]`.

## The nonlinearity that changes the interpretation of everything

Jermann (NBER WP 31386, June 2023) builds a no-arbitrage model with investors and users and finds gold's sensitivity to 10y real yields is **strongly nonlinear**: elasticity roughly **19.3** in the bottom third of the rate distribution versus roughly **4.7** when rates are high `[asserted · moderate · src: raw-research-gold-drivers-2026-09-19#§3.5]`.

Same paper: expected gold price ≈ **3.8x** the value users alone would pay, so investment demand is more than two thirds of gold's value. Interest rate changes account for roughly **26%** of unconditional annual gold volatility (model-implied 4.3% against actual 14.8%) `[asserted · moderate · src: raw-research-gold-drivers-2026-09-19#§3.5]`.

This matters enormously for [[gold-regime-break-2022-2026]]. Jermann gives a theoretical reason why the relationship should weaken in a high-rate regime **without any structural break at all**. It is a competing explanation to the de-dollarisation story and it is rarely cited alongside it `[inferred · moderate · src: raw-research-gold-drivers-2026-09-19#§4.5]`.

## Tenor: 10y by convention, never tested

Every credible source uses the **10-year TIPS yield**: PIMCO, Erb and Harvey, RBC, Murenbeeld, the Chicago Fed, the Malta dissertation, and WGC's GRAM `[corroborated · high · src: raw-research-gold-drivers-2026-09-19#§6.2]`.

The theoretical case for 10y is that gold is a perpetual, zero-coupon, non-maturing claim, so the relevant discount rate is long-dated. The case for the front end is that the marginal holder is often a levered futures or ETF position financed at the short rate.

**No published research formally tests 2y against 10y real yields as competing gold inputs with comparative fit statistics** `[unverified · low · src: raw-research-gold-drivers-2026-09-19#gaps]`. Every source uses 10y by convention without testing the choice. Queued in [[_ingest-queue]] as candidate original work: we already have the data to settle it.

## The live hypothesis worth knowing about

State Street (Sept 2026) notes bond term premia across the US, UK, Germany and France reached their highest since 2011, driven by fiscal imbalances rather than growth, and argues this "strengthens gold's hedge appeal despite higher yields" `[asserted · moderate · src: raw-research-gold-drivers-2026-09-19#§6.2]` [single-source].

If that is right, the long-end real yield is **no longer a clean opportunity-cost signal**, because a term-premium-driven rise in the 10y real yield is simultaneously a rise in the sovereign risk gold hedges. That would make the "breakdown" a measurement problem rather than a behavioural one. As far as the research could establish, **untested** `[inferred · low · src: raw-research-gold-drivers-2026-09-19#§6.2]`.

## Related
[[gold-price-drivers]] · [[gold-regime-break-2022-2026]] · [[dollar-indices-for-gold]] · [[central-bank-demand-and-de-dollarisation]]
