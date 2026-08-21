---
title: "NDX CVD — Cash Index Volume Delta Aggregation"
date: 2026-08-21
draft: false
tags: ["atlas", "NDX CVD", "order flow", "aggregation", "microstructure"]
---

# NDX CVD — Cash Index Volume Delta Aggregation

**In Antigravity Cosmology:** Central Star Fuel (NDX).
**In Classical Language:** Aggregated, capitalization-weighted Cumulative Volume Delta (CVD) for the 100 constituent stocks of the NASDAQ-100 index.

## How NDX CVD is Constructed

The NASDAQ-100 index is a basket of equities rather than a single traded share. The **NDX CVD** metric in Heniu's telemetry is constructed as follows:

1. **Transaction Feed:** Continuous monitoring of executed prints across all 100 index components.
2. **Trade Classification:** Prints executing at Ask (aggressive buyers) add to delta; prints at Bid (aggressive sellers) subtract from delta.
3. **Weighting and Aggregation:** Volume deltas are aggregated in real time weighted by index representation, yielding a single synthetic net energy flow line for the entire spot cash market.
4. **Session Reset:** CVD is reset at the cash market opening bell at 9:30 AM ET, establishing a clean daily baseline.

## Unit Interpretation

Reported values (e.g. `+162.49M` or `-175.43M`) represent the total net shares aggressively bought or sold across index components during the session.

* **NDX / CVD Divergence:** If price declines while NDX CVD climbs, it reflects passive limit-order absorption of aggressive market selling. Conversely, rising price on negative CVD indicates passive distribution into aggressive buying.

---

*Atlas Card. Zero signals — pure system physics.*
