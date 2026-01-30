---
title: How to Swap Tokens
description: Step-by-step guide to swapping tokens on Orca.
icon: arrow-right-arrow-left
---

Trade any token on Solana in seconds with Orca's intuitive swap interface.

<Info>
Orca compares quotes from its own pools and Jupiter aggregator, so you always get the best price without leaving the app.
</Info>

---

## Before You Start

<CardGroup cols={3}>
  <Card title="Solana Wallet" icon="wallet">
    Phantom, Backpack, or any supported wallet
  </Card>
  <Card title="SOL for Fees" icon="coin">
    Keep at least 0.05 SOL for network fees
  </Card>
  <Card title="Tokens to Trade" icon="coins">
    The token you want to swap
  </Card>
</CardGroup>

<Tip>
New to Solana? See our [wallet setup guide](/support/wallets) to get started.
</Tip>

---

## How to Swap

<Steps>
  <Step title="Go to Orca and connect your wallet">
    Visit [orca.so](https://www.orca.so) and click **Connect Wallet** in the top right corner (or center of the trading modal on mobile).

    Select your wallet from the list and approve the connection.
  </Step>

  <Step title="Select your tokens">
    In the swap interface:
    - Click the top token selector to choose the token you want to **sell** (pay with)
    - Click the bottom token selector to choose the token you want to **buy** (receive)

    <Frame caption="Select tokens using the dropdown or search by name, ticker, or mint address">
      <img src="/images/image_61.jpg" alt="Token selection interface" />
    </Frame>
  </Step>

  <Step title="Enter the amount">
    Type the amount you want to swap in either field:
    - Enter in the **top field** to specify how much you're selling
    - Enter in the **bottom field** to specify how much you want to receive

    Use **Half** or **Max** buttons for quick amounts.

    <Frame caption="Enter your swap amount and see the live quote">
      <img src="/images/image_62.jpg" alt="Swap amount entry" />
    </Frame>
  </Step>

  <Step title="Review the quote">
    Check the swap details:
    - **Rate** — Current exchange rate
    - **Price impact** — How your trade affects the price
    - **Minimum received** — Guaranteed minimum after slippage

    Click the dropdown arrow to see more details.

    <Frame caption="Review full trade details before confirming">
      <img src="/images/image_63.jpg" alt="Swap quote details" />
    </Frame>
  </Step>

  <Step title="Compare prices (optional)">
    Orca shows you quotes from both:
    - **Orca Direct** — Trading through Orca's pools
    - **Jupiter** — Aggregated from multiple DEXs

    The better price is highlighted. Choose your preferred option.
  </Step>

  <Step title="Adjust slippage (optional)">
    Click the **gear icon** (⚙️) to adjust slippage tolerance if needed.

    | Pair Type | Recommended Slippage |
    |-----------|---------------------|
    | Stablecoins | 0.1% |
    | Major pairs (SOL/USDC) | 0.5% |
    | Volatile tokens | 1-3% |

    See [Understanding Slippage](/trade/slippage) for more details.
  </Step>

  <Step title="Execute the swap">
    Click **Trade** (or **Swap**) and approve the transaction in your wallet.

    The UI will show progress and confirm when complete.
  </Step>
</Steps>

---

## After Your Swap

<AccordionGroup>
  <Accordion title="Where are my tokens?">
    Swapped tokens appear in your wallet immediately after the transaction confirms. Check your wallet's token list—you may need to add the token if it's new to your wallet.
  </Accordion>

  <Accordion title="Why did I receive less than quoted?">
    The final amount can differ slightly due to:
    - **Slippage** — Price moved between quote and execution
    - **Price impact** — Your trade size affected the price

    You'll never receive less than the "Minimum received" shown.
  </Accordion>

  <Accordion title="My transaction failed—what now?">
    Common causes and fixes:
    - **Slippage too low** — Increase slippage tolerance
    - **Insufficient SOL** — Add more SOL for fees
    - **Price moved** — Try again with updated quote

    See [FAQs](/support/faqs) for more troubleshooting.
  </Accordion>
</AccordionGroup>

---

## Tips for Better Trades

<CardGroup cols={2}>
  <Card title="Check Price Impact" icon="chart-line">
    High price impact means you're moving the market. Consider splitting large trades or using a pool with more liquidity.
  </Card>
  <Card title="Verify Token Addresses" icon="shield-check">
    Always verify token mint addresses, especially for new or unfamiliar tokens. Scam tokens often mimic popular names.
  </Card>
  <Card title="Start Small" icon="flask">
    Testing with a small amount first is always a good practice, especially with new tokens or large trades.
  </Card>
  <Card title="Compare Quotes" icon="scale-balanced">
    Use Orca's built-in comparison to ensure you're getting the best deal between Orca and Jupiter.
  </Card>
</CardGroup>

<Warning>
**Always verify your transaction details in your wallet before approving.** Check the tokens, amounts, and destination address carefully.
</Warning>

---

## Get SOL for Fees

If you need SOL for transaction fees:

1. **From a centralized exchange** — Buy SOL and withdraw to your wallet address
2. **Through a fiat on-ramp** — Some wallets have built-in purchase options
3. **Bridge from another chain** — Use a bridge if you have assets elsewhere

<Note>
When withdrawing from an exchange, ensure you select the **Solana (SPL)** network. Test with a small amount first.
</Note>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Understanding Slippage" icon="sliders" href="/trade/slippage">
    Learn how slippage works and how to protect your trades
  </Card>
  <Card title="Range Orders" icon="crosshairs" href="/trade/range-orders">
    Set limit-order-style trades that earn fees while waiting
  </Card>
  <Card title="Provide Liquidity" icon="droplet" href="/liquidity/getting-started/beginner-guide">
    Earn trading fees by providing liquidity
  </Card>
  <Card title="FAQs" icon="circle-question" href="/support/faqs">
    Common questions and troubleshooting
  </Card>
</CardGroup>
