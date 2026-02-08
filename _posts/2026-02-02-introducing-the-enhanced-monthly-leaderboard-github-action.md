---
layout: post
title: "Introducing the Enhanced Monthly Leaderboard GitHub Action"
date: 2026-02-02 01:51
author: admin
image: https://github.com/user-attachments/assets/2301ef11-24cd-4024-a9c7-29ee58d4c4a1
---

# 🚀 Introducing the Enhanced Monthly Leaderboard GitHub Action

We're excited to announce a major update to our automated leaderboard system! The new **Monthly Leaderboard Bot** brings transparency, fairness, and motivation to our contributor community.

## What's New?

### 📊 Comprehensive Point System

Our new leaderboard tracks multiple types of contributions with a fair point system:

- **Open Pull Requests**: +1 point each (encourages active contributions)
- **Merged Pull Requests**: +10 points each (rewards successful contributions)
- **Closed (not merged) PRs**: -2 points (encourages quality over quantity)
- **Code Reviews**: +5 points each (first two reviews per PR count)
- **Issue Comments**: +2 points each (values community engagement)
- **CodeRabbit Discussions**: Configurable points with daily cap to prevent abuse

### 🎯 Monthly Rankings

The leaderboard resets monthly (based on UTC timezone), giving everyone a fresh start and highlighting current active contributors. Rankings consider:

1. Total points (primary sorting)
2. Merged PRs (tiebreaker)
3. Review count (secondary tiebreaker)
4. Alphabetical order (final tiebreaker)

### 🛡️ Anti-Abuse Features

To maintain quality and prevent spam:

- **PR Limit**: Automatically closes PRs if a contributor has 50+ open PRs
- **Bot Detection**: Automated accounts (like dependabot, copilot) are excluded
- **Daily Caps**: CodeRabbit discussion points have configurable daily limits per user

### 🏅 Automatic Leaderboard Comments

Every time a new pull request is opened, the bot automatically:

- Posts a leaderboard comment showing your current ranking
- Displays your position with nearby competitors
- Shows medals (🥇🥈🥉) for top 3 contributors
- Highlights your entry with ✨

### 🔒 Security First

The action uses `pull_request_target` with careful security measures:

- Only uses GitHub API (never checks out or executes PR code)
- Safe execution even for PRs from forked repositories
- Limited permissions (read contents, write PR comments)

## Example Leaderboard

Here's what a leaderboard comment looks like:

```
| Rank | User | Open PRs | PRs (merged) | PRs (closed) | Reviews | Comments | Total |
|------|------|----------|--------------|--------------|---------|----------|-------|
| 🥇 #1 | @contributor1 | 5 | 12 | 0 | 8 | 15 | **175** |
| 🥈 #2 | @contributor2 | 3 | 10 | 1 | 6 | 12 | **151** |
| #3 | **`@you`** ✨ | 2 | 8 | 0 | 5 | 10 | **112** |
```

## Configuration Options

Repository maintainers can configure:

- **CR_DISCUSSION_MODE**: `visible` (show column), `hidden` (score but don't show), or `separate` (track but don't score)
- **CR_DISCUSSION_POINTS**: Points awarded per CodeRabbit discussion (default: 0)
- **CR_DISCUSSION_DAILY_CAP**: Maximum counted discussions per user per day (default: 7)

## Impact on Contributors

This system encourages:

- **Quality contributions** through the high value of merged PRs
- **Community engagement** through review and comment points
- **Active participation** through open PR bonuses
- **Constructive feedback** through review rewards

## Technical Details

The leaderboard uses:

- **GitHub GraphQL API** for efficient data fetching
- **Smart pagination** to handle large repositories
- **Monthly time windows** (UTC-based)
- **Upsert logic** to update existing comments instead of spamming

## Getting Started

There's nothing you need to do! The leaderboard automatically runs when:

- You open a new pull request
- The bot posts/updates your ranking in the PR comments

Start contributing, reviewing, and engaging with the community to climb the leaderboard!

## Recognition & Credits

This enhancement was contributed by the community through **PR #5465**, demonstrating the collaborative spirit that makes open source projects thrive.

---

**Ready to compete?** Open your next PR and see where you rank! 🏆

*Questions or feedback? Join the discussion in the comments below or reach out to the maintainers.*
