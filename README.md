# Gold Desk

Shared working repository for the AI macroeconomic research tool for gold traders.

Malek builds and drives the product. Chris advises and builds the evidence base. This repo
exists so both of us, and both of our AI assistants, can work from the same facts instead of
re-explaining the project to a fresh session every time.

Private. Nothing here is public.

---

## Start here

| If you want | Open |
|---|---|
| The two-minute version | [`kb/_snapshot.md`](kb/_snapshot.md) |
| A map of everything | [`kb/gold-moc.md`](kb/gold-moc.md) or [`kb/_index.md`](kb/_index.md) |
| What we actually measured | [`kb/A2-signals/macro-surprise-engine-findings.md`](kb/A2-signals/macro-surprise-engine-findings.md) |
| What is open and what is blocked | [`kb/_ingest-queue.md`](kb/_ingest-queue.md) |
| The live status board | [`control-centre/`](control-centre/) |

## What is in here

```
kb/               The knowledge base. 56 nodes. This is the substance.
  A1-market/      How gold actually prices
  A2-signals/     Candidate signals, including our own results
  A3-product/     The product, the prototype, the feedback loop
  A4-trading/     The bots, and the standards a trading claim has to meet
  A5-commercial/  Market, competitors, pricing, data licensing, regulation
  A6-raw-register/ Verbatim sources, hashed, with coverage logs
  people/ organisations/
engine/           The Stage 0 event-study code and its output
control-centre/   The status board and the registers behind it
```

## How to read a node

Every material claim carries a tag like this:

```
[corroborated · high · src: raw-research-gold-drivers-2026-09-19#§1.1]
```

That is **status**, **evidence grade**, and a **pointer back to the raw source**, down to the
transcript timestamp or the section number. If a claim has no tag, it is not evidence.

- **status**: `asserted` (one source says so), `corroborated` (two independent sources or a primary),
  `inferred` (our reasoning, not stated anywhere), `contested` (sources disagree),
  `unverified` (we could not check it)
- **grade**: `high` / `moderate` / `low`. High requires two independent sources or a primary one.
  Single-source stays moderate or low and carries `[single-source]`, however confident it reads.

Two rules specific to this domain, both in [`kb/_conventions.md`](kb/_conventions.md):

1. **Always state the frequency.** Gold's relationship to real yields explains 87% of variance in
   annual levels, 12% quarterly and 1.2% daily, from the same paper and the same variables. A
   number without its frequency is not a number here.
2. **Always state the trial count.** No backtest statistic enters this repo without the number of
   strategy variants tested to produce it, or an explicit note that the count is undeclared.

## Where the project stands, in five lines

- **The effect is real and it is fast.** Macro surprises move gold with t = 10.55 at one minute,
  and the fitted relationship stops generalising between one and four hours.
- **The EMA21 hypothesis is null.** Tested three independent ways. The write-up is
  [`kb/A2-signals/ema21-hypothesis.md`](kb/A2-signals/ema21-hypothesis.md), and it distinguishes the
  claim that was tested from the one that was not.
- **The fifteen dollar business model does not survive the arithmetic.** Not because of price.
  See [`kb/A5-commercial/business-model-hypothesis.md`](kb/A5-commercial/business-model-hypothesis.md).
- **The bot integration idea may be the actual business**, and nobody has published a test of it.
  See [`kb/A3-product/bot-integration-layer.md`](kb/A3-product/bot-integration-layer.md).
- **Three things are blocking** and must be verified before anything is repeated to a third party.
  They are at the top of [`kb/_ingest-queue.md`](kb/_ingest-queue.md).

## Adding to it

Point your assistant at this repo and tell it to read `CLAUDE.md` first. That file is the
operating instructions: where things go, how claims are tagged, and what it must not do.

If you are adding something new, the short version is: put the raw source in
`kb/A6-raw-register/` with a hash, write the derived claims into the right `A*` folder with
per-claim tags, add a line to `kb/log.md`, and register any new node in `kb/_index.md`.

## The engine

`engine/` holds the Stage 0 event study. `engine/ENGINE.md` explains how to run it.
`engine/RESULTS.md` and `engine/analysis.json` are the output that the knowledge base cites.

Note that `fetch_ticks.py` pulls roughly 3.3 GB of tick data. Do not run it casually.
