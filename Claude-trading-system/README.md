# Claude Options Trading System

A structured, catalyst-driven options trading workflow built on top of Claude.ai. No extra tools, no subscriptions beyond Claude Pro, no APIs required. Just a well-built project with persistent memory, custom skills, and a repeatable process.

---

## What This Is

This is not a signal service. Not a bot. Not a guarantee.

It is a process for converting buying power into well-researched, catalyst-driven option positions with defined entry, exit, and stop levels — using Claude as a research partner.

Built and refined over months of real trading sessions. Every rule came from a mistake made or a pattern that worked.

---

## How It Works

You do not retype prompts every session. The system runs on three layers:

**1. Memory**
Set up your trader profile once. Claude remembers it across every session — your rules, your position size, your blocked tickers, your risk tolerance. Each session you just share your current buying power and open positions.

**2. Custom Skills**
Claude has been trained with built-in skills that trigger automatically based on what you ask. No manual prompting required.

| Skill | What It Does |
|---|---|
| `us-stock-analysis` | Fundamental + technical analysis on any US ticker |
| `options-strategy-advisor` | Options structure, Greeks, P&L simulation, strategy recommendations |
| `earnings-calendar` | Upcoming earnings dates, expected moves, prior quarter results |
| `technical-analyst` | Chart analysis from screenshots — support, resistance, trend, entry timing |
| `market-news-analyst` | Recent market-moving news and sector impact |
| `market-environment-analysis` | Overall tape assessment before deploying capital |

**3. The Workflow**
A six-step daily process for every new trade. Never skip a step.

---

## Setup

### Requirements
- Claude.ai account (Pro plan required — $20/month)
- A broker with options trading enabled (built around Robinhood but adaptable)
- Nothing else

### Claude Settings to Enable
Go to Claude Settings and turn on:
- ✅ Web Search
- ✅ Memory
- ✅ Advanced Research (Deep Research)

---

## First Session

Open a new Claude chat and paste the profile below. Tell Claude to remember it permanently.

```
I want to use you as my trading research assistant. Please remember this profile across all our future conversations.

About me. My name is [NAME]. I trade options on [BROKER]. My account size is approximately [AMOUNT]. My typical position size per trade is [AMOUNT]. My options experience level is [BEGINNER / INTERMEDIATE / ADVANCED].

Trading rules I live by.
- Minimum 30 days to expiry on any new position
- Earnings catalyst required inside the option's life
- Limit sell target set before every entry
- 50% stop loss on any single position
- No averaging down on losers
- Cut dead money after two weeks of sideways

Blocked tickers I will not trade. [LIST THEM HERE]

Communication preferences. Be direct. No fluff. Push back when my logic is weak. Verify live data with the advanced research tool whenever recent prices or catalysts matter. When I send screenshots, read them carefully and use them to verify any pricing you recommended. If something does not fit my budget, adjust.

Acknowledge this profile and ask any clarifying questions before we start trading.
```

---

## The Daily Workflow

### Step 1 — State Buying Power and Constraints
Tell Claude exactly what you have to work with.

> *I have $1,200 in buying power. Single call option. No PLTR. Minimum 30 days to expiry. Earnings catalyst required.*

### Step 2 — Share Your Portfolio
Send screenshots of open option positions, stock holdings, and recent trade history. Trade history matters for PDT tracking.

### Step 3 — Ask for the Recommendation
> *Given my buying power, current positions, and constraints, find me the best single call option to buy right now. Use advanced research to check current prices, recent earnings results, and upcoming catalysts. Give me one specific recommendation with ticker, strike, expiry, estimated cost, limit sell target, and full thesis.*

### Step 4 — Verify Against the Live Chain ⚠️
**Most people skip this. Don't.**

Claude models premium estimates — it does not quote live chains. Before placing any order, pull the actual chain in your broker, screenshot the relevant strikes, and send it back. Confirm the strike is priced at or below your budget. Adjust if not.

### Step 5 — Set Up the Order
Place a buy-to-open limit order. Immediately after the fill, set a GTC sell-to-close limit at your take-profit target. Do this before you close the app.

### Step 6 — Document the Trade
Tell Claude what you executed. Strike, fill price, sell limit, stop level. This updates memory for future sessions.

---

## Position Management Rules

| Rule | Details |
|---|---|
| Catalyst passed | Exit within 1–2 sessions after the catalyst fires. Holding past it converts a thesis trade into a hope trade. |
| 50% down | Forces a decision. Cut it or document why the original thesis still holds. Never let it drift. |
| Doubled | Sell at least half mechanically. Remaining contracts run on house money. |
| Dead money | Two weeks sideways with no catalyst — ask Claude "is this dead money?" and cut or redeploy. |

---

## The Hard Rules

```
✅ Catalyst required inside the option's life
✅ Minimum 30 days to expiry
✅ Limit sell target set BEFORE the buy
✅ Mental stop at 50% loss documented before entry
✅ Verify the live chain before any order
✅ Position size matches stated risk tolerance — no exceptions
❌ No weeklies the day before earnings
❌ No averaging down on losers
❌ No holding losers past the catalyst hoping for a bounce
❌ No chasing after a 20%+ single-session move
```

---

## Weekly Review

Every Friday after the close:

> *Run a weekly review of my book. What worked, what did not, what positions are open, what catalysts are in the next two weeks, and what changes should I consider for next week.*

This is the discipline that turns trading into a process.

---

## What This System Is Not

Not a way to get rich. Not a path to predictable returns. Options can lose 100% of premium on any trade and losing streaks happen at the portfolio level.

What it does is give you a structured way to make better-researched decisions, document your thinking, and learn from your own results.

**The edge is process, not picks.**

---

## Why It Works

- You follow the rules instead of cherry-picking the convenient ones
- The memory system means Claude already knows your constraints every session
- The custom skills trigger automatically — no manual prompting
- You verify pricing on the live chain before every entry
- You treat Claude as a research partner to pressure-test your thesis, not a signal service to blindly follow

---

*Built from real trading sessions. Not theory.*
