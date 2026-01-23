---
title: FAQs
description: Frequently asked questions about Orca.
icon: circle-question
---

Find answers to common questions about trading, providing liquidity, and using Orca.

---

## About Orca

<AccordionGroup>
  <Accordion title="What is Orca?">
    Orca is a decentralized exchange (DEX) that strives to be the epicenter of spot trading on Solana. Built by DeFi OGs with a user-first approach, Orca combines concentrated liquidity (CLMM) with an intuitive UI and unparalleled user support.
  </Accordion>

  <Accordion title="What's the difference between a CLMM and traditional exchange?">
    Traditional order book exchanges (CLOBs) match buyers and sellers based on price. AMMs/CLMMs let you trade against a pool of tokens rather than directly with other users.

    Orca believes CLMMs offer a superior approach for blockchain applications due to their simplicity and composability. With the right tools, a CLMM can achieve everything a CLOB can—and more.
  </Accordion>

  <Accordion title="Why Solana?">
    Solana offers exceptional performance: 50,000 TPS, 400ms block times, and low transaction fees. Orca believes Solana is the best choice to support the next generation of DeFi apps.
  </Accordion>

  <Accordion title="Has Orca been audited?">
    Yes. Orca's Whirlpools concentrated liquidity product is [double audited](https://github.com/orca-so/whirlpools/tree/main/.audits), and amendments are also audited.
  </Accordion>

  <Accordion title="Does Orca have a governance token?">
    Yes. The ORCA governance token launched on August 9, 2021. See [Token Treasury](/governance/treasury) for details and [Governance](/governance/overview) for the governance process.
  </Accordion>
</AccordionGroup>

---

## Trading

