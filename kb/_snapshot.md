---
title: "gold-kb — _snapshot"
type: _snapshot
status: active
created: 2026-09-19
updated: 2026-09-19
domain: gold
---

# Gold Desk — _snapshot (2026-09-19)

**What this domain is.** Malek is building an AI macroeconomic research tool for retail gold traders. Chris is **advisor and thinking partner, not co-founder**; Malek drives. Originated in a recorded brainstorm on 12 September 2026. Working name in the plan: **Macro Surprise Engine**.

**What has been built.** A Stage 0 event-study engine over 24 release families against a 3.3 GB gold tick archive; a mobile-ready five-tab prototype; a methodology assessment; and a handover review pack with a 13-question survey. All published as artifacts. See [[gold-desk-prototype]].

**The headline result, which is ours and not anyone else's.** Pooled surprise effect **t = 10.55 at one minute**, within-R² decaying **6.97% → 6.30% → 3.77% → 1.35% → 0.68%** across 1min / 15min / 1hr / 4hr / close. Out of sample **+4.1% and +3.2%** at the two shortest horizons, **−2.0% and −2.4%** at 1 and 4 hours, **+0.4%** to the close. Payrolls explains **38.2% at 15 minutes** against a 4.7% noise floor on n = 82 (Advance GDP scores higher on n = 28, too small to headline). Eleven of 24 releases survive false-discovery correction, clustering tightly in **labour, inflation and consumption**. The crude-oil placebo came back null. See [[macro-surprise-engine-findings]].

**The tradeable window is the first minutes**, where the relationship generalises out of sample; it fails at 1 and 4 hours and is weakly positive again to the close. That is a design constraint and it sharpens the product rather than shrinking it.

**Malek's positions, tested.** EMA21 as a modulator of event impact: **null** at 10, 21 and 50 days, sign reverses in the sealed holdout ([[ema21-hypothesis]]). Asymmetry: **null**. Spike-and-retest: **not supported in the literature as stated**, though Nagel's liquidity-provision result offers a better explanation of the same edge ([[spike-and-retest]]). DXY: concept right, instrument wrong, fix is free ([[dollar-indices-for-gold]]). Drawdown scaling: he is right at R below ~1.7 and wrong above it ([[position-sizing-and-drawdown-scaling]]). Central bank flow not yet tradeable: **correct**.

**The $15 business model does not survive the arithmetic.** FXStreet is $39.99 not $50; Investing.com already sells at an effective $8.95, and lower on longer terms; the Investing vertical supports the **highest** prices in the category ($27/month median) while the adjacent Money vertical shows the **worst** churn of any category (16.67% monthly); and customers leave because they stop trading, not because the price is too high. See [[business-model-hypothesis]].

**The most interesting development is new as of 19 September: using the research output as an on/off switch on Malek's bots** ([[bot-integration-layer]]). It avoids competing against free, sells at higher value per user, and can be validated against his own P&L. **No peer-reviewed study tests a macro on/off switch on a gold technical system and reports a profit factor.** We have the engine, the tick archive and a live bot. That is a better research position than any of the cited papers had.

**Three blocking verifications** before anything reaches a third party: the FSCA leverage and negative-balance-protection position; the date and case name of the FSCA signal-provider penalty; Trading Economics' real pricing. All in [[_ingest-queue]].

**Open action items from the 19 September call:** push this KB to a shared GitHub repo so Malek can connect his own AI; build a central control-centre dashboard across workstreams; ingest Malek's survey response or voice note when it arrives.

Read [[_index]] or [[gold-moc]] for routes. Claims carry per-source tags — trust the tags, not vibes. Two rules specific to this domain: **always state the frequency**, and **always state the trial count**. See [[_conventions]].
