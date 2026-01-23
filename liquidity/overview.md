---
title: Providing Liquidity on Solana
description: Learn how to provide liquidity on Orca and earn trading fees.
icon: droplet
---

Earn yield by providing liquidity to Orca's concentrated liquidity pools (CLMMs). Concentrate your capital within specific price ranges for enhanced efficiency and returns.

<Info>
Orca's concentrated liquidity pools replace traditional order books, allowing anyone to create pools and earn trading fees. Understand the mechanics and risks before providing liquidity.
</Info>

---

## What is Concentrated Liquidity?

A CLMM (Concentrated Liquidity Market Maker) lets you allocate capital to **specific price ranges** instead of spreading it across all prices. This targeted approach maximizes capital efficiency and potential yields.

<CardGroup cols={2}>
  <Card title="Traditional AMM (CPMM)" icon="chart-simple">
    Liquidity spread across **all prices** from 0 to infinity. Less efficient, but simpler to manage.
  </Card>
  <Card title="Concentrated Liquidity (CLMM)" icon="bullseye">
    Liquidity focused on **chosen price ranges**. More efficient, higher potential yields, requires monitoring.
  </Card>
</CardGroup>

---

## Why Provide Liquidity on Orca?

<AccordionGroup>
  <Accordion title="Enhanced Capital Efficiency" icon="gauge-high">
    Focus your capital on profitable price ranges instead of spreading it across the entire price curve. Get more yield per dollar deposited.
  </Accordion>

  <Accordion title="Increased Earning Potential" icon="coins">
    By targeting high-volume trading ranges, you can earn significantly more from transaction fees than traditional full-range pools.
  </Accordion>

  <Accordion title="Flexible Management" icon="sliders">
    Adjust your price ranges in response to market conditions. Optimize returns and manage risk more effectively than with fixed positions.
  </Accordion>

  <Accordion title="Advanced Strategies" icon="chess">
    CLMMs support advanced techniques like limit orders and take-profit orders, providing greater versatility for sophisticated LPs.
  </Accordion>
</AccordionGroup>

---

## CLMM vs Traditional AMM

| Feature | Traditional CPMM | Orca CLMM |
|---------|-----------------|-----------|
| **Liquidity distribution** | Spread across all prices | Concentrated in chosen range |
| **Capital efficiency** | Lower | Higher |
| **Potential fees earned** | Less per $ deposited | More per $ deposited |
| **Management needed** | Minimal | More active monitoring |
| **Impermanent loss risk** | Lower | Can be higher if poorly managed |

---

## Position Types

<CardGroup cols={2}>
  <Card title="Full-Range Position" icon="arrows-left-right" href="/liquidity/getting-started/full-range">
    **Best for beginners**

    Spread liquidity from 0 to infinity. Lower maintenance, always in range, but less capital efficient.
  </Card>
  <Card title="Custom-Range Position" icon="crosshairs" href="/liquidity/getting-started/custom-range">
    **For experienced LPs**

    Concentrate liquidity in a specific range. Higher potential returns, requires active management.
  </Card>
</CardGroup>

---

## Getting Started

<Steps>
  <Step title="Understand the risks">
    Learn about [impermanent loss](/liquidity/concepts/impermanent-loss) and how concentrated liquidity affects your returns.
  </Step>
  <Step title="Choose your strategy">
    Decide between full-range (passive) or custom-range (active) positions based on your goals.
  </Step>
  <Step title="Create your position">
    Follow our guides to deposit liquidity and start earning fees.
  </Step>
  <Step title="Monitor and manage">
    Track your positions and adjust as needed using the [Portfolio](/liquidity/manage/portfolio) page.
  </Step>
</Steps>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Beginner's Guide" icon="graduation-cap" href="/liquidity/getting-started/beginner-guide">
    Complete introduction to liquidity provision on Orca
  </Card>
  <Card title="Full-Range Position" icon="arrows-left-right" href="/liquidity/getting-started/full-range">
    Create your first simple position
  </Card>
  <Card title="Custom-Range Position" icon="crosshairs" href="/liquidity/getting-started/custom-range">
    Advanced concentrated liquidity
  </Card>
  <Card title="Impermanent Loss" icon="chart-line-down" href="/liquidity/concepts/impermanent-loss">
    Understand the key risk of LP
  </Card>
</CardGroup>
