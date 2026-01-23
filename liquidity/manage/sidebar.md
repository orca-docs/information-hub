---
title: Position Details Sidebar
description: Use the position details sidebar to manage your LP positions.
icon: sidebar
---

The Position Details sidebar is your central hub for monitoring and managing liquidity positions. Access detailed information, harvest fees, deposit more liquidity, or withdraw—all in one place.

---

## Accessing the Sidebar

You can open the sidebar from two locations:

<CardGroup cols={2}>
  <Card title="Liquidity Terminal" icon="terminal">
    From the **My Positions** pane when viewing any pool
  </Card>
  <Card title="Portfolio Page" icon="chart-pie">
    From [orca.so/portfolio](https://www.orca.so/portfolio)
  </Card>
</CardGroup>

### How to Open

<Tabs>
  <Tab title="Click the Position">
    Click anywhere on your position row to open the sidebar.

    <Frame caption="Click anywhere on the position to open details">
      <img src="/images/image_69.jpg" alt="Click position to open sidebar" />
    </Frame>
  </Tab>

  <Tab title="Use the Menu">
    Click the **...** (ellipsis) button on the right side of your position.

    <Frame caption="Click the ellipsis for quick actions">
      <img src="/images/image_70.jpg" alt="Ellipsis menu" />
    </Frame>

    Then select from the dropdown:
    - **Position Details** — Full sidebar view
    - **+ Deposit Liquidity** — Jump straight to deposit
    - **- Withdraw Liquidity** — Jump straight to withdraw

    <Frame caption="Select your action from the menu">
      <img src="/images/image_71.jpg" alt="Position menu options" />
    </Frame>
  </Tab>
</Tabs>

---

## Sidebar Tabs

The sidebar has three main tabs:

<AccordionGroup>
  <Accordion title="Details" icon="circle-info">
    View comprehensive information about your position:
    - **Token balances** — Current amounts of each token
    - **Price range** — Your min/max bounds
    - **Current price** — Where the market is now
    - **In-range status** — Whether you're earning fees
    - **Performance metrics** — Fees earned, value changes
    - **Harvest button** — Collect accumulated fees

    <Card title="How to Harvest Yield" icon="seedling" href="/liquidity/manage/harvest">
      Learn about harvesting your earned fees
    </Card>
  </Accordion>

  <Accordion title="Deposit" icon="plus">
    Add more liquidity to your existing position:
    - Enter amounts for either token
    - Auto-balancing calculates the other
    - Use **Max** for quick deposits
    - Enable **Autoswap** to balance tokens automatically

    <Card title="How to Add Liquidity" icon="plus" href="/liquidity/manage/add">
      Step-by-step deposit guide
    </Card>
  </Accordion>

  <Accordion title="Withdraw" icon="arrow-up-from-bracket">
    Remove liquidity from your position:
    - Enter amounts or use the slider
    - Partial or full withdrawal
    - Option to keep position NFT when closing
    - Fees harvested automatically

    <Card title="How to Withdraw Liquidity" icon="arrow-up-from-bracket" href="/liquidity/manage/withdraw">
      Step-by-step withdrawal guide
    </Card>
  </Accordion>
</AccordionGroup>

---

## Quick Actions from the Menu

The ellipsis (**...**) menu provides quick access to common actions:

| Action | What It Does |
|--------|--------------|
| **Position Details** | Opens full sidebar |
| **Harvest Yield** | Collects fees without opening sidebar |
| **+ Deposit Liquidity** | Opens sidebar to Deposit tab |
| **- Withdraw Liquidity** | Opens sidebar to Withdraw tab |
| **× Close Position** | Withdraws all liquidity and closes |

---

## Tips for Using the Sidebar

<AccordionGroup>
  <Accordion title="Check status before harvesting">
    If your position is out of range, consider whether to wait for price to return or close and reposition.
  </Accordion>

  <Accordion title="Use Autoswap for deposits">
    When depositing, if you don't have the right token ratio, Autoswap can balance your tokens automatically.
  </Accordion>

  <Accordion title="Keep the NFT when testing">
    If you're experimenting with positions, keep the NFT when closing so you can redeposit to the same range later.
  </Accordion>
</AccordionGroup>

---

## Related Guides

<CardGroup cols={2}>
  <Card title="Portfolio Management" icon="chart-pie" href="/liquidity/manage/portfolio">
    Overview of managing all your positions
  </Card>
  <Card title="Position Alerts" icon="bell" href="/liquidity/manage/alerts">
    Set up notifications for your positions
  </Card>
  <Card title="Harvest Yield" icon="seedling" href="/liquidity/manage/harvest">
    Collect your earned fees
  </Card>
  <Card title="Close Position" icon="xmark" href="/liquidity/manage/close">
    Fully exit a position
  </Card>
</CardGroup>
