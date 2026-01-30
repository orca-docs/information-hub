---
title: Orca for Token Creators
description: Resources for token creators to launch tokens and pools on Orca.
icon: coins
---

Launch and manage liquid onchain markets for your token. Orca empowers token creators to permissionlessly create tokens and pools without approval.

<Info>
Need help? Open a ticket via the **Support** function in the Orca UI. You can also reach the community on [Discord](https://discord.gg/orca-so) or [Telegram](https://t.me/orca_so).
</Info>

---

## What You Can Do

<CardGroup cols={2}>
  <Card title="Create a Pool" icon="circle-plus" href="/create/pools/splash">
    Launch a liquidity pool for your token so users can trade it
  </Card>
  <Card title="Add Rewards" icon="gift" href="/create/rewards/overview">
    Incentivize liquidity providers with token rewards
  </Card>
  <Card title="List Your Token" icon="list-check" href="/create/listings/token-list">
    Add your token to the Orca Token List for better visibility
  </Card>
  <Card title="Token Extensions" icon="puzzle-piece" href="/create/pools/extensions">
    Learn about SPL Token Extension support
  </Card>
</CardGroup>

---

## Choosing a Pool Type

<CardGroup cols={2}>
  <Card title="Splash Pool" icon="droplet" href="/create/pools/splash">
    **Best for most token launches**

    - Simple setup process
    - Lower creation cost
    - Full-range liquidity only
    - Minimal management needed
  </Card>
  <Card title="CLMM Pool" icon="chart-mixed" href="/create/pools/clmm">
    **For advanced users**

    - Full customization options
    - Custom range positions
    - Multiple fee tiers
    - More complex setup
  </Card>
</CardGroup>

<Tip>
**New to Orca?** Start with a [Splash Pool](/create/pools/splash) for the simplest launch experience.
</Tip>

---

## Launch Checklist

<Steps>
  <Step title="Prepare your token">
    Have your SPL token minted and ready. Ensure you have enough tokens for initial liquidity.
  </Step>
  <Step title="Plan your liquidity">
    Decide how much liquidity to provide and at what initial price.
  </Step>
  <Step title="Create your pool">
    Follow the [Splash Pool](/create/pools/splash) or [CLMM Pool](/create/pools/clmm) guide.
  </Step>
  <Step title="Verify and test">
    Confirm the pool appears in the UI and test with a small swap.
  </Step>
  <Step title="List your token">
    [Apply for the Orca Token List](/create/listings/token-list) to improve discoverability.
  </Step>
  <Step title="(Optional) Add rewards">
    [Incentivize LPs](/create/rewards/overview) to deepen liquidity.
  </Step>
</Steps>

---

## Token Extensions Support

Orca supports SPL Token Extensions for tokens with advanced compliance requirements.

<Card title="Token Extensions Documentation" icon="puzzle-piece" href="/create/pools/extensions">
  Learn about supported extensions and limitations
</Card>

---

## Best Practices

<AccordionGroup>
  <Accordion title="Setting the initial price">
    - If your token already trades elsewhere, match that price
    - For new tokens, set based on your tokenomics
    - **Verify before confirming** — price cannot be changed after creation
  </Accordion>

  <Accordion title="Providing initial liquidity">
    - More liquidity = less price impact for traders
    - Consider starting with enough for reasonable trade sizes
    - You can always add more liquidity later
  </Accordion>

  <Accordion title="Choosing a fee tier">
    | Fee Tier | Best For |
    |----------|----------|
    | 0.01% | Stablecoin pairs |
    | 0.30% | Standard pairs |
    | 1.00% | Volatile/new tokens |
  </Accordion>

  <Accordion title="Getting your token listed">
    - Apply for [Orca Token List](/create/listings/token-list)
    - Consider [CoinGecko listing](/create/listings/coingecko) for price data
    - [Jupiter listing](/create/listings/jupiter) for aggregator routing
  </Accordion>
</AccordionGroup>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Create Splash Pool" icon="droplet" href="/create/pools/splash">
    Simple pool creation for most use cases
  </Card>
  <Card title="Create CLMM Pool" icon="chart-mixed" href="/create/pools/clmm">
    Advanced pool with full customization
  </Card>
  <Card title="Add LP Rewards" icon="gift" href="/create/rewards/overview">
    Incentivize liquidity providers
  </Card>
  <Card title="Token List Application" icon="list-check" href="/create/listings/token-list">
    Get your token officially listed
  </Card>
</CardGroup>
