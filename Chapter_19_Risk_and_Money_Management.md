# Chapter 19: Risk and Money Management

## 19.1 The First Job of a Trader

Your first job is not to make money. It is to remain solvent long enough for your statistical edge to work. Even an excellent SNR strategy will experience losing trades, losing streaks, slippage, and periods when market conditions do not match its tested behavior. Risk management converts those inevitable losses from account-threatening events into normal business expenses.

This chapter provides a framework for sizing positions, setting stops, evaluating reward-to-risk, controlling correlation, and limiting drawdown. It is educational material, not a promise of profitability or personalized financial advice. Trading leveraged products, including forex and gold CFDs, can result in rapid losses exceeding expectations; verify your broker's contract specifications and local regulatory requirements before trading live.

## 19.2 Define Risk Before Entry

Every trade should have a fixed maximum loss determined before the order is placed. A common framework is to risk a small percentage of account equity per trade, such as 0.25%–1%, depending on your experience, system testing, drawdown tolerance, and instrument volatility. The exact percentage is a design choice, not a universal rule.

Your pre-entry plan should state:

- Account equity used for calculation.
- Maximum currency loss if the stop is hit.
- Entry price and stop-loss price.
- Position size and contract specification.
- Target prices and expected costs.
- Conditions that invalidate the setup.

Never define the risk by lot size alone. The same lot size can represent very different monetary risk on EURUSD, XAUUSD, indices, or other instruments.

## 19.3 Position-Size Formula

The basic position-size relationship is:

\[
\text{Position size} = \frac{\text{Maximum money risk}}{\text{Stop distance} \times \text{Value per price unit}}
\]

For a percentage-based plan:

\[
\text{Maximum money risk} = \text{Account equity} \times \text{Risk percentage}
\]

Example: If equity is $10,000 and planned risk is 0.5%, maximum loss is $50. If the stop distance and broker's contract value imply that one lot would lose $250 at the stop, the position size would be 0.20 lots before considering spread, commission, and slippage. Confirm the exact calculation with your platform because gold contract specifications differ between brokers.

## 19.4 Stop-Loss Logic

A stop-loss should sit at the price that invalidates the trade idea, not at a distance chosen to force a desired lot size. For an SNR buy, invalidation is generally below the zone's outer boundary and any relevant sweep low. For an SNR sell, it is generally above the zone's outer boundary and sweep high.

Add a volatility-appropriate buffer, but avoid placing the stop so far away that the trade no longer offers a logical target. If the correct stop makes the position too large for your risk limit or the target too close for acceptable expectancy, skip the trade.

## 19.5 Reward-to-Risk and Expectancy

Reward-to-risk is useful, but it is not a standalone quality measure. A trade with a 3:1 target can still be poor if the probability of reaching the target is very low. Evaluate the complete system using expectancy:

\[
\text{Expectancy} = (\text{Win rate} \times \text{Average win}) - (\text{Loss rate} \times \text{Average loss})
\]

For example, a strategy winning 40% of trades with an average win of 2R and an average loss of 1R has expectancy:

\[
(0.40 \times 2R) - (0.60 \times 1R) = 0.20R
\]

This is a simplified example before costs and execution differences. Measure expectancy from a sufficiently large, consistently recorded sample—not from a few attractive chart examples.

## 19.6 Daily and Weekly Loss Limits

A per-trade limit does not prevent a trader from taking many correlated losses in one session. Add circuit breakers to your plan:

- Maximum number of trades per session.
- Maximum daily loss, such as 2R or another tested amount.
- Maximum weekly loss.
- Mandatory pause after a defined losing streak.
- No immediate revenge trade after a stop-out.

Once a circuit breaker is reached, stop trading and review later. The purpose is to protect decision quality as well as capital.

## 19.7 Correlation and Concentration Risk

Several positions can express the same idea. A long XAUUSD position, a long USD-related commodity exposure elsewhere, and multiple trades all depending on lower US yields may create more concentration than the ticket sizes suggest. Before entering, ask:

- Are these instruments driven by the same macro factor?
- Are multiple trades sitting at the same type of SNR zone?
- What is the maximum combined loss if the shared thesis fails?
- Does the portfolio-level risk remain within the plan?

Treat correlated trades as one risk cluster rather than independent opportunities.

## 19.8 Managing the Position

Define management rules before entry:

- Whether partial profit is taken at the first structural target.
- Whether the stop moves to breakeven, and under what objective condition.
- Whether a trailing stop follows new swing points.
- What happens if price reaches the zone but fails to trigger.
- Whether positions are closed before a scheduled high-impact event.

Moving a stop to breakeven too quickly can reduce average win size and cause avoidable exits. Test the rule instead of adopting it because it feels safer.

## 19.9 Drawdown and Recovery Mathematics

Losses and recovery are not symmetrical. A 10% account loss requires an 11.1% gain to recover; a 50% loss requires a 100% gain. This is why preserving capital matters more than trying to recover quickly.

During drawdown, reduce risk according to a predefined protocol rather than increasing it. For example, after reaching a tested drawdown threshold, reduce per-trade risk and resume normal size only after a review confirms that execution—not necessarily the strategy's short-term variance—is under control.

## 19.10 Worked Example: Risking a Fixed Amount

A trader has $5,000 equity and risks 0.5% per trade, so maximum planned loss is $25. An XAUUSD buy setup triggers at $2,366, with the correct stop at $2,359: a $7 price distance. The trader checks the broker's XAUUSD contract specification, calculates the monetary loss per lot for a $7 move, and selects a position size whose loss at the stop—including estimated spread and commission—does not exceed $25.

The next trade may have a $3 stop or a $15 stop, but position size changes accordingly. Risk stays approximately constant; the lot size does not.

## 19.11 Chapter Summary

- Capital preservation allows a probabilistic edge to operate over many trades.
- Define maximum monetary risk before entry and calculate position size from stop distance and contract value.
- Stops belong at structural invalidation points, not at arbitrary distances chosen to support a desired lot size.
- Evaluate strategies using expectancy, drawdown, and properly recorded samples—not win rate alone.
- Control daily losses, correlated exposure, and emotional escalation with predefined circuit breakers.

## 19.12 Review Questions

1. Why should position size be calculated from monetary risk and stop distance rather than chosen first?
2. Write the position-size formula in your own words.
3. How does expectancy differ from reward-to-risk?
4. Why should correlated positions be treated as one risk cluster?
5. What should happen after a daily loss limit is reached?

*Next: Chapter 20 — Trading Psychology and Discipline, where you'll learn how to execute these rules consistently when fear, greed, and recent results try to interfere.*
