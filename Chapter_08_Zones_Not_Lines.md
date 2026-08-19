# Chapter 8: Zones, Not Lines

## 8.1 Revisiting the Core Principle

Since Chapter 3, this book has repeated one principle: SNR is a **zone**, not a single-price line. This chapter formalizes exactly how to draw that zone correctly, how wide it should be, and how zone width should adapt across timeframes and instruments — including the higher volatility of XAUUSD compared to major forex pairs.

## 8.2 Why Single Lines Fail

A single-price line implies price must reverse at that *exact* number to validate your analysis. In reality:

- Spread and slippage mean your broker's price and another broker's price for the same instrument can differ by several pips/points at any moment.
- Institutional orders are rarely placed at one exact price; they're scaled across a small range to manage market impact.
- Retail stop-losses cluster in a range around obvious levels, not at one precise tick.

Drawing a single line and expecting a reaction at that precise number leads to two common failures: **premature entries** (entering as price approaches the line, then getting stopped out by a slightly deeper wick) and **missed entries** (skipping a trade because price reversed a few pips before or after the exact line).

## 8.3 Constructing the Zone Correctly

Combining the methods from Chapters 5 and 6, construct each zone using this rule:

- **Inner boundary** — the candle body edge closest to current price (per Chapter 5's two-candle rule).
- **Outer boundary** — extend slightly beyond the inner boundary to account for the "cluster" of resting orders, typically to the nearest significant wick extreme or the next candle's body edge.
- Cross-check with the Malaysian SNR (Chapter 6) V/A point — if it falls inside your zone, your boundaries are well-calibrated; if it falls noticeably outside, consider widening the zone slightly to include it.

## 8.4 Zone Width by Timeframe

Zone width should scale with the timeframe you're analyzing, because price naturally moves more per candle on higher timeframes:

- **Daily/Weekly zones** — wider zones, often spanning tens of dollars on XAUUSD or dozens of pips on major forex pairs.
- **H4/H1 zones** — moderate width, roughly half to a third of the Daily zone width for the same instrument.
- **M15 and below** — narrow zones, used only for fine-tuning entries within an already-identified HTF zone (per Chapter 11), never as standalone significant levels.

A practical rule of thumb: if your zone width looks disproportionately wide or narrow compared to the average candle range on that timeframe, recalibrate using Section 8.3's boundary rule.

## 8.5 Zone Width by Instrument Volatility

Because you actively trade XAUUSD, this section deserves special attention. Gold is significantly more volatile in absolute price terms than most forex pairs, meaning SNR zones on gold must be proportionally wider than the equivalent zone on, say, EURUSD:

- A EURUSD Daily zone might reasonably span 10–15 pips.
- A XAUUSD Daily zone might reasonably span $5–$15 or more, depending on current volatility regimes (news-heavy periods require wider zones than calm periods).
- Always check the Average True Range (ATR) on your analysis timeframe as a sanity check for whether your zone width is proportionate — an ATR-based check acts as a quick, objective confirmation of the visually-drawn zone.

## 8.6 Avoiding Overly Wide Zones

While zones must be wider than a single line, they shouldn't become so wide that they lose predictive value — a zone spanning 5% of the entire chart's visible range is effectively meaningless. If your zone construction (Section 8.3) produces something this wide, it usually means you're combining two genuinely separate zones into one, or working from too low-quality a formation (revisit the significance filters from Chapter 5.5).

## 8.7 Worked Example

On XAUUSD H4, suppose the two-candle handoff (Chapter 5) gives inner/outer boundaries of $2,358–$2,364, and the Malaysian SNR line-chart V-point sits at $2,361 — comfortably inside this range. The current H4 ATR is roughly $6, meaning your $6-wide zone is proportionate to typical price movement on this timeframe. This zone is well-calibrated and ready to be used in the entry frameworks covered in Part 4.

## 8.8 Chapter Summary

- SNR should always be drawn as a zone, using inner (body-based) and outer (wick/next-candle) boundaries.
- Zone width must scale with both timeframe and instrument volatility — XAUUSD requires proportionally wider zones than most forex majors.
- ATR provides an objective sanity check for whether a drawn zone is proportionate.
- Overly wide zones usually indicate two distinct zones have been merged incorrectly.

## 8.9 Review Questions

1. Why does a single-price line lead to both premature and missed entries?
2. How should zone width scale as you move from Daily to M15 timeframes?
3. Why does XAUUSD generally require wider SNR zones than a pair like EURUSD?
4. What does it usually mean if your constructed zone spans an unusually large price range?

*Next: Chapter 9 — Role Reversal Levels, where you'll learn how broken support becomes resistance (and vice versa), and how to trade this transition with confidence.*
