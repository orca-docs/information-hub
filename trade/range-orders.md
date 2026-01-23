---
title: Range Orders
description: Use concentrated liquidity positions as limit orders to buy low or sell high.
icon: crosshairs
---

Range orders let you set limit-order-style trades that **earn fees while waiting to execute**. Buy tokens at lower prices or sell at higher prices—automatically.

<Info>
Range orders use Orca's concentrated liquidity pools. Unlike traditional limit orders that cost fees, you **earn** trading fees while your order is active.
</Info>

---

## How Range Orders Work

By creating a single-sided liquidity position outside the current price, you can:

- **Buy tokens** when price drops to your target
- **Sell tokens** when price rises to your target
- **Earn fees** as price moves through your range

<CardGroup cols={2}>
  <Card title="Buy Limit Order" icon="arrow-trend-down">
    Deposit stablecoins below current price. When price drops through your range, your stablecoins convert to the target token.
  </Card>
  <Card title="Sell/Take Profit Order" icon="arrow-trend-up">
    Deposit tokens above current price. When price rises through your range, your tokens convert to stablecoins.
  </Card>
</CardGroup>

---

## Advantages Over Traditional Limit Orders

| Feature | CLOB Limit Order | Orca Range Order |
|---------|------------------|------------------|
| **Fees** | Often pay fees | Earn fees |
| **Tax timing** | Taxable on execution | Taxable on withdrawal* |
| **Partial fills** | Yes | Yes (gradual conversion) |
| **Price precision** | Exact price | Price range |

<Note>
*Tax treatment varies by jurisdiction. Consult a tax professional for your specific situation.
</Note>

---

## Limitations to Understand

<Warning>
Range orders are **not identical** to traditional limit orders. Key differences:

- **Must withdraw to complete**: Your order isn't "done" until you withdraw. If you don't withdraw, price can move back and reverse the conversion.
- **Price range, not exact price**: You set a range, not a single price point.
- **Requires monitoring**: You need to watch for execution and withdraw at the right time.
</Warning>

---

## Creating a Buy Limit Order

Use this when you want to **buy tokens at a lower price** than current market.

**Example scenario**: SOL is at $160 and you want to buy at $150.

