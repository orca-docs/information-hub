---
title: Understanding Slippage
description: Learn about slippage, price impact, and how to protect your trades.
icon: sliders
---

Slippage is the difference between the price you expect and the price you actually get. Understanding it helps you trade smarter and avoid costly mistakes.

---

## Slippage vs Price Impact

These terms are often confused but mean different things:

<CardGroup cols={2}>
  <Card title="Slippage" icon="chart-line">
    Price movement that happens **between** when you submit a trade and when it executes—caused by other traders and market activity.
  </Card>
  <Card title="Price Impact" icon="arrow-trend-down">
    Price movement caused **by your trade itself**—larger trades in smaller pools have higher price impact.
  </Card>
</CardGroup>

| Factor | Slippage | Price Impact |
|--------|----------|--------------|
| **Cause** | Other market activity | Your trade size |
| **Control** | Set tolerance limit | Choose better pools/split trades |
| **Visibility** | Unknown until execution | Shown in quote |

<Info>
Orca displays price impact in the swap interface before you trade. Always check this before large swaps.
</Info>

---

## Slippage Tolerance Settings

Slippage tolerance is the **maximum price difference** you're willing to accept. If the price moves more than your tolerance, the transaction fails instead of executing at a bad price.

### Recommended Settings

| Scenario | Tolerance | Notes |
|----------|-----------|-------|
| Stablecoin pairs | 0.1% | Very stable prices |
| Major pairs (SOL/USDC) | 0.5% | Normal market conditions |
| Volatile tokens | 1-3% | Higher volatility expected |
| High volatility periods | 2-5% | Use with caution |

### How to Adjust Slippage

<Steps>
  <Step title="Open settings">
    Click the **gear icon** (⚙️) in the swap interface
  </Step>
  <Step title="Set your tolerance">
    Enter your desired slippage percentage or select a preset
  </Step>
  <Step title="Save and trade">
    Your setting applies to your current and future trades
  </Step>
</Steps>

<Tip>
Orca has separate slippage settings for **trades** and **liquidity operations**. Liquidity operations can safely use higher slippage since they're not vulnerable to front-running.
</Tip>

---

## Risks of High Slippage

Setting slippage too high exposes you to:

<AccordionGroup>
  <Accordion title="Front-running attacks">
    **What it is:** A bot sees your pending transaction and places trades before and after yours, profiting from the price movement.

    **Sandwich attack:** Your trade gets "sandwiched" between two attacker transactions:
    1. Attacker buys → price goes up
    2. Your trade executes at higher price
    3. Attacker sells → profits from your trade

    **Protection:** Lower slippage tolerance limits how much value can be extracted.
  </Accordion>

  <Accordion title="Poor value trades">
    Even without attacks, high slippage means you might accept a significantly worse price if the market moves against you between quote and execution.

    **Example:** You quote a trade at $100. With 5% slippage, you could receive as little as $95 if the market moves.
  </Accordion>
</AccordionGroup>

<Warning>
Never set slippage higher than necessary. Start low and only increase if transactions fail.
</Warning>

---

## When to Increase Slippage

Sometimes higher slippage is necessary:

| Situation | Why | Recommendation |
|-----------|-----|----------------|
| **High volatility** | Prices moving rapidly | Increase gradually until trade succeeds |
| **Low liquidity pools** | Price swings more easily | Consider if the trade is worth the risk |
| **Network congestion** | Transactions take longer to confirm | Small increases may help |
| **Urgent trades** | Can't afford failed transactions | Accept the trade-off knowingly |

<Note>
If you don't need to trade immediately, waiting for volatility to settle is often better than increasing slippage.
</Note>

---

## Avoiding Poor Value Trades

Even with proper slippage settings, you can get bad prices if you're not careful:

### Always Check Before Trading

<Steps>
  <Step title="Verify the quoted price">
    Does the rate match what you expect? Compare with price aggregators like CoinGecko.
  </Step>
  <Step title="Check price impact">
    High price impact (>1%) means you're significantly moving the market. Consider splitting the trade.
  </Step>
  <Step title="Look at pool liquidity">
    Low liquidity pools have worse prices and higher volatility.
  </Step>
  <Step title="Verify the token">
    Confirm you're trading the correct token by checking the mint address.
  </Step>
</Steps>

### Red Flags to Watch For

- **Price significantly different from other markets** — The pool may be stale or manipulated
- **Very high price impact** — Your trade is too large for the available liquidity
- **New or unfamiliar tokens** — Higher risk of scams or extreme volatility
- **Pools with very low TVL** — Prices can swing wildly

<Warning>
Pool prices are determined by trading activity, not external oracles. A pool's price can differ significantly from other markets, especially in low-liquidity or inactive pools. Always verify the quoted price meets your expectations.
</Warning>

---

## Summary

<CardGroup cols={2}>
  <Card title="Set Appropriate Slippage" icon="sliders">
    Start with 0.5% for most trades, adjust only if needed
  </Card>
  <Card title="Check Price Impact" icon="magnifying-glass-chart">
    Always review before large trades
  </Card>
  <Card title="Verify Prices" icon="circle-check">
    Compare with external price sources
  </Card>
  <Card title="Be Cautious" icon="shield">
    When in doubt, start with a small test trade
  </Card>
</CardGroup>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="How to Swap" icon="arrow-right-arrow-left" href="/trade/how-to-swap">
    Step-by-step swap guide
  </Card>
  <Card title="Range Orders" icon="crosshairs" href="/trade/range-orders">
    Advanced order types
  </Card>
</CardGroup>
