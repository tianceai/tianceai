# Tiance Guanlan AI

> Crypto data intelligence platform. We pull the data you can't see, crunch it, show it to you. You decide.

**Status**: Pre-launch · Closed beta opens July 2026
**Website**: [tianceai.cc](https://tianceai.cc)
**Contact**: `beta@tianceai.cc`

---

## What this is (and isn't)

**This IS**: a data intelligence platform that scrapes, cross-references, and analyzes crypto market data across multiple exchanges + news sources — and hands the result to you.

**This is NOT**: a trading bot, a signal-selling group, or a "quant strategy" you subscribe to. **We don't trade for you.** We help you see what you couldn't see alone.

---

## Why does this exist?

It's 3 AM. You're still staring at the chart.

BTC just printed a long wick. Should you take profit?

Meanwhile — an AI scanned both Binance and OKX, checked 15 indicators, AND read the latest CoinDesk headline. In 30 seconds.

You're racing your fingers. It's already seen everything worth seeing.

**We got tired of losing that race.** So we built the tool that watches for you.

---

## The 3 walls every manual trader hits

**Wall 1 · News is always 5 minutes faster than you**

CZ tweets → you translate → copy → paste to your group → discuss → price already moved 3%.

You're not slow. You're *structurally* slow. You can't watch 8 news sources 24/7. But an AI can. Every 30 seconds, all of them.

**Wall 2 · Your emotions are stronger than your rules**

-5% and you can't sleep. +2% and you want to run. That's not a skill problem. That's biology.

Charts hit the emotional part of your brain — the same one that made cavemen run from tigers. It wasn't designed for finance.

An AI doesn't have that problem. It just sees data. Done.

**Wall 3 · Altcoins never sleep**

BTC/ETH/SOL/BNB alone drain you. 380+ altcoins with signals every 30 minutes? Impossible.

And even IF you catch a volume spike — is it real accumulation, or pump-and-dump? Good luck telling apart at 3 AM.

---

## What we built

Three things, simply put:

### 1️⃣ Watch two exchanges at once (Binance + OKX)

Most tools watch ONE exchange. This is a mistake — because:

- Binance has depth on majors, OKX has depth on many altcoins
- A single-exchange wick is often just that exchange's liquidity glitch, not a real reversal

We watch both. Only signals confirmed on BOTH sides get shown to you. Half the false signals — gone.

### 2️⃣ A model called "Eagle Eye"

It does NOT predict price. Price prediction is mostly a lie.

It answers one question: **"Is the wind with you, or against you, right now?"**

Bad wind → duck early. Good wind → act with confidence.

**You decide whether to act. We just tell you the wind direction.**

<details>
<summary><b>Tech details (click to expand)</b></summary>

- Trained on multi-month K-line + orderflow data across major coins
- Multi-timeframe features (5m / 15m / 1h / 4h / 1d) + orderflow imbalance + news sentiment
- Output: action confidence, NOT price prediction
- Label strategy: multi-horizon triple-barrier with `trigger_ts=close_ts` (no lookahead leakage)
- Ensemble: XGBoost + LightGBM, sub-100ms inference

</details>

### 3️⃣ Altcoin accumulation radar

Every 30 minutes, we scan 380+ altcoins and classify each into 3 buckets:

- ✅ Real accumulation (shown to you)
- ❌ Pump-and-dump (filtered out)
- 🔇 Noise (ignored)

The goal is NOT to help you chase. It's to help you **avoid getting rekt**.

<details>
<summary><b>How we tell them apart (click to expand)</b></summary>

Four dimensions cross-checked:
- Volume acceleration (4H rolling window)
- Order book pressure ratio (bid/ask depth imbalance)
- Whale wallet inflow (on-chain proxy)
- Cross-exchange price divergence

</details>

---

## Closed beta · 100 seats

Each seat gets **8M TOKEN credits** (~30 days of usage).

We're picking:
- ❌ NOT people willing to pay upfront
- ❌ NOT people with big follower counts
- ✅ People willing to break the product with us and give real feedback

You get:
- Direct dev feedback channel
- Your data, fully open — you can inspect everything yourself

Apply: [tianceai.cc](https://tianceai.cc) or DM us "beta"

---

## Roadmap

- **W1 July 2026** · Closed beta opens (100 seats)
- **W2-W3** · Feedback loop + altcoin radar tuning
- **W4** · Public whitepaper — full dual-source architecture writeup
- **August 1** · Cohort 2 evaluation

---

## One more thing

We won't tell you WHAT to buy or sell.

We won't trade for you either.

We just help you see what you couldn't see alone.

The rest — that's your call.

**Tiance Guanlan AI · Every decision, a little sharper than yesterday.**

---

## Disclaimer

This tool provides data analysis and market intelligence for informational purposes only. Not investment advice. All trading decisions and their consequences are the sole responsibility of the user. Crypto trading carries significant capital loss risk.

---

**Contact**: [beta@tianceai.cc](mailto:beta@tianceai.cc)
**License**: TBA

## 📅 最近更新
- [2026-07-15] [2026-07-15 · BTC/ETH/SOL 盘口速览](blog/2026-07-15-daily-briefing.md)
- [2026-07-14] [2026-07-14 · BTC/ETH/SOL 盘口速览](blog/2026-07-14-daily-briefing.md)
- [2026-07-10] [2026-07-10 · BTC/ETH/SOL 盘口速览](blog/2026-07-10-daily-briefing.md)
- [2026-07-09] [2026-07-09 · BTC/ETH/SOL 盘口速览](blog/2026-07-09-daily-briefing.md)
- [2026-07-08] [2026-07-08 · BTC/ETH/SOL 盘口速览](blog/2026-07-08-daily-briefing.md)
- [2026-07-07] [2026-07-07 · BTC/ETH/SOL 盘口速览](blog/2026-07-07-daily-briefing.md)
