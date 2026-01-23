---
title: Trading on Orca
description: Overview of trading features and why Orca offers the best trading experience on Solana.
icon: arrow-right-arrow-left
---

Orca is Solana's leading decentralized exchange, designed to make trading crypto simple, fast, and cost-effective.

<Info>
Orca v2 compares quotes from its own pools and Jupiter aggregator—you always get the best price without leaving the app.
</Info>

---

## Why Trade on Orca?

<CardGroup cols={3}>
  <Card title="Best Prices" icon="badge-dollar">
    Concentrated liquidity pools pack liquidity tightly around current prices for lower slippage
  </Card>
  <Card title="Sub-Second Speed" icon="bolt">
    Trades confirm almost instantly on Solana with fees typically under $0.01
  </Card>
  <Card title="Simple Interface" icon="hand-pointer">
    Swap in just a few clicks with clear information upfront
  </Card>
</CardGroup>

---

## How Orca Works

### Concentrated Liquidity

Unlike traditional DEXs that spread liquidity across all prices, Orca uses Concentrated Liquidity Market Makers (CLMMs):

| Traditional DEX | Orca CLMM |
|----------------|-----------|
| Liquidity spread thin | Liquidity concentrated around market price |
| Higher slippage | Lower slippage |
| Worse prices | Better prices |

### Smart Routing

When you make a trade, Orca:

<Steps>
  <Step title="Finds the best pools">
    Scans available liquidity across all relevant pools
  </Step>
  <Step title="Calculates optimal route">
    Determines the path that gives you the best output
  </Step>
  <Step title="Compares with Jupiter">
    Shows you both Orca and aggregated quotes
  </Step>
  <Step title="Executes with minimal slippage">
    Completes your trade at the best available price
  </Step>
</Steps>

---

## What You Can Do

<CardGroup cols={2}>
  <Card title="Swap Tokens" icon="arrow-right-arrow-left" href="/trade/how-to-swap">
    Exchange any supported token for another in seconds. See real-time prices and set slippage protection.
  </Card>
  <Card title="Range Orders" icon="crosshairs" href="/trade/range-orders">
    Set limit-order-style positions that earn fees while waiting to execute. Buy low or sell high automatically.
  </Card>
</CardGroup>

---

## Trading Costs

| Cost Type | Amount | Notes |
|-----------|--------|-------|
| **Network fee** | ~$0.001-0.01 | Solana transaction fee |
| **Trading fee** | 0.01% - 1% | Depends on pool, paid to LPs |
| **Slippage** | Varies | You set the maximum |

### Fee Tiers

Trading fees are paid to liquidity providers:

| Fee Tier | Typical Use |
|----------|-------------|
| **0.01%** | Stablecoin pairs (USDC/USDT) |
| **0.05%** | Stable pairs, high volume |
| **0.30%** | Most pairs |
| **1.00%** | Volatile/exotic pairs |

---

## Getting Started

### Prerequisites

<CardGroup cols={3}>
  <Card title="Solana Wallet" icon="wallet">
    Phantom, Backpack, or another Solana wallet
  </Card>
  <Card title="SOL for Fees" icon="coin">
    Keep at least 0.01 SOL
  </Card>
  <Card title="Tokens to Trade" icon="coins">
    The token you want to swap
  </Card>
</CardGroup>

### Your First Trade

<Steps>
  <Step title="Visit Orca">
    Go to [orca.so](https://www.orca.so)
  </Step>
  <Step title="Connect wallet">
    Click Connect Wallet and approve
  </Step>
  <Step title="Select tokens">
    Choose what to sell and buy
  </Step>
  <Step title="Enter amount">
    Input your trade size
  </Step>
  <Step title="Review and confirm">
    Check the quote and approve in wallet
  </Step>
</Steps>

<Card title="Detailed Swap Guide" icon="book-open" href="/trade/how-to-swap">
  Follow our step-by-step tutorial with screenshots
</Card>

---

## Trading Tips

<AccordionGroup>
  <Accordion title="For better prices">
    - **Trade popular pairs** — More liquidity = better prices
    - **Avoid small pools** — Low liquidity means higher slippage
    - **Check the quote** — Compare Orca vs Jupiter pricing
    - **Split large trades** — Reduces price impact
  </Accordion>

  <Accordion title="For safer trades">
    - **Set appropriate slippage** — Start with 0.5-1% for major pairs
    - **Verify token addresses** — Especially for new or unfamiliar tokens
    - **Start small** — Test with a small amount first
    - **Review in wallet** — Always check transaction details before signing
  </Accordion>

  <Accordion title="Understanding slippage">
    Slippage is the difference between expected and actual trade price. Higher volatility and lower liquidity increase slippage.

    [Learn more about slippage →](/trade/slippage)
  </Accordion>
</AccordionGroup>

---

## Common Questions

<AccordionGroup>
  <Accordion title="Is Orca safe?">
    Orca's smart contracts are audited and have secured billions in trading volume. However, always practice good security hygiene—verify transactions and protect your wallet.
  </Accordion>

  <Accordion title="What tokens can I trade?">
    Any SPL token with a liquidity pool on Orca. Major tokens like SOL, USDC, and USDT have the deepest liquidity.
  </Accordion>

  <Accordion title="Why did my trade fail?">
    Common reasons:
    - Slippage tolerance too low
    - Insufficient SOL for fees
    - Price moved during confirmation

    [See troubleshooting guide →](/support/faqs)
  </Accordion>

  <Accordion title="Are there trading limits?">
    No account limits. Trade size is only limited by available liquidity in the pool.
  </Accordion>
</AccordionGroup>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="How to Swap" icon="arrow-right-arrow-left" href="/trade/how-to-swap">
    Step-by-step trading guide
  </Card>
  <Card title="Understanding Slippage" icon="sliders" href="/trade/slippage">
    Learn about price impact
  </Card>
  <Card title="Range Orders" icon="crosshairs" href="/trade/range-orders">
    Advanced order types
  </Card>
  <Card title="FAQs" icon="circle-question" href="/support/faqs">
    Common questions answered
  </Card>
</CardGroup>
