---
title: How to Create a Custom-Range Position
description: Create concentrated liquidity positions with custom price ranges for higher yields.
icon: crosshairs
---

Custom-range positions let you **concentrate liquidity** within specific price ranges. This increases capital efficiency and potential yields—but requires more active management.

<Warning>
Custom-range positions are an **advanced feature**. They require understanding of impermanent loss and active position management. Read [Impermanent Loss](/liquidity/concepts/impermanent-loss) before proceeding.
</Warning>

<CardGroup cols={2}>
  <Card title="Pros" icon="circle-check">
    - Higher capital efficiency
    - Greater fee earnings potential
    - More control over your position
  </Card>
  <Card title="Cons" icon="circle-xmark">
    - Can go out of range (stop earning)
    - Higher impermanent loss risk
    - Requires active monitoring
  </Card>
</CardGroup>

---

## How to Create a Custom-Range Position

<Steps>
  <Step title="Navigate to the Pools page">
    Go to [orca.so/pools](https://www.orca.so/pools)

    <Warning>
    Always verify the URL in your browser before connecting your wallet.
    </Warning>
  </Step>

  <Step title="Connect your wallet">
    Click **Connect Wallet** and ensure both the UI and your wallet are set to the Solana network.
  </Step>

  <Step title="Find your pool">
    Locate your pool using the list or search by token name, ticker, or mint address.

    <Tip>
    Verify you've selected the correct token by checking the mint address.
    </Tip>
  </Step>

  <Step title="Open the Liquidity Terminal">
    Click on your chosen pool to open the Liquidity Terminal.
  </Step>

  <Step title="Select Custom range">
    In the Create Position sidebar, select **Custom**.

    <Frame caption="Select Custom to set your own price range">
      <img src="/images/image_157.jpg" alt="Custom range selection" />
    </Frame>
  </Step>

  <Step title="Set your price range">
    Define your range using any of these methods:
    - **Drag the sliders** in the sidebar
    - **Drag range boundaries** on the price chart
    - **Select a preset** (±5%, ±10%, etc.)
    - **Type a custom percentage** range
    - **Enter specific prices** in the lower/upper fields
    - **Use +/- buttons** for fine adjustments

    <Frame caption="Multiple ways to set your custom range">
      <img src="/images/image_158.jpg" alt="Range adjustment options" />
    </Frame>

    <Tip>
    **Narrower ranges** = higher capital efficiency but more likely to go out of range.
    **Wider ranges** = lower efficiency but more stable earnings.
    </Tip>
  </Step>

  <Step title="Enter deposit amounts">
    Enter your deposit amount in one of the token fields.

    <Frame caption="Enter your deposit amount">
      <img src="/images/image_159.jpg" alt="Deposit amount entry" />
    </Frame>

    The other value auto-adjusts based on your chosen range and current price.

    <Note>
    If current price is outside your range, you'll only deposit one token (single-sided position).
    </Note>

    Options:
    - Type a specific amount
    - Click **Max** to use your full balance
    - Use **Autoswap** to balance your tokens
  </Step>

  <Step title="(Optional) Adjust liquidity slippage">
    Click **Liq. slippage** to adjust tolerance if needed.

    See [Understanding Slippage](/trade/slippage) for details.
  </Step>

  <Step title="Complete your deposit">
    Review and click **Deposit**.

    <Frame caption="Click Deposit to create your position">
      <img src="/images/image_160.jpg" alt="Deposit confirmation" />
    </Frame>
  </Step>

  <Step title="Approve the transaction">
    Review the details in your wallet and approve.

    <Warning>
    **Review carefully.** Verify your range and ensure the pool price matches wider market values. Incorrect settings may result in loss.
    </Warning>
  </Step>
</Steps>

---

## After Creating Your Position

<Info>
Your wallet now contains a **position NFT** representing your liquidity. It displays "**DO NOT BURN**".
</Info>

<Warning>
**Protect your position NFT:**
- **DO NOT** sell or burn this NFT—you'll lose your liquidity
- Orca **cannot** recover funds lost from burning position NFTs
</Warning>

---

## Managing Your Custom-Range Position

Custom-range positions require monitoring:

<AccordionGroup>
  <Accordion title="Monitor in-range status">
    Your position only earns fees when the current price is **within your range**. Check your [Portfolio](https://www.orca.so/portfolio) regularly or set up [alerts](/liquidity/manage/alerts).
  </Accordion>

  <Accordion title="What to do when out of range">
    If price moves outside your range:
    - **Wait** for price to return (if you expect it to)
    - **Close and reopen** with a new range around current price
    - **Accept it** if using as a [range order](/trade/range-orders)
  </Accordion>

  <Accordion title="Rebalancing strategies">
    Some LPs regularly close and reopen positions to stay centered on current price. This can maximize fee earnings but incurs transaction costs.
  </Accordion>
</AccordionGroup>

---

## Choosing Your Range

| Strategy | Range Width | Best For |
|----------|-------------|----------|
| **Tight** (±1-5%) | Very narrow | Stablecoin pairs, short-term trades |
| **Medium** (±10-25%) | Moderate | Active LPs, volatile pairs |
| **Wide** (±50%+) | Broad | Less monitoring, longer holds |

<Tip>
Use the [Position Simulator](/liquidity/advanced/simulator) to visualize how different ranges might perform.
</Tip>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Manage Portfolio" icon="chart-pie" href="/liquidity/manage/portfolio">
    Monitor and manage your positions
  </Card>
  <Card title="Position Simulator" icon="chart-line" href="/liquidity/advanced/simulator">
    Visualize potential performance
  </Card>
  <Card title="Position Alerts" icon="bell" href="/liquidity/manage/alerts">
    Get notified when out of range
  </Card>
  <Card title="LP Strategies" icon="lightbulb" href="/liquidity/advanced/strategies">
    Learn advanced LP techniques
  </Card>
</CardGroup>
