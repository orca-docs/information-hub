---
title: How to Harvest Yield
description: Collect your earned trading fees and rewards.
icon: seedling
---

Harvest your accumulated trading fees and rewards from liquidity positions to your wallet.

<Info>
Fees accumulate automatically as trades occur in your range. You can harvest anytime—there's no lockup period.
</Info>

---

## Two Ways to Harvest

<CardGroup cols={2}>
  <Card title="Harvest All" icon="layer-group">
    Collect fees from all positions in one transaction. Fastest for multiple positions.
  </Card>
  <Card title="Harvest Single" icon="crosshairs">
    Collect fees from one specific position. Useful for selective harvesting.
  </Card>
</CardGroup>

---

## Harvest All Positions

The quickest way to collect all your pending fees:

<Steps>
  <Step title="Go to Portfolio">
    Navigate to the [Portfolio page](https://www.orca.so/portfolio)
  </Step>
  <Step title="Click Harvest All">
    Find the **Harvest All** button in the top right of the page
  </Step>
  <Step title="Approve the transaction">
    Review the details in your wallet—including network fees—and approve
  </Step>
</Steps>

---

## Harvest Single Position

To harvest from one specific position:

<Tabs>
  <Tab title="Quick Method">
    <Steps>
      <Step title="Go to Portfolio">
        Navigate to the [Portfolio page](https://www.orca.so/portfolio)
      </Step>
      <Step title="Find your position">
        Locate the position you want to harvest from
      </Step>
      <Step title="Open the menu">
        Click the **...** (ellipsis) button on the right side of the position
      </Step>
      <Step title="Select Harvest Yield">
        Choose **Harvest Yield** from the dropdown menu
      </Step>
      <Step title="Approve the transaction">
        Review and approve in your wallet
      </Step>
    </Steps>
  </Tab>

  <Tab title="Sidebar Method">
    <Steps>
      <Step title="Open Position Details">
        Click on the position to open the sidebar
      </Step>
      <Step title="Click Harvest">
        Find and click the **Harvest** button in the position details
      </Step>
      <Step title="Approve the transaction">
        Review and approve in your wallet
      </Step>
    </Steps>

    See the [Position Details Sidebar Guide](/liquidity/manage/sidebar) for more.
  </Tab>
</Tabs>

---

## When to Harvest

<AccordionGroup>
  <Accordion title="Fees reach a meaningful amount">
    Network fees cost ~$0.001-0.01 per harvest. Wait until accumulated fees significantly exceed this cost.
  </Accordion>

  <Accordion title="Before making position changes">
    Fees are automatically harvested when you withdraw or close. But if you're adding liquidity, harvest first to ensure accurate tracking.
  </Accordion>

  <Accordion title="For tax or accounting purposes">
    If you need to realize gains/losses for a specific period, harvest to record the income.
  </Accordion>

  <Accordion title="To compound earnings">
    Harvest and re-add the tokens as liquidity to earn fees on your fees.
  </Accordion>
</AccordionGroup>

<Tip>
For most users, harvesting weekly or monthly is sufficient. Very active positions may warrant more frequent harvesting.
</Tip>

---

## What You'll Receive

When you harvest, you receive:

| Type | Description |
|------|-------------|
| **Trading fees** | Your share of swap fees from trades through your range |
| **Token rewards** | Additional incentive tokens (if the pool has active rewards) |

<Note>
Fees are paid in the pool's token pair. If you're in a SOL/USDC pool, you'll receive fees in both SOL and USDC.
</Note>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Manage Portfolio" icon="chart-pie" href="/liquidity/manage/portfolio">
    View all your positions and performance
  </Card>
  <Card title="Position Alerts" icon="bell" href="/liquidity/manage/alerts">
    Get notified when positions go out of range
  </Card>
  <Card title="Add Liquidity" icon="plus" href="/liquidity/manage/add">
    Increase your position with earned fees
  </Card>
  <Card title="Withdraw Liquidity" icon="arrow-up-from-bracket" href="/liquidity/manage/withdraw">
    Remove liquidity from positions
  </Card>
</CardGroup>
