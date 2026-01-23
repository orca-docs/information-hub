---
title: Impermanent Loss
description: Understand impermanent loss (divergence loss) and how it affects liquidity providers.
icon: chart-line-down
---

Impermanent loss (IL) is one of the most misunderstood concepts in DeFi. Despite the name, it's not always impermanent—and not always a true loss relative to your original capital.

<Info>
Orca prefers the term **Divergence Loss** (DL) because it more accurately describes what happens: asset prices move apart (diverge) from their original ratio.
</Info>

---

## What This Guide Covers

- Why "impermanent loss" can be misleading
- How IL works in Concentrated Liquidity (CLMMs)
- When IL becomes permanent—and when it doesn't
- How position management affects outcomes

---

## What Is Impermanent Loss?

<CardGroup cols={2}>
  <Card title="Simple Definition" icon="book">
    The difference in value between providing liquidity vs. simply holding the tokens in your wallet.
  </Card>
  <Card title="Key Insight" icon="lightbulb">
    IL is a **relative** comparison, not necessarily an absolute loss from your original deposit.
  </Card>
</CardGroup>

In an AMM, IL occurs when the relative prices of your deposited assets change. If you withdraw at a different price ratio than when you deposited, your position value may be lower than if you had just held the tokens.

---

## Why the Name Is Confusing

<AccordionGroup>
  <Accordion title="It's not always 'impermanent'" icon="clock">
    The term suggests the loss will resolve itself. In reality, if you withdraw at the wrong time, the loss becomes **permanent**.
  </Accordion>

  <Accordion title="It's not always a 'loss'" icon="chart-line">
    You can still be **profitable overall** compared to your initial deposit, even with IL. The term "loss" compares to holding—not to your starting capital.
  </Accordion>
</AccordionGroup>

<Tip>
Think of IL as an **opportunity cost** compared to holding, not necessarily money lost from your pocket.
</Tip>

---

## Example Scenarios

For these examples, assume:
- 1 USDC = $1
- Initial SOL price: $200
- Selected range: $160–$250
- Liquidity provided: 2.5 SOL ($500) + 500 USDC = **$1,000 total**

### Scenario 1: When IL Is Temporary

<Steps>
  <Step title="Price drops to $170">
    If you withdraw now:
    - Receive ~4.50 SOL ($765) + 130 USDC
    - **Total: ~$896**
  </Step>
  <Step title="Compare to holding">
    If you had simply held:
    - 2.5 SOL ($425) + 500 USDC = **$925**

    IL at this point: **$29**
  </Step>
  <Step title="Price returns to $200">
    If you **wait** and price returns to $200:
    - Position value: **$1,000**
    - No loss realized

    This is **path independence**: withdraw at the same price you deposited = same value.
  </Step>
</Steps>

<Note>
**Key Takeaway:** IL only becomes permanent if you withdraw at a different price than you deposited.
</Note>

---

### Scenario 2: When IL Isn't Really a Loss

<Steps>
  <Step title="Price rises to $250">
    If you withdraw now:
    - Receive ~$1,059 USDC
    - **Total: ~$1,059**
  </Step>
  <Step title="Compare to holding">
    If you had simply held:
    - 2.5 SOL ($625) + 500 USDC = **$1,125**

    IL compared to holding: **$66**
  </Step>
  <Step title="But you're still ahead">
    Your original deposit was **$1,000**.
    You now have **$1,059**.

    You're **up $59** from your starting capital!
  </Step>
</Steps>

<Info>
This example doesn't even include **trading fees earned** while your liquidity was active. Fees often more than compensate for IL.
</Info>

---

## IL in Concentrated Liquidity (CLMMs)

Concentrated liquidity **amplifies** both potential gains and IL:

| Factor | Effect on IL |
|--------|--------------|
| **Narrower range** | Higher IL risk (more concentrated exposure) |
| **Wider range** | Lower IL risk (more diversified) |
| **Higher fees** | Can offset more IL |
| **More trades** | More fees to compensate |

<Warning>
In CLMMs, price movements have a larger effect because your liquidity is concentrated in a smaller range. Understand this before choosing tight ranges.
</Warning>

---

## Key Takeaways

<CardGroup cols={2}>
  <Card title="IL Is Only Realized When You Withdraw" icon="hand">
    If prices recover before withdrawal, the "loss" can disappear. But price may never return to your exact deposit level.
  </Card>
  <Card title="IL Is Relative, Not Absolute" icon="scale-balanced">
    You compare to holding, not to your initial deposit. You can have IL **and** still profit.
  </Card>
  <Card title="Fees Are Critical" icon="coins">
    You outperform holding when earned fees exceed realized IL. High-volume pools help offset IL.
  </Card>
  <Card title="Position Management Matters" icon="sliders">
    Expecting price recovery? Hold your position. Expecting continued divergence? Consider repositioning.
  </Card>
</CardGroup>

---

## Why Orca Prefers "Divergence Loss"

<AccordionGroup>
  <Accordion title="More accurate terminology">
    - **Divergence** directly describes what happens: prices move apart from their original ratio
    - **Impermanent** implies it will reverse—which isn't guaranteed
    - **Loss** should be understood relative to an alternative, not as absolute
  </Accordion>

  <Accordion title="Helps LPs make better decisions">
    Understanding that IL depends on **your behavior** (when you withdraw) rather than just market behavior helps you make more informed decisions.
  </Accordion>
</AccordionGroup>

---

## Managing IL Risk

<AccordionGroup>
  <Accordion title="Choose appropriate ranges">
    - **Wider ranges** = less IL risk, lower capital efficiency
    - **Tighter ranges** = higher IL risk, higher potential fees
    - Match your range to your risk tolerance and monitoring capacity
  </Accordion>

  <Accordion title="Select high-volume pools">
    More trading volume = more fees to offset potential IL. Check the 24h volume and fee APR before depositing.
  </Accordion>

  <Accordion title="Monitor and rebalance strategically">
    - Don't panic-withdraw during temporary price swings
    - Consider waiting for price recovery if you expect it
    - Rebalance only when the cost is justified
  </Accordion>

  <Accordion title="Understand your exit strategy">
    Know in advance:
    - At what point will you withdraw?
    - What price movement would trigger a rebalance?
    - Are you willing to hold through volatility?
  </Accordion>
</AccordionGroup>

---

## Conclusion

Impermanent loss is an important concept, but it's only part of the bigger picture. Successful liquidity provision requires balancing:

- **Fee generation** — Earning from trading activity
- **Price divergence risk** — Understanding IL dynamics
- **Opportunity costs** — Comparing to holding, staking, or lending

<Tip>
With careful strategy and active management, LPs can often turn impermanent loss from a threat into an opportunity.
</Tip>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Position Simulator" icon="chart-line" href="/liquidity/advanced/simulator">
    Visualize IL for different scenarios
  </Card>
  <Card title="LP Strategies" icon="lightbulb" href="/liquidity/advanced/strategies">
    Learn techniques to manage IL
  </Card>
  <Card title="Create a Position" icon="plus" href="/liquidity/getting-started/beginner-guide">
    Start providing liquidity
  </Card>
  <Card title="Understanding Ticks & Fees" icon="gauge" href="/liquidity/concepts/ticks-and-fees">
    Learn how fees work in CLMMs
  </Card>
</CardGroup>
