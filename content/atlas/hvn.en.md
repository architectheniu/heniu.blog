---
title: "HVN — High Volume Node, the Barrier of the System"
date: 2026-10-12
draft: false
tags: ["atlas", "HVN", "volume profile", "microstructure"]
---

# HVN — High Volume Node

**In the Antigravity cosmology:** a Barrier — a volume node of the US100 ecosystem.
**In classical language:** High Volume Node — a price level at which the market has done an unusually large amount of trading in recent days.

## What an HVN really is

An ordinary chart shows *when* trading happened. A volume profile shows *where*: it spreads several days of volume across price levels. Price merely passes through most levels. At some of them the market trades long and willingly, because both sides found that price acceptable — that is where a node grows, a High Volume Node.

In Heniu's cosmology a node is a barrier: a place with a lot of previously transacted interest on both sides. Sometimes price stops there, sometimes it passes straight through. Heniu does not assume in advance what will happen — Heniu records what did happen.

## HVN at Heniu: the whole US100 ecosystem

Heniu does not look for the nodes of a single instrument. An HVN is a level where the whole US100 ecosystem concentrated its volume: NQ futures contracts (the Probe), shares of the NDX index companies (the Star) and shares of the QQQ fund (the Dyson Sphere). Outside the cash session only NQ trades, so only NQ adds volume to the profile then.

Contracts, company shares and fund shares are different units, so Heniu does not add them up. Each market has an **equal voice** (the Architect's decision): the volume at a level is divided by that market's volume over the whole window, and the ecosystem profile is the average of the three shares. What counts is where each market concentrates its volume, not which one trades more units.

## How we measure it on the bridge

- **Common axis:** the NDX index level, in steps of 10 points. Heniu converts the NQ price to this axis through the basis (NQ − NDX) and the QQQ price through the ratio (NDX / QQQ). Both relations are measured live during the cash session — the median of the last 600 measurements — and kept overnight.
- **Hours:** NQ counts during CME trading hours; NDX and QQQ during the cash session.
- **Volume:** the volume of the current 15-minute candle, read from the TradingView screen by a browser extension. The candle grows for 15 minutes; Heniu adds each increase in its volume to the level where price stood at that moment, and only along the longest non-decreasing run of readings, so momentary reading spikes (e.g. 1,560 → 16,720 → 1,560) never enter the profile.
- **Window:** the last 5 CME trading days; a trading day starts at 18:00 New York time.
- **Node:** a level that is the strongest within 2 levels on either side (±20 points) and holds at least half the share of the strongest level in the whole profile.
- **Breakout:** price (on the NDX axis) must stand at least 5 points beyond the level. Breakouts alternate (up, then down), at most once every 10 minutes per level. Heniu accepts an NQ price jump of more than 60 points only once it has held for 2 minutes — a fuse against reading errors.

## How HVNs show up in the Logs

The bridge records three kinds of events, and the Sage notes them in the next T-Log:

- **new node** — e.g. "HVN node at NDX level 30660 (NQ ≈ 30887)", with each of the three markets' share of 5-day volume;
- **barrier taken** — a node broken to the upside;
- **support overturned** — a node broken to the downside.

The level always sits on the NDX axis; the brackets give its approximate NQ equivalent, because the basis between the contract and the index changes from day to day. When events touch several neighbouring levels, the Sage merges them into a zone, e.g. "30690 – 30730".

## What an HVN does not do

It does not predict whether price will bounce off a node or pass through it. A node is a record of the past: a map of where the ecosystem traded most willingly over the last 5 days. A breakout is a fact recorded after the fact, not a signal. On this blog an HVN describes the terrain price moves across — nothing more.

---

*An Atlas card. Zero signals — only the physics of the System.*
