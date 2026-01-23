---
title: How to Close a Position
description: Close a liquidity position and withdraw all funds.
icon: xmark
---

Completely exit a liquidity position, withdrawing all tokens and accumulated fees.

<Info>
Closing a position automatically harvests any uncollected fees and returns all tokens to your wallet.
</Info>

---

## How to Close a Position

<Steps>
  <Step title="Go to your Portfolio">
    Navigate to [orca.so/portfolio](https://www.orca.so/portfolio) and connect your wallet.
  </Step>

  <Step title="Find your position">
    Locate the position you want to close in your positions list.
  </Step>

  <Step title="Open the position menu">
    Click the **...** (ellipsis) button on the right side of the position.

    <Frame caption="Click the ellipsis menu to see position actions">
      <img src="/images/image_76.jpg" alt="Position menu" />
    </Frame>
  </Step>

  <Step title="Select Close Position">
    Choose **× Close Position** from the dropdown menu.
  </Step>

  <Step title="Review the details">
    A confirmation modal shows:
    - Tokens you'll receive
    - Fees being harvested
    - Whether the NFT will be burned

    <Frame caption="Review what you'll receive before confirming">
      <img src="/images/image_77.jpg" alt="Close position confirmation" />
    </Frame>
  </Step>

  <Step title="Confirm and close">
    Click **Close Position**, then review and approve the transaction in your wallet.
  </Step>
</Steps>

---

## What Happens When You Close

<CardGroup cols={2}>
  <Card title="Tokens Returned" icon="wallet">
    All deposited tokens return to your wallet immediately
  </Card>
  <Card title="Fees Harvested" icon="coins">
    Any uncollected fees are automatically harvested
  </Card>
  <Card title="NFT Burned" icon="fire">
    The position NFT is burned by default (optional to keep)
  </Card>
  <Card title="Position Removed" icon="trash">
    The position no longer appears in your portfolio
  </Card>
</CardGroup>

---

## Keep vs Burn the NFT

When closing, you can choose to **keep the position NFT**:

<CardGroup cols={2}>
  <Card title="Burn NFT (Default)" icon="fire">
    **Choose if:**
    - You don't plan to reopen this exact range
    - You want a clean portfolio
    - You're done with this position
  </Card>
  <Card title="Keep NFT" icon="bookmark">
    **Choose if:**
    - You might want to redeposit into the same range
    - You want to preserve the position parameters
    - You're temporarily exiting
  </Card>
</CardGroup>

<Tip>
Keeping the NFT allows you to add liquidity back to the **exact same price range** later without creating a new position.
</Tip>

---

## Alternative: Withdraw All

You can also close a position using the [Withdraw](/liquidity/manage/withdraw) function:

1. Open the position sidebar
2. Go to the **Withdraw** tab
3. Click **Max** or set to 100%
4. The button changes to **Close Position**

Both methods achieve the same result.

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Open New Position" icon="plus" href="/liquidity/getting-started/beginner-guide">
    Start a new liquidity position
  </Card>
  <Card title="View Portfolio" icon="chart-pie" href="/liquidity/manage/portfolio">
    Manage your remaining positions
  </Card>
  <Card title="Trading" icon="arrow-right-arrow-left" href="/trade/how-to-swap">
    Swap tokens on Orca
  </Card>
  <Card title="Range Orders" icon="crosshairs" href="/trade/range-orders">
    Use positions as limit orders
  </Card>
</CardGroup>
