---
layout: post
title: "How to Deploy a Fungible Token on Bitcoin Ordinals"
date: 2025-08-26 00:05:23 +0000
categories: announcements
author: krrish__sehgal
image: /assets/images/bitcoin_ordials.png
---


My Journey Deploying the Bacon Token on Bitcoin Ordinals and Solana
When I first started exploring Bitcoin Ordinals and Solana, my goal was simple: understand how tokens can be created and deployed on two very different blockchain ecosystems. What began as curiosity turned into a full learning journey when I deployed BLT's token — Bacon — on both Bitcoin Ordinals and Solana.

Why Bitcoin Ordinals and Solana?
Bitcoin Ordinals opened up a new frontier, letting developers inscribe unique data (like NFTs or tokens) directly onto Bitcoin’s smallest units, satoshis. The challenge is that Bitcoin wasn’t originally designed for token deployments, so working around those limitations was both exciting and educational.
Solana on the other hand, is built with scalability and speed in mind. Deploying a token here is straightforward compared to Bitcoin, but it introduces its own set of concepts around smart contracts, accounts, and transaction fees.
By working with both ecosystems, I could compare the differences in token standards, deployment complexity, and community tooling.

My Process
On Bitcoin Ordinals: I had to start from scratch — syncing a Bitcoin Core node, setting up the Ordinals and Runes infrastructure, and inscribing data to represent the token. This was more about patience and infrastructure readiness than writing code.
On Solana: I used the Solana CLI and Token Program to deploy Bacon. This required understanding wallets, the SDK, and the basics of Solana’s programmatic token creation system.
Lessons Learned
Running a Bitcoin node is resource-heavy but essential for trustless token operations.
Solana’s ecosystem is developer-friendly, but comes with trade-offs in decentralization and reliance on RPC providers.
Security is key in both cases — from handling private keys safely to ensuring proper validation of transactions.
What This Blog Covers
In my full step-by-step guide on Medium, I break down exactly how I:

Set up the Bitcoin and Solana environments
Synced Bitcoin Core for Ordinals
Deployed the Bacon token on Solana using the CLI
Tested, verified, and interacted with the token
You can read the complete guide here and also see my work on Bitcoin Ordinals, including the actual Bacon inscription:
🔗 How to Deploy Runes and Ordinals on Bitcoin
🔗 Bacon Inscription

Further Developments for Bacon in BLT
Beyond deploying Bacon on Bitcoin and Solana, I am also actively contributing to BLT by building features around Bacon, including:

Streamlining of the UI: GitHub PR #4368
AI-Based Reward System: GitHub PR #4398
Staking Feature: GitHub PR #4461
I hope my journey inspires other developers to experiment with cross-chain token creation. If you’ve been curious about Ordinals, Runes, or Solana, this guide will give you the steps to deploy your own token from scratch.