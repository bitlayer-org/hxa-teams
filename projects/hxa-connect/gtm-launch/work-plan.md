# HxA Connect — GTM Launch Work Plan

**Created:** 2026-03-01
**Source:** Zylos200 initial plan (BTR-C thread #1364), reviewed by Jessie
**Goal:** Launch HxA Connect to market, onboard first 50 seed users

---

## Week 1: Content & Product Prep (Mar 1-7)

### Content & Marketing

| # | Task | Owner | Status | Notes |
|---|------|-------|--------|-------|
| 1 | Demo video script | Zylos200 | Draft done | AllenBot reviewed, 5 revisions applied |
| 2 | Demo video recording | Jessie (recording) + Zylos200 (editing) | Pending | Multi-angle: Web Console + TG + GitHub |
| 3 | Article #1: "My team has 8 people, 4 are AI Agents" | Zylos200 (draft) → Kevin (review + publish) | Pending | Kevin IP is distribution core |
| 4 | ClawFeed viral article analysis | Zylos200 | Done | PDF sent to Charlie |
| 5 | Operation manual v1 (CLI Quick Start) | Zylos200 (framework) + AllenBot (tech steps) | In progress | |

### Product & Dev

| # | Task | Owner | Status | Notes |
|---|------|-------|--------|-------|
| 6 | Read-only thread viewer MVP | Jessie | Pending | 2-3 days, viewer_token + share link (Notion-style) |
| 7 | Product readiness assessment | Zylos200 | Done | Ready to push to PR #13 |

### Customer Prep

| # | Task | Owner | Status | Notes |
|---|------|-------|--------|-------|
| 8 | White-glove onboarding plan (50 users) | Zylos200 (plan) → Allen/Kevin (confirm) | Pending | |
| 9 | Landing page copy | Zylos200 | Pending | |

---

## Week 2: GTM Launch (Mar 8-14)

### Launch Day

| # | Task | Owner | Notes |
|---|------|-------|-------|
| 10 | Article publish | Kevin | Twitter (EN) + WeChat (CN) simultaneously |
| 11 | KOL amplification | Allen (budget/coordination) + Zylos200 (KOL outreach) | Budget: $500-1000 |
| 12 | Product Hunt launch | Kevin/Allen decide | Same day or delay 1 week |
| 13 | Zhihu/Jike/Xiaohongshu publish | Zylos200 | Platform-specific versions |

### Customer Onboard

| # | Task | Owner | Notes |
|---|------|-------|-------|
| 14 | First seed customer onboard (white-glove) | Jessie (tech setup) + Allen/Kevin (customer intro) | |
| 15 | Customer feedback collection | Zylos200 | Design feedback mechanism |

---

## Week 3-4: Iterate (Mar 15-28)

| # | Task | Owner | Est. |
|---|------|-------|------|
| 16 | Customer Dashboard | Jessie | 3-5 days |
| 17 | Self-service registration page | Jessie | 3-5 days |
| 18 | Article #2: "Stop Having Meetings" | Zylos200 (draft) | |
| 19 | Article #3: "Your Team Doesn't Need More People" | Zylos200 (draft) | |

---

## Role Summary

| Role | Person | Key Responsibilities |
|------|--------|---------------------|
| **Founder IP** | Kevin | Review + publish articles, confirm PH timing, intro seed customers |
| **Biz Lead** | Allen | Marketing budget, KOL coordination, intro seed customers, daily progress review |
| **Tech Lead (Agent)** | Jessie | Viewer MVP dev, demo recording, white-glove tech setup, Dashboard + registration dev |
| **Content (Agent)** | Zylos200 | Articles, demo script, operation manual, product readiness, landing page, onboarding plan, daily standup summary |
| **Tech Writer (Agent)** | AllenBot | Operation manual tech steps, demo scene review, GTM strategy execution |

---

## Jessie Review Notes

1. **Timeline is aggressive but feasible** if we execute in parallel. Week 1 content (Zylos200) and viewer MVP (Jessie) can happen simultaneously.
2. **Viewer MVP is the critical path** for Week 2 launch — seed customers need somewhere to "see for themselves" after the demo. The viewer_token share link approach avoids building a full auth system.
3. **White-glove onboarding (task #8) needs more detail** — 50 users at once means we need: batch ticket generation, a clear setup guide per customer, and monitoring for Hub capacity. Current single-node Hub may need load testing.
4. **Missing from plan: Hub capacity check.** Current deployment is single-node PM2. 50 concurrent WebSocket connections should be fine, but we should load test before Week 2.
5. **Daily standup cadence** — suggest using HxA Connect thread (bcd49692) as the standup channel, consistent with how we're already working.
