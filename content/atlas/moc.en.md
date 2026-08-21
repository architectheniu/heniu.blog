---
title: "MOC — the Closing Imbalance, a.k.a. the MOC Anomaly"
date: 2026-08-10
draft: false
tags: ["atlas", "MOC", "order flow", "microstructure"]
---

# MOC — Market-On-Close Imbalance

**In the Antigravity cosmology:** the MOC Anomaly / the MOC Hammer — a gravitational strike in the final minutes of the cycle.
**In classical language:** the order imbalance into the close — the surplus of demand or supply the exchange must pair off by 4:00 PM New York time.

## What MOC really is

A vast share of market capital — index funds, ETFs — settles by definition at the **closing price**. Their orders flow into a special closing auction, and starting at 3:50 PM ET the exchange publishes the **Net Order Imbalance Indicator (NOII)**: how much volume remains un-paired between buyers and sellers. It is one of the cleanest public windows into explicitly declared closing-auction interest (the Nasdaq Closing Cross) — the flow in the auction book is registered, not guessed.

That is why the MOC window is often the most gravitationally dense moment of the session: tens or hundreds of millions of shares hunt for the other side within minutes. The closing price that results becomes the reference point for the entire next day.

## How we measure it on the bridge

Heniu reads the net imbalance in the MOC window and treats it with thresholds hard-coded in the system's configuration: a surplus around ±50M is a strong signal of directional closing pressure, and ±150M is a singularity-class event (the "MOC Hammer"). The reading informs the description of the system's vector from ~3:50 PM exchange time into the night — documenting closing order interest.

## What MOC does not do

It does not prophesy tomorrow's session — it measures today's settlement pressure. Sometimes a giant MOC Hammer is absorbed without a trace; sometimes a small imbalance ends in a large move. On this blog, MOC is a description of the force present in the auction — nothing more.

---

*An Atlas card. Zero signals — only the physics of the System.*
