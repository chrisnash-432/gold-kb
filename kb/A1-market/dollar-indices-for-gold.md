---
title: "Dollar indices for gold work — why DXY is the wrong one"
aliases: [DXY, Dixie, dollar index, BBDXY, broad dollar index]
type: concept
node_kind: concept
status: active
domain: gold
source: research-ingest 2026-09-19
confidence: high
last_verified: 2026-09-19
generated_by: research-ingest@v2
derived_from: [raw-research-gold-drivers-2026-09-19, raw-malek-convo-2026-09-19]
raw_ref: raw-research-gold-drivers-2026-09-19
valid_from: 2026-09-19
review_by: 2027-09-19
tags: [gold, dollar, DXY, data-choice]
---

# Dollar indices for gold work

## Why this node exists

On the 2026-09-19 call Malek described DXY as "a correlated asset that basically reflects six or seven different interactions of price that give a strong indication of dollar strength or weakness", and named it as a candidate input to the app and to his bots `[asserted · high · src: raw-malek-convo-2026-09-19#@00:23:00]`.

The description is accurate as far as it goes. The problem is what those six currencies are.

## What DXY actually is

Administered by ICE. Base March 1973 = 100. Six currencies `[corroborated · high · src: raw-research-gold-drivers-2026-09-19#§5.1]`:

| Currency | Weight |
|---|---|
| **EUR** | **57.6%** |
| JPY | 13.6% |
| GBP | 11.9% |
| CAD | 9.1% |
| SEK | 4.2% |
| CHF | 3.6% |

**The basket has been changed exactly once since 1973**, when legacy European currencies were folded into the euro in 1999. The weights encode 1973 trade patterns `[corroborated · high · src: raw-research-gold-drivers-2026-09-19#§5.2]`.

**China, Mexico, South Korea, India, Taiwan and Brazil are entirely absent.** Sweden and Switzerland remain `[corroborated · high · src: raw-research-gold-drivers-2026-09-19#§5.2]`.

To a first approximation DXY is an inverted EUR/USD chart with a yen overlay `[inferred · high · src: raw-research-gold-drivers-2026-09-19#§5.2]`.

## What to use instead

**Federal Reserve Broad Dollar Index (H.10), FRED series `DTWEXBGS`.** 26 economies, weights from bilateral trade shares, revised annually. 2026 top weights `[asserted · high · src: raw-research-gold-drivers-2026-09-19#§5.3]`:

Euro Area 21.0% · Mexico 14.8% · Canada 12.8% · China 10.9% · UK 5.2% · Japan 5.2% · Korea 3.6% · India 3.4% · Taiwan 3.0% · Switzerland 3.0%

**Bloomberg US Dollar Spot Index (BBDXY).** 12 currencies, 50% trade weight and 50% BIS FX turnover, rebalanced annually at end-June. Contains CNH (7.0%) and MXN (9.8%) `[asserted · moderate · src: raw-research-gold-drivers-2026-09-19#§5.3]`.

The contrast: euro 21.0% versus 57.6%; Mexico 14.8% versus 0%; China 10.9% versus 0%; Sweden 0.6% versus 4.2% `[inferred · high · src: raw-research-gold-drivers-2026-09-19#§5.3]`.

## The practical rulings for this project

1. **Do not use DXY as the dollar input to the research engine.** Use the Fed broad index (free on FRED) for analysis `[inferred · high · src: raw-research-gold-drivers-2026-09-19#§5]`.
2. **Do keep DXY for the trading layer if Malek's bots trade it**, because DXY has a liquid futures and CFD market and the broad index does not. The two uses are different and should not be conflated `[inferred · moderate · src: raw-research-gold-drivers-2026-09-19#§5.3]`.
3. **Check which index a study used before comparing dollar betas.** The WGC's own benchmark model uses the Fed broad index. Murenbeeld used a three-currency index, narrower even than DXY. Comparing betas across studies without checking is a category error `[inferred · high · src: raw-research-gold-drivers-2026-09-19#§5.3]`.

This is a good example of the kind of correction the app can make that a retail trader would not: same concept, better instrument, free data.

## Related
[[gold-price-drivers]] · [[real-yields-and-gold]] · [[malek]] · [[bot-integration-layer]]
