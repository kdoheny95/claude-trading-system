# Skills Reference

These are the six custom skills built into this trading system. They live inside Claude's project memory and trigger automatically based on what you ask — no manual prompting required.

---

## How Skills Work

Skills are loaded into your Claude Project. Once they're in place, Claude reads them and knows when to use each one based on the context of your request. You don't call them by name. You just ask your question and Claude routes to the right skill automatically.

To load a skill into your project:
1. Open your Claude Project
2. Go to Project Knowledge
3. Upload or paste the contents of each `SKILL.md` file

---

## The Six Skills

### 1. `us-stock-analysis`
**What it does:** Full fundamental + technical analysis on any US ticker. Pulls current price, financials, valuation metrics, analyst ratings, and recent news. Runs a structured investment report with bull/bear case, support levels, and conviction rating.

**When it triggers:** "Analyze MU", "Give me a report on NVDA", "Is AMZN overvalued?", "Compare TSLA vs AMD"

📁 `skills/us-stock-analysis/SKILL.md`

---

### 2. `options-strategy-advisor`
**What it does:** Options structure analysis using Black-Scholes pricing model. Calculates Greeks, simulates P/L scenarios, evaluates strategy fit (calls, spreads, straddles, iron condors), and gives risk management guidance including position sizing and stop levels.

**When it triggers:** "Should I buy a call or spread on NVDA?", "What's my max loss on this position?", "Calculate my Greeks exposure", "Should I trade before earnings?"

📁 `skills/options-strategy-advisor/SKILL.md`

---

### 3. `earnings-calendar`
**What it does:** Pulls the upcoming earnings calendar using the FMP API. Filters for mid-cap and above ($2B+ market cap), organizes by date and timing (before market open / after market close), and includes EPS and revenue estimates.

**When it triggers:** "What earnings are coming up next week?", "Build me a catalyst calendar for the next 8 weeks", "What tech names report this month?"

📁 `skills/earnings-calendar/SKILL.md`

> **Note:** Requires a free FMP API key. Get one at https://site.financialmodelingprep.com/developer/docs

---

### 4. `technical-analyst`
**What it does:** Pure chart analysis from screenshots. Identifies trend direction, support/resistance levels, moving average alignment, volume patterns, and chart patterns. Produces probabilistic scenarios (bull/base/bear) with price targets and invalidation levels.

**When it triggers:** Send a chart screenshot + ask "analyze this chart", "where's support?", "what's the trend?", "should I enter here?"

📁 `skills/technical-analyst/SKILL.md`

---

### 5. `market-news-analyst`
**What it does:** Pulls and analyzes market-moving news from the past 10 days. Covers FOMC decisions, earnings from mega-caps, geopolitical events, and commodity moves. Ranks events by market impact and explains the actual market reaction vs. what was expected.

**When it triggers:** "What happened in the market this week?", "How did the Fed decision affect tech?", "Summarize recent market news", "What's moving the tape right now?"

📁 `skills/market-news-analyst/SKILL.md`

---

### 6. `market-environment-analysis`
**What it does:** Comprehensive current market environment report. Covers US/European/Asian indices, forex, commodities, VIX, yield curve, and sector rotation. Outputs a risk-on/risk-off assessment with short-term directional outlook.

**When it triggers:** "What does the market look like right now?", "Is it a good time to deploy capital?", "What's the overall tape?", "Give me a market briefing"

📁 `skills/market-environment-analysis/SKILL.md`

---

## Recommended Setup Order

1. Load all 6 `SKILL.md` files into your Claude Project Knowledge
2. Paste your trader profile (see README → First Session)
3. Get your FMP API key for the earnings calendar skill
4. Run your first trade using the 6-step daily workflow

---

## Skills Do Not Replace Judgment

These skills give Claude structured frameworks to work from. They do not make decisions for you. The output is a research input — you still verify the live chain, you still set your own limits, and you still decide whether to pull the trigger.

Process first. Always.
