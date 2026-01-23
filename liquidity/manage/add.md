---
title: How to Add Liquidity
description: Add more liquidity to an existing position.
icon: plus
---

Increase your position size by depositing additional tokens into an existing liquidity position.

<Warning>
Due to [impermanent loss](/liquidity/concepts/impermanent-loss), you are not guaranteed a positive return when providing liquidity. Understand the risks before depositing.
</Warning>

---

## How to Add Liquidity

<Steps>
  <Step title="Open the Position Details sidebar">
    Navigate to your [Portfolio](https://www.orca.so/portfolio) and click on the position you want to add liquidity to.

    See the [Position Details Sidebar Guide](/liquidity/manage/sidebar) for a full walkthrough.
  </Step>

  <Step title="Select the Deposit tab">
    In the sidebar, ensure the **Deposit** tab is selected.
  </Step>

  <Step title="Enter deposit amounts">
    Enter the amount you wish to deposit in one of the token fields.

    <Frame caption="Enter your deposit amount in either token field">
      <img src="/images/image_73.jpg" alt="Deposit amount entry" />
    </Frame>

    The other value will auto-adjust to match the deposit ratio required for your existing range.

    <Tip>
    Click **Max** to deposit the maximum quantity of a token from your wallet.
    </Tip>

    <Frame caption="Use Max to deposit all available tokens">
      <img src="/images/image_74.jpg" alt="Max deposit option" />
    </Frame>
  </Step>

  <Step title="(Optional) Use Autoswap">
    If you don't have the right token ratio, **Autoswap** can help by trading one token for the other to match the required ratio.

    Enable Autoswap in the deposit interface if available.
  </Step>

  <Step title="(Optional) Adjust liquidity slippage">
    Click the **Liq. slippage** button to adjust your slippage tolerance if needed.

    See [Understanding Slippage](/trade/slippage) for more information.
  </Step>

  <Step title="Complete your deposit">
    Review the deposit details and click **Deposit**.

    <Frame caption="Click Deposit to add liquidity to your position">
      <img src="/images/image_75.jpg" alt="Deposit confirmation" />
    </Frame>
  </Step>

  <Step title="Approve the transaction">
    Review the details in your wallet—including any network fees—and approve.

    <Warning>
    **Review carefully.** Verify your range and ensure the current pool price matches your intentions. Depositing at a price inconsistent with wider market values may result in loss.
    </Warning>
  </Step>
</Steps>

---

## After Depositing

<Info>
You will **not** receive a new pool position NFT. Your existing NFT continues to represent the updated position with increased liquidity.
</Info>

The NFT remains in your wallet displaying "**DO NOT BURN**."

<Warning>
**Protect your position NFT:**
- **DO NOT** sell or burn this NFT—you'll lose your liquidity
- You can transfer it to another wallet to move your position
- Orca **cannot** recover funds lost from burning position NFTs
</Warning>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Manage Portfolio" icon="chart-pie" href="/liquidity/manage/portfolio">
    View and manage all your positions
  </Card>
  <Card title="Harvest Yield" icon="seedling" href="/liquidity/manage/harvest">
    Collect your earned fees and rewards
  </Card>
  <Card title="Withdraw Liquidity" icon="arrow-up-from-bracket" href="/liquidity/manage/withdraw">
    Remove liquidity from your position
  </Card>
  <Card title="Position Alerts" icon="bell" href="/liquidity/manage/alerts">
    Get notified when positions go out of range
  </Card>
</CardGroup>
