---
title: "gold-kb — Conventions"
type: conventions
status: active
created: 2026-09-19
updated: 2026-09-19
domain: gold
registers_into: "cosmos-kb › C3 › gold"
---

# gold-kb — Conventions

Inherits the portable PAIOS engine rules. Registers upward into **cosmos-kb C3 (Creation & Work)** at `C3 › gold`.
Scope: the gold macro research tool, its evidence base, and the trading, commercial and regulatory context around it.

## Routing spine (defined 2026-09-19, first ingest)
- `A1-market/` — how gold actually prices: drivers, regimes, event response, volatility
- `A2-signals/` — candidate signal families and what the evidence says about each
- `A3-product/` — the product itself: vision, prototype, features, the feedback loop
- `A4-trading/` — Malek's bots and the standards by which a trading claim should be judged
- `A5-commercial/` — market, competitors, pricing, data licensing, regulation
- `A6-raw-register/` — raw sources, manifest, methods notes
- `people/` + `organisations/` — entity axes (role data only; POPIA)

## Claim tagging
Every material claim carries an inline tag: `[status · grade · src: raw-slug#locator]` per research-ingest@v2.

- **status** — `asserted` (one source says so), `corroborated` (two independent sources or a primary), `inferred` (our reasoning, not stated anywhere), `contested` (sources disagree), `unverified` (we could not check it).
- **grade** — `high` / `moderate` / `low`.
- **Triangulation rule** — `high` requires two independent sources or a primary source. Single-source stays `low` or `moderate` and carries `[single-source]`.

- **Negative findings** ("we searched and this does not appear to exist") are tagged `unverified · low` throughout, however thorough the search. Absence of evidence in a search is weak evidence.
- **`high` means two different things depending on status.** For `asserted` and `corroborated` it means well-triangulated. For `inferred` it means we are confident in our own reasoning. Those are different scales sharing one label; read the status first.

Supersede, never delete. On a contradiction, add a `contradicts` edge and keep both.

## Two rules specific to this domain

**1. Always state the frequency and the sample.** Gold's relationship to real yields explains 87% of variance in annual levels, 12% quarterly and 1.2% daily, from the same paper and the same variables. A number without its frequency is not a number here.

**2. Always state the trial count.** No backtest statistic enters this KB without the number of strategy variants tested to produce it, or an explicit note that the count is undeclared. This applies to our own work first: [[macro-surprise-engine-findings]] declares its count up front. Where a third-party figure is quoted with no declared count, the node says so, because an undeclared count means the figure cannot be deflated and therefore cannot be bounded. See [[system-evaluation-standards]].

**3. A negative finding is a finding.** Where the research established that something does not exist in the literature, that is recorded as a result with a locator, not left as a silence. Four of them in this domain are original-work opportunities; see [[gold-moc]].

## House style
Em dashes are fine inside the KB. Strip them when content becomes an external-facing deliverable (Chris's standing preference). Outward-facing documents also go through `/cold-read` before they are considered done.
