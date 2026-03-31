# Hormozi Marketing Agent Skills

Six Claude agent skills that give AI assistants the complete Alex Hormozi business and marketing playbook. Each skill covers a distinct phase of the business-building pipeline — from crafting irresistible offers to scaling beyond founder-dependent operations.

## Skills

| Skill | Trigger Name | Description |
|-------|-------------|-------------|
| **Offer Creation & Pricing** | `hormozi-offer-creation` | Creates irresistible Grand Slam Offers using Alex Hormozi's $100M Offers framework. Applies the Value Equation, dream outcome stacking, bonus architecture, guarantee engineering, scarcity/urgency triggers, and pricing strategy. Use when building offers, pricing products/services, creating bonuses, writing guarantees, structuring packages, or making any offer more compelling. |
| **Sales & Closing** | `hormozi-sales-closing` | Closes deals using Alex Hormozi's CLOSER framework, objection handling system, and high-ticket sales methodology. Covers the full sales conversation arc from rapport to close, with specific scripts for handling price, spouse, time, and trust objections. Use when writing sales scripts, preparing for sales calls, training sales teams, handling objections, or improving close rates on any offer. |
| **Content & Copywriting** | `hormozi-content-copywriting` | Creates high-converting content and sales copy using Alex Hormozi's frameworks for hooks, headlines, storytelling, calls-to-action, and audience-building content strategy. Covers YouTube titles, email campaigns, ad copy, social media posts, landing pages, and long-form content. Use when writing any marketing content, headlines, hooks, emails, ads, social posts, video scripts, or sales pages. |
| **Lead Generation** | `hormozi-lead-generation` | Generates leads using Alex Hormozi's $100M Leads framework covering the Core Four acquisition channels, lead magnet creation, warm/cold outreach strategies, paid advertising, and content-based lead generation. Use when building lead generation systems, creating lead magnets, planning outreach campaigns, setting up ad funnels, growing an audience, or diagnosing why leads aren't converting. |
| **Business Scaling** | `hormozi-business-scaling` | Scales businesses using Alex Hormozi's frameworks for growth levers, leverage types, hiring and team building, operational systems, and the Acquisition.com portfolio model. Covers diagnosing growth bottlenecks, choosing the right business model, building systems that run without the founder, and making the transition from operator to owner. Use when planning business growth, hiring, building systems, diagnosing bottlenecks, choosing a business model, or scaling beyond founder-dependent revenue. |
| **Monetization & Value** | `hormozi-monetization-value` | Maximizes business profitability and customer lifetime value using Alex Hormozi's frameworks for pricing psychology, ascension models, retention systems, audience monetization, and unit economics optimization. Use when optimizing pricing, reducing churn, building recurring revenue, monetizing an audience, creating product ladders, improving profit margins, or designing customer retention systems. |

## How They Work Together

The skills form a natural business-building pipeline:

```
Offer Creation → Lead Generation → Sales & Closing → Monetization & Value
      ↑                                                       |
      └──── Content & Copywriting (fuels all stages) ────────┘
                    Business Scaling (operates across all)
```

Start with **Offer Creation** to build something worth selling, use **Lead Generation** and **Content** to fill the pipeline, close with **Sales**, then maximize returns with **Monetization**. **Business Scaling** applies whenever you're ready to grow beyond founder-dependent operations.

## Installation

### Method 1 — Claude Code plugin (recommended)

```bash
claude plugin marketplace add Wrenbjor/Hormozi-Marketing-Agent-Skills
claude plugin install hormozi-marketing-skills@Hormozi-Marketing-Agent-Skills
```

### Method 2 — Manual copy

```bash
git clone git@github.com:Wrenbjor/Hormozi-Marketing-Agent-Skills.git
cp -r Hormozi-Marketing-Agent-Skills/skills/* ~/.claude/skills/
```

## Compatibility

- **Claude Code** (CLI, desktop app, VS Code/JetBrains extensions)
- **Claude.ai** — upload individual skill folders as zipped skills via Settings > Features > Skills
- **Cursor** and any editor that supports SKILL.md-based agent skills
- **Claude API** — load via the `/v1/skills` endpoint

## Directory Structure

```
Hormozi-Marketing-Agent-Skills/
├── plugin.json
├── README.md
└── skills/
    ├── hormozi-business-scaling/
    │   └── SKILL.md
    ├── hormozi-content-copywriting/
    │   └── SKILL.md
    ├── hormozi-lead-generation/
    │   └── SKILL.md
    ├── hormozi-monetization-value/
    │   └── SKILL.md
    ├── hormozi-offer-creation/
    │   └── SKILL.md
    └── hormozi-sales-closing/
        └── SKILL.md
```

## Credits

Skills inspired by Alex Hormozi's marketing frameworks from *$100M Offers* and *$100M Leads*. Built by [WCR Studios](https://wcrstudios.com).

---

This plugin can also be found on:
- [skillsmp.com](https://skillsmp.com) — the Claude skills marketplace
- awesome-claude-skills community repositories
