---
title: Managing Your Portfolio
description: Monitor and manage your liquidity positions on Orca.
icon: chart-pie
---

The Portfolio page is your command center for managing liquidity positions on Orca. View all positions, track performance, harvest fees, and make adjustments.

---

## Accessing Your Portfolio

<Steps>
  <Step title="Visit the Portfolio page">
    Go to [orca.so/portfolio](https://www.orca.so/portfolio)
  </Step>
  <Step title="Connect your wallet">
    Click Connect Wallet and approve the connection
  </Step>
  <Step title="View your positions">
    Your positions load automatically
  </Step>
</Steps>

---

## Portfolio Overview

### What You'll See

<CardGroup cols={2}>
  <Card title="Total Value" icon="sack-dollar">
    Combined USD value of all your positions
  </Card>
  <Card title="Unclaimed Fees" icon="coins">
    Fees ready to harvest across all positions
  </Card>
  <Card title="Positions List" icon="list">
    All your active liquidity positions
  </Card>
  <Card title="Performance Metrics" icon="chart-line">
    APR, fees earned, and value changes
  </Card>
</CardGroup>

### Position Cards

Each position displays:

| Information | Description |
|-------------|-------------|
| **Token pair** | Which tokens you're providing liquidity for |
| **Current value** | USD value of your position |
| **Price range** | Your selected min/max prices |
| **Status** | In range (earning) or out of range |
| **Unclaimed fees** | Accumulated fees to harvest |
| **Fee APR** | Current estimated annual return |

---

## Understanding Position Status

<CardGroup cols={2}>
  <Card title="In Range" icon="circle-check">
    **You're earning fees**

    Current price is within your bounds. The position indicator shows green. Continue monitoring normally.
  </Card>
  <Card title="Out of Range" icon="triangle-exclamation">
    **Not earning fees**

    Price moved outside your bounds. Consider rebalancing, waiting for price to return, or closing the position.
  </Card>
</CardGroup>

<Tip>
Set up [position alerts](/liquidity/manage/alerts) to get notified when your position moves out of range.
</Tip>

---

## Position Management Actions

<AccordionGroup>
  <Accordion title="View Details" icon="eye">
    Click on any position to see:
    - Detailed token balances
    - Price range visualization
    - Fee breakdown
    - Performance history
    - Available actions
  </Accordion>

  <Accordion title="Harvest Fees" icon="seedling">
    Collect accumulated fees:
    1. Click on the position
    2. Click **Harvest**
    3. Approve the transaction

    [Detailed Harvest Guide →](/liquidity/manage/harvest)
  </Accordion>

  <Accordion title="Add Liquidity" icon="plus">
    Increase your position:
    1. Click on the position
    2. Click **Add Liquidity**
    3. Enter amount and approve

    [Adding Liquidity Guide →](/liquidity/manage/add)
  </Accordion>

  <Accordion title="Withdraw Liquidity" icon="arrow-up-from-bracket">
    Reduce or close your position:
    1. Click on the position
    2. Click **Withdraw** or **Close Position**
    3. Enter amount and approve

    [Withdrawal Guide →](/liquidity/manage/withdraw)
  </Accordion>
</AccordionGroup>

---

## Understanding Position NFTs

<Info>
Your liquidity positions are represented by NFTs. Each position = one unique NFT in your wallet that proves ownership.
</Info>

### Why This Matters

- Whoever holds the NFT **controls the position**
- Transferring the NFT transfers the entire position
- Burning the NFT means **permanent loss** of your position

<Warning>
**Protect your position NFTs:**
- Never burn position NFTs
- Don't transfer unless intentionally moving the position
- Keep NFTs in your primary wallet
- Beware of scams asking you to send NFTs
</Warning>

### Transferring Positions

To move a position to another wallet:

1. Transfer the position NFT to the new wallet
2. The new wallet can now manage the position
3. The original wallet loses access

Useful for:
- Moving to a hardware wallet
- Transferring to a multisig
- Selling positions (advanced)

---

## Tracking Performance

### Key Metrics

| Metric | What It Tells You |
|--------|------------------|
| **Position Value** | Current worth of deposited tokens |
| **Fees Earned** | Total fees collected over time |
| **Fee APR** | Annualized return from fees |
| **Time in Range** | How long you've been earning |
| **Impermanent Loss** | Value change vs. holding |

### Calculating Real Returns

```
Actual Return = Fees Earned - Impermanent Loss
```

- If IL is negative (you lost value), fees may offset it
- Even with IL, total return can be positive if fees are high
- Track both metrics to understand true performance

---

## Best Practices

<AccordionGroup>
  <Accordion title="Regular Monitoring">
    | Position Type | Check Frequency |
    |---------------|-----------------|
    | Full-range | Weekly or less |
    | Wide custom range | Every few days |
    | Tight custom range | Daily |

    Set up [alerts](/liquidity/manage/alerts) for automated monitoring.
  </Accordion>

  <Accordion title="Harvest Timing">
    Consider harvesting:
    - When fees reach a meaningful amount (relative to network fees)
    - Before making any position changes
    - For tax tracking purposes
    - To compound earnings back into the position
  </Accordion>

  <Accordion title="When to Adjust">
    Consider adjusting positions when:
    - Out of range for extended periods
    - Market conditions change significantly
    - Better opportunities emerge
    - You want to realize gains/losses
  </Accordion>
</AccordionGroup>

---

## Troubleshooting

<AccordionGroup>
  <Accordion title="Position not showing">
    1. **Check wallet connection** — Reconnect if needed
    2. **Refresh the page** — Wait for data to load
    3. **Verify correct wallet** — Ensure you're using the right address
    4. **Check NFT ownership** — Position NFT must be in connected wallet
  </Accordion>

  <Accordion title="Incorrect values displayed">
    1. **Refresh the page** — Prices update in real-time
    2. **Check network status** — Solana RPC issues can cause delays
    3. **Clear browser cache** — May show stale data
  </Accordion>

  <Accordion title="Can't interact with position">
    1. **Verify NFT ownership** — Must be in connected wallet
    2. **Check SOL balance** — Need SOL for transaction fees
    3. **Try again** — Network congestion can cause failures
  </Accordion>
</AccordionGroup>

---

## Security Tips

<CardGroup cols={2}>
  <Card title="Protect NFTs" icon="shield">
    Never share or transfer position NFTs unless intentionally moving positions
  </Card>
  <Card title="Use Hardware Wallet" icon="usb">
    Consider hardware wallets for large positions
  </Card>
  <Card title="Verify Transactions" icon="magnifying-glass">
    Always review transaction details before approving
  </Card>
  <Card title="Avoid Scams" icon="user-secret">
    Never click links from DMs or transfer NFTs to unknown addresses
  </Card>
</CardGroup>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Position Sidebar" icon="sidebar" href="/liquidity/manage/sidebar">
    Quick actions for position management
  </Card>
  <Card title="Harvest Yield" icon="seedling" href="/liquidity/manage/harvest">
    Collect your earned fees
  </Card>
  <Card title="Add Liquidity" icon="plus" href="/liquidity/manage/add">
    Increase your positions
  </Card>
  <Card title="Position Alerts" icon="bell" href="/liquidity/manage/alerts">
    Set up automated notifications
  </Card>
</CardGroup>
