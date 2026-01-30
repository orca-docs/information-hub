---
title: Wallets
description: Find compatible wallets to connect to Orca.
icon: wallet
---

Connect to Orca using any wallet that meets the Solana Wallet standards.

---

## Supported Wallets

Orca automatically supports any compatible Solana wallet, including:

| Wallet | Desktop | Mobile | Multichain |
|--------|:-------:|:------:|:----------:|
| [Phantom](http://phantom.app/) | ✅ | ✅ | ✅ |
| [Backpack](https://www.backpack.app/) | ✅ | ✅ | ✅ |
| [Solflare](https://solflare.com/) | ✅ | ✅ | |
| [OKX Wallet](https://www.okx.com/web3) | ✅ | ✅ | ✅ |
| [Brave](https://brave.com/wallet) | ✅ | ✅ | ✅ |
| [Exodus](https://www.exodus.com/web3-wallet/) | ✅ | ✅ | ✅ |
| [Trust Wallet](https://trustwallet.com/) | ✅ | ✅ | ✅ |
| [Coin98](https://coin98.com/) | ✅ | ✅ | ✅ |
| [Glow](https://glow.app/) | ✅ | ✅ | |
| [SafePal](https://safepal.io/) | ✅ | ✅ | ✅ |
| [Token Pocket](https://tokenpocket.pro/) | ✅ | ✅ | ✅ |
| [Math Wallet](https://mathwallet.org/) | ✅ | ✅ | ✅ |
| [Bitkeep](https://bitkeep.com/) | ✅ | ✅ | ✅ |
| [Torus](https://solana.tor.us/login) | ✅ | ✅ | ✅ |
| [Ultimate](https://ultimate.app/) | ✅ | ✅ | |

<Info>
You can also connect compatible wallets using **WalletConnect**. Orca integrates new wallets as they become available.
</Info>

---

## Popular Wallets

<CardGroup cols={3}>
  <Card title="Phantom" icon="ghost" href="https://phantom.app/">
    Widely used Solana wallet with mobile support and hardware wallet compatibility.
  </Card>
  <Card title="Backpack" icon="backpack" href="https://www.backpack.app/">
    Feature-rich wallet with xNFT support and clean interface.
  </Card>
  <Card title="Solflare" icon="sun" href="https://solflare.com/">
    Solana-native wallet with staking features and Ledger support.
  </Card>
</CardGroup>

---

## Setting Up Your Wallet

<Steps>
  <Step title="Download your wallet">
    Visit the official wallet website and download the browser extension or mobile app.

    <Warning>
    Always download from official sources. Verify the URL carefully to avoid phishing sites.
    </Warning>
  </Step>

  <Step title="Create or import a wallet">
    - **New users**: Create a new wallet and securely store your seed phrase
    - **Existing users**: Import using your seed phrase or private key
  </Step>

  <Step title="Fund your wallet">
    Add SOL to your wallet for transaction fees:
    - Transfer from an exchange (use Solana network)
    - Buy directly in-wallet (some wallets support this)
    - Bridge from another chain
  </Step>

  <Step title="Connect to Orca">
    1. Visit [orca.so](https://www.orca.so)
    2. Click **Connect Wallet**
    3. Select your wallet
    4. Approve the connection
  </Step>
</Steps>

---

## Wallet Security Tips

<AccordionGroup>
  <Accordion title="Protect your seed phrase">
    - **Never share** your seed phrase with anyone
    - **Write it down** on paper and store securely
    - **Never enter** your seed phrase on any website
    - Consider using a hardware wallet for large amounts
  </Accordion>

  <Accordion title="Verify connections">
    - Always check the URL before connecting
    - Bookmark orca.so to avoid phishing sites
    - Review transaction details before approving
  </Accordion>

  <Accordion title="Use hardware wallets">
    For significant holdings, use a hardware wallet like Ledger. Both Phantom and Solflare support hardware wallet connections.
  </Accordion>
</AccordionGroup>

<Warning>
Orca does not endorse or guarantee the security of any wallet. Always do your own research before using any wallet.
</Warning>

---

## Troubleshooting

<AccordionGroup>
  <Accordion title="Wallet won't connect">
    - Refresh the page and try again
    - Ensure wallet extension is enabled
    - Try disconnecting and reconnecting
    - Clear browser cache
  </Accordion>

  <Accordion title="Transaction keeps failing">
    - Ensure you have enough SOL for fees (0.01+ SOL recommended)
    - Try increasing slippage tolerance
    - Network may be congested—wait and retry
  </Accordion>

  <Accordion title="Tokens not showing">
    - Some wallets require manually adding tokens
    - Check that you're on the Solana network
    - Refresh your wallet
  </Accordion>
</AccordionGroup>

---

## Next Steps

<CardGroup cols={2}>
  <Card title="Start Trading" icon="arrow-right-arrow-left" href="/trade/how-to-swap">
    Make your first swap on Orca
  </Card>
  <Card title="Provide Liquidity" icon="droplet" href="/liquidity/getting-started/beginner-guide">
    Earn fees by providing liquidity
  </Card>
</CardGroup>
