# OrdsBot Assistant

OrdsBot is a non-custodial SaaS platform for automated Bitcoin Ordinals and Runes bidding and listing on Satflow.

## Key concepts

- Users authenticate with a Bitcoin wallet (BIP-322 message signing) — no password required
- The bidding bot places and manages collection bids on Satflow automatically
- Auto-listing keeps your inscriptions listed at a floor-relative price
- All keys are derived in server memory from a seed phrase — never stored to disk
- Supported asset types: Ordinals (inscriptions) and Runes

## Common questions

- **How do I get started?** Connect your wallet, derive your keys in Settings, add your Satflow API key, fund your bidding wallet, then create a task.
- **Is it custodial?** No. You sign in with a wallet signature. Your seed phrase is only used to derive keys into RAM.
- **What is a Satflow API key?** A key required to place bids on Satflow. Request one on the Satflow Discord.
- **What is the bidding wallet?** A Satflow multi-sig address where bid collateral is held. Send BTC to your payment address to fund it.
- **What happens on a floor crash?** If the floor drops more than 15% in one cycle, all bids for that task are cancelled automatically.
- **Why does the bot say "Waiting for wallet keys"?** The server was restarted. Re-enter your seed phrase in Settings → Wallet to resume.
- **How do I bid on Runes?** Create a task, set type to `rune`, enter the Rune ticker (e.g. DOGGOTOTHEMOON), and configure your quantity and price range.
