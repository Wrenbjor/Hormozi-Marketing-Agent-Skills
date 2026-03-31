# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

A Claude Code plugin containing six agent skills based on Alex Hormozi's marketing frameworks (*$100M Offers*, *$100M Leads*). There is no application code, build system, or test suite — the repo is pure content in Markdown.

## Repository Structure

- `plugin.json` — Plugin manifest that registers all six skills by directory path
- `skills/<name>/SKILL.md` — Each skill is a single Markdown file with YAML frontmatter (`name`, `description`) followed by the framework content

## The Six Skills and Their Pipeline

```
Offer Creation → Lead Generation → Sales & Closing → Monetization & Value
      ↑                                                       |
      └──── Content & Copywriting (fuels all stages) ────────┘
                    Business Scaling (operates across all)
```

| Skill Directory | Domain |
|----------------|--------|
| `hormozi-offer-creation` | Grand Slam Offers, Value Equation, guarantee engineering, pricing |
| `hormozi-lead-generation` | Core Four channels, lead magnets, outreach, paid ads, nurture |
| `hormozi-sales-closing` | CLOSER framework, objection handling (price/spouse/time/trust) |
| `hormozi-monetization-value` | LTV, pricing psychology, ascension models, retention, churn |
| `hormozi-content-copywriting` | Hooks, PAS/AIDA frameworks, storytelling, platform-specific copy |
| `hormozi-business-scaling` | Growth levers, 4 leverage types, operator-to-owner transition |

Skills cross-reference each other via relative Markdown links (e.g., `../lead-generation/SKILL.md`).

## SKILL.md Format

Every skill file follows this structure:

```markdown
---
name: hormozi-<skill-name>
description: <one-paragraph description used for skill matching/triggering>
---

# Title

## Core Philosophy
<foundational principle>

## Frameworks / Workflows
<step-by-step methodology sections>

## When to Use This Skill
<trigger conditions>
```

## Editing Guidelines

- Maintain consistent YAML frontmatter format — `name` must match the directory name
- Keep the `description` field accurate; it's what Claude uses to decide when to activate a skill
- Frameworks use numbered steps, tables, and code blocks for structured processes — preserve these formats
- When adding or modifying frameworks, follow Hormozi's principle hierarchy: philosophy → equation/model → step-by-step workflow → common mistakes
- Cross-references between skills should use relative paths (`../other-skill/SKILL.md`)
- If adding a new skill, register it in `plugin.json` under the `skills` array
