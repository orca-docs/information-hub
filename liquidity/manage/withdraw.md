---
title: How to Withdraw Liquidity
description: Withdraw liquidity from your positions.
icon: arrow-up-from-bracket
---

Remove some or all liquidity from an existing position to reclaim your tokens.

---

## How to Withdraw

<Steps>
  <Step title="Open the Position Details sidebar">
    Navigate to your [Portfolio](https://www.orca.so/portfolio) and click on the position you want to withdraw from.

    See the [Position Details Sidebar Guide](/liquidity/manage/sidebar) for a full walkthrough.
  </Step>

  <Step title="Select the Withdraw tab">
    In the sidebar, click the **Withdraw** tab.
  </Step>

  <Step title="Enter withdrawal amount">
    Choose how much to withdraw:
    - **Enter a specific amount** in one of the token fields
    - **Use the slider** to select a percentage of your position
    - **Click Max** to withdraw everything

    <Frame caption="Enter withdrawal amount or use the slider">
      <img src="/images/image_94.jpg" alt="Withdrawal amount entry" />
    </Frame>

    The other token value will auto-adjust based on your current position ratio.

    <Frame caption="Click Max to withdraw all liquidity">
      <img src="/images/image_95.jpg" alt="Max withdrawal option" />
    </Frame>
  </Step>

  <Step title="(Optional) Adjust liquidity slippage">
    Click the **Liq. slippage** button to adjust tolerance if needed.

    See [Understanding Slippage](/trade/slippage) for more information.
  </Step>

  <Step title="Complete your withdrawal">
    Click **Withdraw** to proceed.

    <Frame caption="Click Withdraw to remove liquidity">
      <img src="/images/image_96.jpg" alt="Withdraw button" />
    </Frame>

    <Note>
    If you're removing **all** liquidity, the button changes to **Close Position**.
    </Note>

    <Frame caption="Close Position appears when removing all liquidity">
      <img src="/images/image_97.jpg" alt="Close Position button" />
    </Frame>
  </Step>

  <Step title="(Optional) Keep your position NFT">
    When closing a position, you can **retain the NFT** by unchecking "Harvest and burn the NFT of this position."

    <Frame caption="Uncheck to keep your NFT for future use">
      <img src="/images/image_98.jpg" alt="Keep NFT option" />
    </Frame>

    <Tip>
    Keeping the NFT allows you to redeposit into the same price range later without creating a new position.
    </Tip>
  </Step>

  <Step title="Approve the transaction">
    Review the details in your wallet—including network fees—and approve.
  </Step>
</Steps>

---

## Partial vs Full Withdrawal

<CardGroup cols={2}>
  <Card title="Partial Withdrawal" icon="percent">
    Remove some liquidity while keeping the position active. Good for taking profits or reducing exposure.
  </Card>
  <Card title="Full Withdrawal (Close)" icon="xmark">
    Remove all liquidity and optionally burn the position NFT. Completely exits the position.
  </Card>
</CardGroup>

---

## What Happens to Your Tokens

When you withdraw:
- **Tokens return to your wallet** immediately after transaction confirms
- **Uncollected fees** are harvested automatically during withdrawal
- **Token ratio** depends on current price relative to your range

<Info>
If your position is **out of range**, you'll receive 100% of one token (the one that decreased in value relative to your range).
</Info>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Manage Portfolio" icon="chart-pie" href="/liquidity/manage/portfolio">
    View all your positions
  </Card>
  <Card title="Close Position" icon="xmark" href="/liquidity/manage/close">
    Fully close a position
  </Card>
  <Card title="Add Liquidity" icon="plus" href="/liquidity/manage/add">
    Increase an existing position
  </Card>
  <Card title="Beginner's Guide" icon="graduation-cap" href="/liquidity/getting-started/beginner-guide">
    Learn the basics of liquidity provision
  </Card>
</CardGroup>
