---
title: Programs
type: overview
draft: true
public: false
created: 2026-04-21
updated: 2026-04-21
---

# Programs

**Status:** Work in progress. Several sections are stubbed and waiting on Chop's direct input (see inline `[TBD]` markers and `drafts/PYTH_GAPS.md` for the full punchlist).

---

The programs and systems I've designed, built, or inherited-and-rebuilt during my time at Pyth. Each one is a specific application of the [[philosophy]] — every program exists to feed at least one step of the Recognize → Reward → Attract → Identity → Contribute cycle.

Organized by era, roughly.

---

## Community Council (Founded)

I **built** the Community Council. This is the one I'm most proud of.

[TBD — Chop input needed. This is a major portfolio signal and deserves the deepest treatment on the page. Tell me:
- The year and context. What was the state of Pyth governance before the Council existed?
- The problem it was solving. Why did the protocol need a Council — what gap did you see?
- How you proposed it. Internal pitch? Forum post? Direct to leadership? Who pushed back?
- The rollout. Election process, first cohort, how the first term went.
- The outcome. What did the Council actually ship? What did it unlock (MissionMonitor testing, governance proposals, etc)?
- The transition. You served on it. How did term end, and how does election 2 work?
- The legacy frame. Why this structure specifically — why not advisory board, why not DAO-vote-only.

Target length: 4-6 paragraphs. This is the page's anchor section.]

---

## Early Community Infrastructure

Everything that existed before the big programs — the bones the later work was built on.

### Discord Setup & Structure

[TBD — Chop input needed. The Discord restructure. What was it like before, what you changed, what the logic was. Channel architecture, role system, moderation philosophy. How you mapped the flywheel onto Discord roles and permissions. Target: 2-3 paragraphs.]

### Impact Awards

[TBD — Chop input needed. The Impact Awards system — Impact Ops (memes, education, amplification), Events, Vibes. Origins of the program, how recipients are chosen, budget/rewards structure, what it unlocked in terms of contributor visibility. Target: 2-3 paragraphs.]

### Pythenians NFT

[TBD — Chop input needed. The Pythenians NFT acquisition and community. When/why/how. Current status (your notes mention handover overdue — multisig, Twitter creds, subscriptions). What role it plays in the identity layer. Target: 2 paragraphs.]

### PIRB (Pyth Intelligence Research Bureau)

[TBD — Chop input needed. The invite-only Telegram intelligence agency. Who's in it, what it's for, how it functions as an inner circle for high-signal contributors. Why invite-only and not open. Target: 2 paragraphs.]

---

## Operational Systems

The programs I ship as **architecture, not events** — systems that run forever once built.

### MissionMonitor

The operational heart of community content creation. Live in production.

A mission delivery system that turns campaign requests into structured briefs, routes them to Telegram and Discord simultaneously, tracks submissions, handles judging via emoji reactions, auto-closes on deadline, and exports results to Google Sheets for payout tracking.

The philosophy is simple: **we provide FACTS, creators provide VOICE.** Mission briefs are factual-only — no editorial framing, no pre-written tweets, no "say this." We give creators the data points, the sources, and directional angles. The creative expression is theirs. This is the only way community content stays authentic at scale.

First real deployment was with the Community Council as judges. Referrals system (10% split on attributed submissions, 90-day expiry, self-referral rejection) is coded and awaiting backtest before rollout.

### PythClippers

Clip submission and rewards engine for Discord and Telegram. Built in partnership with the MissionMonitor architecture — they're designed to merge eventually into a single unified content + incentives platform.

Currently staged at 6 of 8 deployment phases. Remaining: production API keys, Docker deploy to VPS, E2E verification, and the legal T&C wrapper that gates the rewards layer.

### Pythentity

The verified identity layer for all content and incentive programs. MVP is live.

The problem: incentive programs without identity become sybil farms. Every bot, every alt account, every extractive participant drains the budget and starves real contributors. Pythentity gates the next generation of Pyth community programs — your identity, once verified, travels with you across MissionMonitor, PythClippers, Impact Awards, and anything else we build.

Positioned strategically as **the gate for the next incentive program**, which means every future program that launches pulls more contributors into the verified identity graph. That's the flywheel — identity isn't a side feature, it's the substrate.

[TBD — Chop input needed: the specific design decisions behind Pythentity (why EVM wallet support, why this identity model vs. others), the partner / grant context (68K PYTH from an 80K grant — what that covered), the migration plan. Target: 1-2 additional paragraphs.]

### Content Incentive Stack

Not a single program — **layers of one machine**.

```
Video Transcripts (117+ files)
    > Notion Database (team discovery layer)
    > PythClippers (clip submission + rewards)
    > MissionMonitor (missions + judging + referrals)
    > Google Sheets (payout tracking)
    > Clipping Incentive Program (2M PYTH budget)
```

The insight: most protocols treat content as a marketing output. I treat it as a contribution input. The stack turns every hour of video Pyth leadership records into 100+ clips, 50+ missions, and a permanent, searchable, creator-facing content library that anyone in the community can mine.

Middle pieces are live. Input layer (Notion DB for team discovery) and legal wrapper (T&Cs for the 2M PYTH clipping budget) are the current blockers.

### Vibecodeathon

A 6-week community hackathon running on the Pyth dev forum. Low-barrier entry (no KYC, no application period, no IRL requirement, no skill gating). Gives builders free access to institutional-grade price feeds and lets them ship whatever they want with it.

55 submissions in round one, ~70% backloaded into the final week (a pattern worth planning for — see the case study in my upcoming blog series on [community hackathon design](../../drafts/01-hackathon-worked) once it publishes).

---

## Strategic Content Programs

### Asset Info Packs (AI Discoverability)

The content pipeline for Pyth's AI visibility push. Each pack (XAU gold, BTC, ETH, equities, FX, commodities) generates 15-20 derivative content pieces across 8 channels, structured to maximize LLM citation rates — answer capsules at the 40-60 word length LLMs prefer, statistics every 150 words, schema.org markup for machine readability.

The strategic bet: when a developer asks Claude or ChatGPT "how do I get price data for my app?", Pyth has to be in the top three suggestions. Right now it isn't. The content gap is closing that. See [[thesis#ai-discoverability]] for the full argument.

### Twitter Growth System (@CHOPPAtheSHARK)

The operational system behind my Twitter presence — 7 tracking files covering strategy, pillar-classified content bank, weekly queue, 8-week thread pipeline, daily routine, reply targets, and metrics. Built for compounding: 30-min daily execution, no bursts, no campaigns.

The theory is in [[philosophy#systems-over-campaigns]]. The execution is the proof of concept.

---

## Partnerships (Downstream)

The partnerships side of the work isn't a separate function — it's what happens when the community becomes valuable enough that counterparties come to *us*. Most of these relationships exist because the Pyth community reached a scale and coherence where integrating made obvious sense, not because a BD pitch closed them.

Notable relationships visible from the outside:

- **Blue Ocean** — exclusive partnership in the gaming / prediction markets vertical
- **Polymarket** — active integration + creator partnership angles
- **Fogo Foundation** — SVM L1 gaming grants pipeline
- **Superteam Earn** — developer grants distribution channel
- **University outreach** — Australian universities network, guest lectures + early-career funnel

[TBD — Chop input needed: specific partnership wins worth naming publicly. Integrations you shipped that are visible. Creator streams that went live. Co-marketing deals that closed. Anything that proves the community-as-gravity-well thesis worked. Target: 2-3 paragraphs of named outcomes, framed as "this happened because the community was already strong."]

---

## Speaking + Public Appearances

[TBD — Chop input needed: streams you've been on, podcasts, conference panels, AMAs. Dates, venues, what they were about, links if available. This is portfolio material for the Chop site — treat it accordingly. Target: a table of appearances chronologically.]

---

## What I've Learned

[TBD — Chop input needed. Optional closing section: 3-5 lessons from running all this at scale. The things that surprised you. The things you got wrong the first time. What you'd do differently if you started over tomorrow. Target: 4-6 paragraphs of distilled operator wisdom — this is the section that makes the page memorable.]

---

## Related

- [[philosophy]] — the theoretical basis for every program on this page
- [[thesis]] — why this portfolio of work, in this order, at this moment
