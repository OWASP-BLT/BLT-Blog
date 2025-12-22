---
layout: post
title: "How to Deploy a Fungible Token on Bitcoin Ordinals"
date: 2025-08-26 05:23
categories: announcements
author: krrish__sehgal
image: /assets/images/bitcoin_ordials.png
---


My Journey Deploying the Bacon Token on Bitcoin Ordinals and Solana
When I first started exploring Bitcoin Ordinals and Solana, my goal was simple: understand how tokens can be created and deployed on two very different blockchain ecosystems. What began as curiosity turned into a full learning journey when I deployed BLT's token — **Bacon** — on both Bitcoin Ordinals and Solana.
<br>
Why Bitcoin Ordinals and Solana?
<br>
**[Bitcoin Ordinals](https://docs.ordinals.com/)** opened up a new frontier, letting developers inscribe unique data (like NFTs or tokens) directly onto Bitcoin’s smallest units, satoshis. The challenge is that Bitcoin wasn’t originally designed for token deployments, so working around those limitations was both exciting and educational.
<br>
**[Solana](https://solana.com/developers)** on the other hand, is built with scalability and speed in mind. Deploying a token here is straightforward compared to Bitcoin, but it introduces its own set of concepts around [smart contracts](https://solana.com/developers/guides/smart-contracts), [accounts](https://solana.com/docs/core/accounts), and transaction fees.
<br>
By working with both ecosystems, I could compare the differences in token standards, deployment complexity, and community tooling.
<br>
My Process
<br>
**On Bitcoin Ordinals:** I had to start from scratch — syncing a [Bitcoin Core node](https://bitcoin.org/en/full-node), setting up the [Ordinals](https://docs.ordinals.com/) and [Runes](https://docs.ordinals.com/runes.html) infrastructure, and inscribing data to represent the token. This was more about patience and infrastructure readiness than writing code.
<br>
**On Solana:** I used the [Solana CLI](https://docs.anza.xyz/cli/) and [Token Program](https://www.solana-program.com/docs/token) to deploy Bacon. This required understanding wallets, the SDK, and the basics of Solana’s programmatic token creation system.
<br>
Lessons Learned
<br>
Running a [Bitcoin node](https://bitcoin.org/en/full-node) is resource-heavy but essential for trustless token operations.
<br>
[Solana’s ecosystem](https://solana.com/developers) is developer-friendly, but comes with trade-offs in decentralization and reliance on [RPC providers](https://solana.com/docs/core/rpc).
<br>
Security is key in both cases — from handling [private keys](https://en.bitcoin.it/wiki/Private_key) safely to ensuring proper validation of transactions.
<br>
What This Blog Covers
<br>
In my full step-by-step guide on Medium, I break down exactly how I:
<br>
Set up the Bitcoin and Solana environments
<br>
Synced Bitcoin Core for Ordinals
<br>
Deployed the Bacon token on Solana using the CLI
<br>
Tested, verified, and interacted with the token
<br>
You can read the complete guide here and also see my work on Bitcoin Ordinals, including the actual Bacon inscription:
<br>
🔗 [How to Deploy Runes and Ordinals on Bitcoin](https://medium.com/@krrishsehgal03/how-to-deploy-runes-and-ordinals-on-bitcoin-84a387abe678)
<br>
🔗 [Bacon Inscription](https://ordinals.com/inscription/9ebf269d5b73ade615e439cbb0ed6427697672e7c60b761dc2e566f4a5a80050i0)
<br>
Further Developments for Bacon in BLT
<br>
Beyond deploying Bacon on Bitcoin and Solana, I am also actively contributing to BLT by building features around Bacon, including:
<br>
**Streamlining of the UI:** [GitHub PR #4368](https://github.com/OWASP-BLT/BLT/pull/4368)
<br>
**AI-Based Reward System:** [GitHub PR #4398](https://github.com/OWASP-BLT/BLT/pull/4398)
<br>
**Staking Feature:** [GitHub PR #4461](https://github.com/OWASP-BLT/BLT/pull/4461)
<br>
I hope my journey inspires other developers to experiment with cross-chain token creation. If you’ve been curious about Ordinals, Runes, or Solana, this guide will give you the steps to deploy your own token from scratch.