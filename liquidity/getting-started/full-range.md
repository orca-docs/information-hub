---
title: How to Create a Full-Range Position
description: Create your first full-range liquidity position on Orca.
icon: arrows-left-right
---

A full-range position spreads your liquidity across **all possible prices** (0 to infinity). This is the simplest way to provide liquidity on Orca.

<CardGroup cols={2}>
  <Card title="Pros" icon="circle-check">
    - Simple to create and manage
    - Always earning fees (never out of range)
    - Lower impermanent loss risk
  </Card>
  <Card title="Cons" icon="circle-xmark">
    - Less capital efficient
    - Lower potential yields
    - Similar to traditional AMM
  </Card>
</CardGroup>

<Tip>
Full-range positions are ideal for **beginners** or those who prefer a hands-off approach. For higher yields with more active management, consider [custom-range positions](/liquidity/getting-started/custom-range).
</Tip>

---

## How to Create a Full-Range Position

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
    Locate the pool you want to add liquidity to:
    - Browse the pool list, or
    - Use the search field to find by token name, ticker, or mint address

    <Frame caption="Search for pools by token name, ticker, or address">
      <img src="/images/image_64.jpg" alt="Pool search interface" />
    </Frame>

    <Tip>
    Verify you've selected the correct token—check the mint address if unsure.
    </Tip>
  </Step>

  <Step title="Open the Liquidity Terminal">
    Click on your chosen pool to open the Liquidity Terminal.

    <Frame caption="The Liquidity Terminal shows pool details and position creation">
      <img src="/images/image_65.jpg" alt="Liquidity Terminal" />
    </Frame>
  </Step>

  <Step title="Select Full range">
    In the Create Position sidebar, ensure **Full** is selected.

    <Frame caption="Select Full for a full-range position">
      <img src="/images/image_66.jpg" alt="Full range selection" />
    </Frame>
  </Step>

  <Step title="Enter deposit amounts">
    Enter the amount to deposit in one of the token fields. The other value auto-adjusts to match the required ratio.

    <Frame caption="Enter your deposit amount">
      <img src="/images/image_67.jpg" alt="Deposit amount entry" />
    </Frame>

    Options:
    - Type a specific amount
    - Click **Max** to deposit your full wallet balance
    - Use **Autoswap** to automatically balance your token ratio

    See [Understanding Slippage](/trade/slippage) if you need to adjust slippage settings.
  </Step>

  <Step title="Complete your deposit">
    Review your deposit and click **Deposit**.

    <Frame caption="Click Deposit to create your position">
      <img src="/images/image_68.jpg" alt="Deposit button" />
    </Frame>
  </Step>

  <Step title="Approve the transaction">
    Review the details in your wallet—including network fees—and approve.

    <Warning>
    **Review carefully.** Verify the pool price matches wider market values. Depositing at an incorrect price may result in immediate loss.
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
- You can transfer it to move your position to another wallet
- Orca **cannot** recover funds lost from burning position NFTs
</Warning>

Click **View Details** to see your transaction on Solscan.

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Manage Your Portfolio" icon="chart-pie" href="/liquidity/manage/portfolio">
    View and manage your positions
  </Card>
  <Card title="Harvest Yield" icon="seedling" href="/liquidity/manage/harvest">
    Collect your earned fees
  </Card>
  <Card title="Custom-Range Position" icon="crosshairs" href="/liquidity/getting-started/custom-range">
    Try concentrated liquidity for higher yields
  </Card>
  <Card title="Position Alerts" icon="bell" href="/liquidity/manage/alerts">
    Get notified about your positions
  </Card>
</CardGroup>