<AccordionGroup>
  <Accordion title="How do I trade on Orca?">
    See our complete [How to Swap guide](/trade/how-to-swap).
  </Accordion>

  <Accordion title="Which wallets can I use?">
    See our [supported wallets](/get-started/wallets). Orca integrates wallets that support Solana program execution.

    <Warning>
    Orca does not endorse or guarantee the security of compatible wallets. Do your own research before using any wallet.
    </Warning>
  </Accordion>

  <Accordion title="Can I use Orca on mobile?">
    Yes! Use Orca with mobile-compatible wallets listed in our [wallets guide](/get-started/wallets).
  </Accordion>

  <Accordion title="What fees do I pay when trading?">
    | Fee Type | Amount |
    |----------|--------|
    | **Trading fee** | 0.01% - 1% (varies by pool) |
    | **Network fee** | ~0.0001-0.001 SOL |

    Orca does not charge additional fees. See [Trading Fees](/reference/fees) for details.
  </Accordion>

  <Accordion title="What is price impact?">
    Price impact is how much your trade moves the market price. Larger trades in smaller pools have higher price impact.

    If your trade has >1% price impact, you'll see a warning. You can still proceed after acknowledging it.
  </Accordion>

  <Accordion title="Why did my trade fail?">
    Common causes:
    - **Slippage too low** — Increase slippage tolerance
    - **Insufficient SOL** — Need SOL for network fees
    - **Price moved** — Market moved beyond your slippage tolerance

    The UI will offer a retry option with the same parameters.
  </Accordion>

  <Accordion title="What does 'spend at most' and 'receive at least' mean?">
    These are your worst-case outcomes based on your slippage tolerance. If actual slippage exceeds these limits, the trade fails instead of executing at a bad price.
  </Accordion>

  <Accordion title="What is a sub-route?">
    Orca's Smart Router can split trades across up to six routes for the best price. A sub-route is an indirect path like ORCA → SOL → USDC. View your trade composition in the details dropdown.
  </Accordion>

  <Accordion title="Can I trade programmatically?">
    Yes! Use the [TypeScript SDK](https://github.com/orca-so/whirlpools). See [Developer Docs](/developers/overview) and ask questions in Discord's #dev-questions channel.
  </Accordion>
</AccordionGroup>

---

## Liquidity Provision

<AccordionGroup>
  <Accordion title="Why provide liquidity on Orca?">
    Liquidity providers earn trading fees from every trade that routes through their position. Some pools also offer additional token rewards.
  </Accordion>

  <Accordion title="How do I earn fees?">
    When you provide liquidity in a pool, you earn a [maker fee](/reference/fees) from each trade executed against your liquidity. Yield is [harvestable](/liquidity/manage/harvest) anytime.
  </Accordion>

  <Accordion title="What is the difference between Full-Range and Custom-Range?">
    | Type | Description |
    |------|-------------|
    | **Full-Range** | Liquidity spread from 0 to infinity. Simple, always earning, but less capital efficient |
    | **Custom-Range** | Liquidity concentrated in a specific range. More efficient but requires monitoring |
  </Accordion>

  <Accordion title="What is divergence loss (impermanent loss)?">
    Divergence loss occurs when token prices deviate from their initial deposit values, causing your position value to decrease compared to simply holding the tokens.

    See [Impermanent Loss](/liquidity/concepts/impermanent-loss) for details.
  </Accordion>

  <Accordion title="Can I withdraw my liquidity at any time?">
    Yes, Orca allows you to withdraw liquidity at any time with no lock-up period.
  </Accordion>

  <Accordion title="What is a pool position NFT?">
    Your liquidity position is represented by an NFT that proves ownership. This NFT:
    - Is required to withdraw your liquidity
    - Can be transferred to move your position
    - **Must not be burned** or your liquidity is permanently lost
  </Accordion>

  <Accordion title="I burned my position NFT—can Orca help?">
    No. If a position NFT is burned, there is no way to recover the associated liquidity. The NFT is proof of ownership on the blockchain—without it, the liquidity cannot be accessed by anyone.
  </Accordion>

  <Accordion title="Why isn't my deposit ratio 50:50?">
    The deposit ratio depends on your price range relative to current price. The closer current price is to one of your range bounds, the less balanced the ratio. Full-range positions have 50:50 ratios.
  </Accordion>

  <Accordion title="What happens if price goes outside my range?">
    Your position becomes 100% one token and stops earning fees. If price returns to your range, you'll start earning again. See [Managing Your Portfolio](/liquidity/manage/portfolio).
  </Accordion>

  <Accordion title="Do I get ORCA tokens as rewards?">
    Some pools receive ORCA token rewards to encourage deeper liquidity. Eligible pools are marked in the explorer. Non-incentivized pools still generate trading fees.
  </Accordion>
</AccordionGroup>

---

## Pool Creation

<AccordionGroup>
  <Accordion title="Does Orca charge fees to create pools?">
    No. Only Solana network and Metaplex fees are payable.
  </Accordion>

  <Accordion title="What is an Adaptive Fee Pool vs Fixed Fee Pool?">
    | Type | Description |
    |------|-------------|
    | **Adaptive Fee** | Dynamically adjusts fees based on market volatility |
    | **Fixed Fee** | Charges the same fee for every trade |

    Learn more: [Adaptive Fees](/liquidity/concepts/adaptive-fees)
  </Accordion>

  <Accordion title="I created a pool but can't find it—where is it?">
    New pools can take up to 15 minutes to appear. Force-refresh your browser to potentially reduce this time.
  </Accordion>

  <Accordion title="How can I change the token price in my pool?">
    You can't directly change a pool price—only market trading activity changes it. Contact Orca via [Discord](https://discord.gg/orca-so) for help calculating trade sizes to move prices.
  </Accordion>

  <Accordion title="Can I delete a pool I created?">
    No. Pools cannot be deleted. Take care during the creation process.
  </Accordion>

  <Accordion title="How do I remove the warning triangle on my token?">
    Contact Orca via the Support function in the UI or [Discord](https://discord.gg/orca-so) to discuss removal.
  </Accordion>

  <Accordion title="What are Token Extensions?">
    Token Extensions are advanced functionalities for tokens to comply with legal requirements. Most tokens don't need them. See [Token Extensions](/create/pools/extensions).
  </Accordion>
</AccordionGroup>

---

## Technical

<AccordionGroup>
  <Accordion title="What does 'Not Enough SOL' mean?">
    SOL is required for network fees. Maintain at least 0.05 SOL. See [Pool Network Fees](/reference/fees).
  </Accordion>

  <Accordion title="Why was I charged higher network fees than usual?">
    If your price range includes limits where no positions exist, you may pay 0.07-0.14 SOL extra to initialize tick arrays. These are Solana network fees, not Orca fees.
  </Accordion>

  <Accordion title="Are tokens on Orca wrapped?">
    Some tokens are wrapped from other chains. Always do your own research before trading wrapped tokens.
  </Accordion>

  <Accordion title="How do I trade ERC-20 tokens on Orca?">
    You'll need to convert ERC-20s to SPL tokens using a bridge. Do your own research before bridging.
  </Accordion>
</AccordionGroup>

---

## Security & Risks

<AccordionGroup>
  <Accordion title="What are the risks of using Orca?">
    | Risk | Mitigation |
    |------|------------|
    | **Smart contract vulnerabilities** | Orca is [double audited](https://github.com/orca-so/whirlpools/tree/main/.audits) |
    | **Divergence loss** | Understand concentrated liquidity mechanics |
    | **Wallet vulnerabilities** | Use reputable wallets, DYOR |
  </Accordion>

  <Accordion title="Is Orca safe?">
    Orca's smart contracts are audited and have secured billions in trading volume. However, always practice good security hygiene—verify transactions and protect your wallet.
  </Accordion>
</AccordionGroup>

---

## More Help

<CardGroup cols={2}>
  <Card title="Discord Support" icon="discord" href="https://discord.gg/orca-so">
    Open a support ticket or ask in #support
  </Card>
  <Card title="Telegram" icon="telegram" href="https://t.me/orca_so">
    Get support on Telegram
  </Card>
</CardGroup>

<Note>
Can't find your answer? Ask in Discord's #support-ticket channel or use the Support button in the Orca UI.
</Note>
