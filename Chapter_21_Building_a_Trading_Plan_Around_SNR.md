# Chapter 21: Building a Trading Plan Around SNR

## 21.1 From Knowledge to a Rulebook

A trading plan converts the ideas in this book into decisions you can make consistently. Without a written plan, traders tend to change definitions after seeing the chart, take setups that were never tested, and judge the strategy by isolated outcomes. Your plan should be specific enough that another trader could understand what you do, while flexible enough to be tested and improved through evidence.

## 21.2 Define Your Trading Scope

Begin by limiting the environment in which your SNR system operates:

- Instruments: for example, selected forex pairs and XAUUSD.
- Trading sessions: Asian, London, New York, or a defined overlap.
- HTF, MTF, and LTF timeframes.
- Maximum number of trades per day and week.
- Whether trades may remain open overnight or through major events.
- Platform, broker, contract specifications, and execution assumptions.

A narrow scope produces cleaner data. Do not combine gold, major forex pairs, indices, and cryptocurrencies in one performance statistic unless you analyze their behavior separately first.

## 21.3 Define Market Context

Write objective definitions for each market state:

- **Uptrend:** a sequence of confirmed HHs and HLs on the selected HTF.
- **Downtrend:** a sequence of confirmed LHs and LLs.
- **Range:** repeated reactions between relatively stable upper and lower boundaries.
- **MSS:** the specific structural break that invalidates the prior directional assumption.
- **BOS:** the specific break that confirms continuation.

Avoid vague phrases such as "the chart looks bullish." State exactly which swing must hold and which break would invalidate the bias.

## 21.4 Define a Qualified SNR Zone

Your plan should specify:

- How support and resistance are identified.
- Whether the two-candle handoff is mandatory.
- How body and wick boundaries are drawn.
- The minimum impulse size or departure quality.
- Maximum acceptable prior tests.
- How zone width is adjusted for timeframe and volatility.
- How Malaysian SNR, order blocks, FVGs, liquidity sweeps, or trendlines are counted as confluence.

For example, a qualified buy zone might require a bearish-to-bullish handoff on H4, a strong departure, no more than one prior test, and alignment with a Daily Higher Low.

## 21.5 Define Entry Rules

Write the exact sequence required before an order is allowed:

1. HTF bias is established.
2. Price reaches a qualified zone.
3. MTF approach does not invalidate the bias.
4. LTF trigger closes: rejection candle, two-candle handoff, liquidity sweep reversal, or structural confirmation.
5. Entry, stop, target, and position size are calculated.
6. Reward-to-risk and event-risk conditions pass.

Also define what does *not* qualify: entering in the middle of a range, chasing an extended move, entering before the candle closes, or trading against a strong HTF structure without a confirmed MSS.

## 21.6 Define Exit and Management Rules

Specify all exits before entry:

- Initial stop location.
- First and second targets.
- Partial-profit rules.
- Trailing-stop method, if any.
- Breakeven rule, if any.
- Time-based exit, if applicable.
- Conditions for manual exit.

A manual exit should be tied to an objective invalidation event, not merely discomfort caused by normal pullback behavior.

## 21.7 Define Risk Rules

Your risk section should include:

- Risk percentage or fixed amount per trade.
- Maximum combined exposure across correlated positions.
- Daily and weekly loss limits.
- Maximum consecutive losses before a pause.
- Maximum open positions.
- Reduced-risk protocol during drawdown.
- Rules for spread, slippage, and abnormal volatility.

The plan must also state whether a new trade is allowed after a stop-out at the same zone. Do not leave this decision to frustration or hope.

## 21.8 Create a Setup Scorecard

A scorecard turns subjective judgment into comparable data. Example fields:

| Factor | Requirement | Score |
|---|---|---:|
| HTF structure | Direction aligned | Mandatory |
| Zone freshness | Fresh or one test | 1 |
| Strong departure | Clear impulse | 1 |
| MTF alignment | No invalidating MSS | Mandatory |
| LTF trigger | Confirmed candle or structure | Mandatory |
| Liquidity event | Sweep and reversal | 1 |
| Trendline/FVG | Valid confluence | 1 |
| Premium/discount | Directionally favorable | 1 |

Set a minimum score before testing the strategy. Do not change the minimum after seeing an individual outcome; evaluate the rule using a defined sample.

## 21.9 Backtesting the Plan

Backtest one clearly defined setup at a time. Record every eligible occurrence, not only the attractive winners. Include spread, commission, likely slippage, and realistic entry timing. Separate in-sample development data from out-of-sample validation data to reduce overfitting.

Useful metrics include:

- Number of trades.
- Win rate.
- Average win and average loss in R.
- Expectancy.
- Maximum drawdown.
- Longest losing streak.
- Profit factor.
- Results by instrument, session, timeframe, and setup score.

A strategy is not validated by a handful of screenshots. It requires a sufficiently broad and consistently labeled sample.

## 21.10 Forward Testing and Automation

After historical testing, forward-test in a demo or very small live account. Confirm that live spreads, execution speed, news conditions, and platform behavior match your assumptions. If you automate parts of the process, keep detection separate from execution at first:

- Detect swing points and candidate zones.
- Calculate freshness and zone width.
- Alert when price enters a qualified zone.
- Require manual or separately tested confirmation before order placement.

Automation can improve consistency, but it cannot turn ambiguous definitions into a reliable system. Every rule must be expressed precisely enough for a human or program to apply the same way.

## 21.11 One-Page SNR Plan Template

**Market and session:**

**Timeframes:**

**HTF bias rule:**

**Qualified support definition:**

**Qualified resistance definition:**

**Freshness rule:**

**Required confluence:**

**Entry triggers:**

**Stop rule:**

**Target rule:**

**Risk per trade:**

**Daily/weekly limits:**

**Trade-management rules:**

**Invalidation conditions:**

**Journal fields:**

## 21.12 Worked Example: A Minimal XAUUSD Plan

- Instrument: XAUUSD only during the London–New York overlap.
- HTF: Daily for bias and H4 for zones; M15 for entry.
- Buy bias: Daily HH/HL structure remains intact and price reaches fresh H4 support near a Daily HL.
- Sell bias: Daily LH/LL structure remains intact and price reaches fresh H4 resistance near a Daily LH.
- Entry: M15 rejection, handoff, or sweep reversal after candle close.
- Risk: fixed percentage per trade, with position size calculated from the actual stop.
- Skip: zone has three or more tests, no HTF alignment, abnormal spread, or daily loss limit reached.

This is only a template. The trader must test the definitions, thresholds, and session before treating the plan as an operational strategy.

## 21.13 Chapter Summary

- A trading plan turns SNR concepts into objective, testable rules.
- Define scope, market structure, zones, entries, exits, risk, and invalidation before trading.
- Scorecards and consistent labels make performance analysis more reliable.
- Backtest complete samples, include realistic costs, and validate with forward testing.
- Automation is useful only after ambiguous concepts have been converted into precise rules.

## 21.14 Review Questions

1. Why should a trading plan define the market and session instead of covering every instrument?
2. Which parts of an SNR setup must be objective enough to backtest?
3. Why should realistic transaction costs be included in testing?
4. What is the difference between detection automation and execution automation?
5. Write your own minimum requirements for a qualified SNR buy zone.

*Next: Chapter 22 — Journaling and Performance Review, where you'll learn how to turn completed trades into useful evidence for improving the system.*
