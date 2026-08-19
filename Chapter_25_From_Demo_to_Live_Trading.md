# Chapter 25: From Demo to Live Trading

## 25.1 The Transition Is a Process

Moving from historical charts to live trading is not a single switch. It is a progression through increasingly realistic forms of uncertainty: first hindsight-free historical testing, then forward testing, then small real-money exposure, and finally gradual scaling. Each stage has a different purpose. Passing one stage does not guarantee success at the next.

The objective is to verify not only that the SNR rules have potential, but also that you can execute them under real spreads, slippage, latency, emotional pressure, and changing market conditions.

## 25.2 Stage 1: Historical Backtesting

Begin with a written strategy, not an informal idea. Test a defined sample while hiding future candles as much as your platform allows. Record every eligible setup, including trades you would prefer to ignore.

At minimum, measure:

- Number of trades.
- Expectancy in R.
- Win rate and average win/loss.
- Maximum drawdown and losing streak.
- Results by instrument, session, timeframe, and setup type.
- Effect of spread, commission, and assumed slippage.

Do not optimize until the definitions are stable. Changing the rules after each result makes the sample unreliable.

## 25.3 Stage 2: Forward Testing

Forward testing evaluates decisions as the market develops in real time. Use a demo account or a replay environment where future information is unavailable.

The focus is on execution:

- Can you mark zones before price reacts?
- Do alerts arrive in time?
- Are the triggers clear enough to apply without hindsight?
- Does the broker's spread behave as assumed?
- Can you follow the plan through a losing streak?

Forward testing should continue long enough to cover different sessions and market states, including trends, ranges, news volatility, and quiet periods.

## 25.4 Stage 3: Minimum-Size Live Trading

A small live account introduces real emotional and execution conditions. Use the smallest practical position size and risk an amount whose loss will not affect your decisions or essential finances.

At this stage, your goal is not maximum profit. Verify:

- Actual fills and slippage.
- Contract specifications and margin behavior.
- Stop execution during fast markets.
- Psychological response to open risk.
- Whether you follow the same rules used in testing.

Never use borrowed money, emergency funds, or money needed for living expenses to test a speculative strategy.

## 25.5 Stage 4: Gradual Scaling

Increase size only after a predefined sample demonstrates both positive or stable performance and acceptable rule adherence. Scale gradually rather than doubling risk after a profitable week.

A scaling plan might require:

- A minimum number of live trades.
- Positive expectancy after costs.
- Rule-adherence above a chosen threshold.
- Drawdown within the tested range.
- No unresolved execution or platform issues.
- A written review approving the next risk level.

If performance deteriorates after scaling, return to the previous level. Scaling is a test of execution capacity, not a reward for recent profits.

## 25.6 Choosing a Broker and Platform

Before live trading, verify:

- Regulation and legal availability in your jurisdiction.
- Contract size, tick value, minimum volume, and margin requirements.
- Typical and event-time spreads.
- Commission, swap, and financing costs.
- Stop-out and liquidation policies.
- Execution model, slippage behavior, and order types.
- Platform stability and data-feed differences.
- Deposit and withdrawal procedures.

For XAUUSD, broker specifications can differ substantially. Confirm the monetary value of a price movement instead of relying on another trader's lot-size example.

## 25.7 Live Execution Checklist

Before placing an order:

1. Is the setup in the written plan?
2. Is HTF structure clear and valid?
3. Is the zone qualified and within freshness limits?
4. Has the required LTF trigger closed?
5. Is the event calendar and spread acceptable?
6. Is the stop at structural invalidation?
7. Is position size calculated from maximum monetary risk?
8. Is the target logical and reachable under the plan?
9. Is total correlated exposure acceptable?
10. Is the order ticket correct before submission?

A checklist prevents avoidable operational errors, especially when gold moves rapidly.

## 25.8 Handling Missed Trades and Platform Problems

A missed trade is not a reason to chase. If the order was not filled, wait for a new setup or a properly defined retest. If a platform, data-feed, or internet problem prevents reliable execution, do not improvise with a wider stop or a different instrument.

Maintain a backup plan for monitoring and communication, but define in advance what happens if your trading environment becomes unreliable. Technical uncertainty is a valid reason to stand aside.

## 25.9 Scaling Out and Withdrawals

If the strategy becomes profitable, decide in advance how profits are handled. Possible rules include maintaining a fixed account-risk percentage, withdrawing a portion at scheduled intervals, or retaining capital until a defined sample is complete.

Do not increase risk solely because the account has recently grown. Update position size according to the written rule, and remember that a larger account can create larger emotional pressure even when the percentage risk is unchanged.

## 25.10 Worked Example: Controlled XAUUSD Progression

A trader backtests 150 defined XAUUSD SNR setups and records positive expectancy after estimated costs. The trader then forward-tests 40 setups in real time, finding that news-window spreads are wider than expected and revising the plan to avoid new entries immediately before major releases.

Next, the trader uses minimum live size for 30 trades at 0.25% risk per trade. Rule adherence remains high, execution matches testing, and drawdown stays within the expected range. The trader moves to 0.5% risk—not because of one profitable week, but because the predefined sample and review conditions were satisfied.

## 25.11 Chapter Summary

- Progress from historical testing to forward testing, minimum-size live trading, and gradual scaling.
- Each stage tests a different problem: strategy behavior, real-time execution, emotional response, and capacity under larger exposure.
- Verify broker-specific costs and XAUUSD contract specifications before live trading.
- Scale only after predefined performance, adherence, and drawdown conditions are met.
- Never chase missed trades or improvise when platform and execution conditions are unreliable.

## 25.12 Review Questions

1. What is the purpose of forward testing after historical backtesting?
2. Why should minimum-size live trading be treated as an execution test rather than a profit challenge?
3. List five broker or platform details that must be verified before trading XAUUSD live.
4. What conditions should be satisfied before increasing risk?
5. Why is chasing a missed trade dangerous?

*Next: Chapter 26 — Common Mistakes and How to Avoid Them, the final main chapter, where you'll consolidate the failure patterns that most often undermine an otherwise sound SNR process.*
