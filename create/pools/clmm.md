---
title: Creating a CLMM Pool
description: Create a concentrated liquidity pool with full customization options.
icon: chart-mixed
---

CLMM (Concentrated Liquidity Market Maker) pools give you complete control over your pool's configuration.

<Info>
**New to pool creation?** Consider starting with a [Splash Pool](/create/pools/splash) for a simpler experience. CLMM pools are best for established tokens or when you need custom configurations.
</Info>

---

## CLMM vs Splash Pool

| Feature | Splash Pool | CLMM Pool |
|---------|------------|-----------|
| **Setup complexity** | Simple | More complex |
| **Cost** | Lower | Higher |
| **Position types** | Full-range only | Custom ranges |
| **Management** | Minimal | More involved |
| **Best for** | New tokens, simple launches | Established tokens, advanced users |

---

## Prerequisites

Before creating a pool:

<CardGroup cols={2}>
  <Card title="Both Tokens" icon="coins">
    Your wallet needs both tokens in the pair
  </Card>
  <Card title="SOL for Fees" icon="gas-pump">
    Keep 0.1+ SOL for transaction fees
  </Card>
  <Card title="Initial Price" icon="tag">
    Decide the starting price for your token
  </Card>
  <Card title="Fee Tier" icon="percent">
    Choose based on expected volatility
  </Card>
</CardGroup>

### Understanding Fee Tiers

| Fee Tier | Best For | Examples |
|----------|----------|----------|
| **0.01%** | Stablecoin pairs | USDC/USDT |
| **0.05%** | Stable, high-volume | Major stablecoins |
| **0.30%** | Standard pairs | SOL/USDC |
| **1.00%** | Volatile/exotic | Memecoins, new tokens |

<Tip>
Higher fees compensate LPs for volatility risk but may reduce trading volume.
</Tip>

---

## Creating a CLMM Pool

<Steps>
  <Step title="Navigate to Pool Creation">
    Go to [orca.so/create-pool](https://www.orca.so/create-pool), connect your wallet, and select **Create Concentrated Pool**.
  </Step>

  <Step title="Select Your Tokens">
    1. Click **Select Token** to choose your token
    2. Search by name, symbol, or paste the mint address
    3. By default, pairs with SOL (click SOL to change)
  </Step>

  <Step title="Set the Initial Price">
    This is the starting trading price for your pool.

    **Option A: Use Estimated Market Price**
    - Orca shows an estimated price from Jupiter
    - Click to use this price and verify it matches expectations

    **Option B: Enter Custom Price**
    - Type your desired price manually
    - Useful for new tokens without market data

    <Warning>
    The initial price determines where trading begins. Wrong price = immediate arbitrage against your pool.
    </Warning>
  </Step>

  <Step title="Choose Position Type">
    <Tabs>
      <Tab title="Full-Range">
        Creates liquidity across all possible prices (0 to infinity).

        **Pros:** Simpler, always in range
        **Cons:** Lower capital efficiency
      </Tab>
      <Tab title="Custom Range">
        Focus liquidity in a specific price range:
        1. Select **Custom Range**
        2. Set **Min Price** (lower bound)
        3. Set **Max Price** (upper bound)

        **Pros:** Higher capital efficiency when in range
        **Cons:** Requires monitoring
      </Tab>
    </Tabs>
  </Step>

  <Step title="Enter Deposit Amount">
    Enter the amount for one token—the other auto-calculates based on your price range and current price.

    <Note>
    For custom ranges not including current price, you may deposit only one token.
    </Note>
  </Step>

  <Step title="Select Fee Tier">
    Click **Change** to select a different fee tier. Consider your token's volatility when choosing.
  </Step>

  <Step title="Review and Create">
    1. Click **Preview Pool**
    2. Review all parameters carefully
    3. Check the acknowledgment box
    4. Click **Create Pool**
  </Step>

  <Step title="Approve Transactions">
    You'll need to approve **two transactions**:
    1. First initializes the pool
    2. Second deposits liquidity

    Wait for confirmation.
  </Step>
</Steps>

---

## After Creating Your Pool

<AccordionGroup>
  <Accordion title="Verify your pool">
    1. Search for your token on [orca.so](https://www.orca.so)
    2. Confirm the pool appears
    3. Test with a small swap
  </Accordion>

  <Accordion title="Token List">
    If your token shows a warning triangle:
    - It's not yet on the Orca Token List
    - Trading still works, but display is limited
    - [Request token list addition](/create/listings/token-list)
  </Accordion>

  <Accordion title="Add Rewards (Optional)">
    Incentivize more LPs with token rewards:
    [How to Add Rewards →](/create/rewards/overview)
  </Accordion>

  <Accordion title="Monitor your pool">
    - [Orca Portfolio](https://www.orca.so/portfolio) — Track your positions
    - [Account Microscope](https://everlastingsong.github.io/account-microscope/) — View pool state
  </Accordion>
</AccordionGroup>

---

## Troubleshooting

<AccordionGroup>
  <Accordion title="Insufficient Balance">
    - Ensure you have enough of both tokens
    - Keep extra SOL for transaction fees
  </Accordion>

  <Accordion title="Transaction Failed">
    - Try increasing slippage tolerance
    - Ensure sufficient SOL for fees
    - Retry—network congestion can cause failures
  </Accordion>

  <Accordion title="Pool not showing in UI">
    - Wait a few minutes for indexing
    - Refresh the page
    - Clear browser cache if needed
  </Accordion>

  <Accordion title="Price immediately changes after creation">
    This usually means:
    - Initial price differed from market price
    - Arbitrageurs corrected the price
    - Double-check your price setting next time
  </Accordion>
</AccordionGroup>

---

## Best Practices

<CardGroup cols={2}>
  <Card title="Setting Initial Price" icon="tag">
    Match existing market price if your token trades elsewhere. Verify before confirming—price cannot be edited after creation.
  </Card>
  <Card title="Choosing Fee Tier" icon="percent">
    Higher volatility → higher fee tier. When in doubt, 0.30% is a reasonable default.
  </Card>
  <Card title="Managing Your Pool" icon="chart-pie">
    Monitor liquidity levels, watch for price movements out of range, and consider adding rewards.
  </Card>
  <Card title="Tick Arrays" icon="grid">
    CLMM pools use tick arrays. Some may need initialization for unlisted tokens. Reach out via the Support widget if you encounter issues.
  </Card>
</CardGroup>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Splash Pools" icon="droplet" href="/create/pools/splash">
    Simpler pool creation option
  </Card>
  <Card title="Token Extensions" icon="puzzle-piece" href="/create/pools/extensions">
    SPL Token Extension support
  </Card>
  <Card title="Add Rewards" icon="gift" href="/create/rewards/overview">
    Incentivize liquidity providers
  </Card>
  <Card title="Token List" icon="list-check" href="/create/listings/token-list">
    Improve token discoverability
  </Card>
</CardGroup>