<Steps>
  <Step title="Navigate to the pool">
    Go to [orca.so/pools](https://www.orca.so/pools) and find the pool (e.g., SOL/USDC).

    <Frame>
      <img src="/images/image_130.jpg" alt="Pool selection" />
    </Frame>
  </Step>

  <Step title="Connect your wallet">
    Click **Connect Wallet** if not already connected.

    <Frame>
      <img src="/images/image_131.jpg" alt="Connect wallet" />
    </Frame>
  </Step>

  <Step title="Open position creation">
    Click on the pool to open the liquidity sidebar, then click **New Position**.
  </Step>

  <Step title="Select Custom range">
    Choose **Custom** range mode to set your own price bounds.
  </Step>

  <Step title="Set your buy range BELOW current price">
    Set both min and max prices **below** the current price where you want to buy.

    **Example**: To buy SOL around $150:
    - Min: $150.00
    - Max: $150.02 (tight range for precise entry)

    <Tip>
    Use a **tight range** for more precise price execution, or a **wider range** to earn more fees during a protracted downtrend.
    </Tip>
  </Step>

  <Step title="Deposit only the quote token">
    Enter the amount of **USDC** (or other stablecoin) you want to use. Since your range is below current price, you'll only deposit the quote token.

    <Frame>
      <img src="/images/image" alt="Deposit interface" />
    </Frame>
  </Step>

  <Step title="Review and create position">
    - Verify your range is **below** current price
    - Check the deposit amount
    - Click **Deposit** and approve in your wallet
  </Step>

  <Step title="Wait for price to reach your range">
    Monitor your position. When price falls through your range, your USDC converts to SOL.
  </Step>

  <Step title="Withdraw to complete the order">
    Once price is at or below your range minimum, **withdraw immediately** to lock in your purchase. If you don't withdraw, price could rise back and convert your SOL back to USDC.
  </Step>
</Steps>

<Warning>
**Critical**: You must withdraw your position after the price passes through your range. Otherwise, if price reverses, your tokens will convert back.
</Warning>

---

## Creating a Sell/Take Profit Order

Use this when you want to **sell tokens at a higher price** than current market.

**Example scenario**: SOL is at $160 and you want to sell at $170.

<Steps>
  <Step title="Navigate to the pool">
    Go to [orca.so/pools](https://www.orca.so/pools) and find the pool (e.g., SOL/USDC).
  </Step>

  <Step title="Connect your wallet">
    Click **Connect Wallet** if not already connected.
  </Step>

  <Step title="Open position creation">
    Click on the pool to open the liquidity sidebar.
  </Step>

  <Step title="Select Custom range">
    Choose **Custom** range mode.
  </Step>

  <Step title="Set your sell range ABOVE current price">
    Set both min and max prices **above** the current price where you want to sell.

    **Example**: To sell SOL around $170:
    - Min: $170.00
    - Max: $170.02 (tight range for precise exit)
  </Step>

  <Step title="Deposit only the base token">
    Enter the amount of **SOL** you want to sell. Since your range is above current price, you'll only deposit the base token.
  </Step>

  <Step title="Review and create position">
    - Verify your range is **above** current price
    - Check the deposit amount
    - Click **Deposit** and approve in your wallet
  </Step>

  <Step title="Wait for price to reach your range">
    Monitor your position. When price rises through your range, your SOL converts to USDC.
  </Step>

  <Step title="Withdraw to complete the order">
    Once price is at or above your range maximum, **withdraw immediately** to lock in your sale.
  </Step>
</Steps>

---

## Tight Range vs Wide Range

<CardGroup cols={2}>
  <Card title="Tight Range" icon="crosshairs">
    **Pros:**
    - More precise entry/exit price
    - Executes quickly once price reaches range

    **Cons:**
    - Earns fewer fees
    - May miss if price doesn't reach exact level
  </Card>

  <Card title="Wide Range" icon="arrows-left-right">
    **Pros:**
    - Earns more fees during price movement
    - Catches price over broader range

    **Cons:**
    - Average price less precise
    - Takes longer to fully convert
  </Card>
</CardGroup>

**Wide range example**: Instead of $150-$150.02, set $150-$160. As price falls through this range, you gradually buy SOL at various prices, averaging out your entry while earning fees.

---

## Important Reminders

<AccordionGroup>
  <Accordion title="Always verify pool price matches market">
    Before depositing, ensure the pool's current price matches wider market values. Depositing to a mispriced pool can result in immediate loss.
  </Accordion>

  <Accordion title="Withdraw promptly after execution">
    If you don't withdraw after your range order executes, price can reverse and undo your trade. Set alerts or check regularly.
  </Accordion>

  <Accordion title="Consider using Alerts">
    Set up [position alerts](/liquidity/manage/alerts) to get notified when your position moves out of range—signaling your order has executed.
  </Accordion>

  <Accordion title="Account for slippage on withdrawal">
    When withdrawing, there's a small slippage tolerance. This is normal and won't significantly affect your results.
  </Accordion>
</AccordionGroup>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Position Alerts" icon="bell" href="/liquidity/manage/alerts">
    Get notified when your range order executes
  </Card>
  <Card title="Understanding Slippage" icon="sliders" href="/trade/slippage">
    Learn about slippage settings for LP
  </Card>
  <Card title="Beginner's Guide" icon="graduation-cap" href="/liquidity/getting-started/beginner-guide">
    Full introduction to liquidity provision
  </Card>
  <Card title="Managing Positions" icon="chart-pie" href="/liquidity/manage/portfolio">
    Monitor and manage your positions
  </Card>
</CardGroup>
