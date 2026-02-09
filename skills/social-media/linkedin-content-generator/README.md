# LINKEDIN CONTENT BUILDER

> A comprehensive Claude skill that generates engaging LinkedIn posts, polls, and articles for entrepreneurs, thought leaders, and LinkedIn content creators—without generic “AI slop” or "Hustle Bro" tones.

![License](https://img.shields.io/badge/license-Repo%20LICENSE-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
![Claude](https://img.shields.io/badge/claude-3.5%2B-orange.svg)

## START HERE

1. [READ THE SKILL](./SKILL.md)
2. [HOW TO USE IT](./README.md)
3. [SEE REAL EXAMPLES](./examples/examples.md)
4. [CHECK TEST COVERAGE](./docs/testing-notes.md)

## REFERENCE LIBRARY

- [RESEARCH](./docs/research.md)
- [BEST PRACTICES](./docs/best-practices.md)

## TEMPLATES

- [HOOK TEMPLATES](./templates/hook-templates.md)
- [CONTENT FRAMEWORKS](./templates/content-frameworks.md)
- [CTA EXAMPLES](./templates/cta-examples.md)
- [CAROUSEL TEMPLATE](./templates/carousel-template.md)
- [PROFILE TEMPLATES](./templates/profile-templates.md)

## QUICK LINKS

- [OVERVIEW](#overview)
- [WHO THIS HELPS](#who-this-helps)
- [FEATURES](#features)
- [USAGE GUIDE](#usage-guide)
  - [HOW TO TRIGGER THIS SKILL](#how-to-trigger-this-skill)
  - [TOPIC](#topic)
- [OUTPUT FORMATS](#output-formats)
  - [LINKEDIN POST (DEFAULT)](#linkedin-post-default)
  - [LINKEDIN POLL](#linkedin-poll)
  - [LINKEDIN ARTICLE](#linkedin-article)
- [WHAT THIS SKILL WILL NOT DO](#what-this-skill-will-not-do)
  - [TESTING](#testing)
- [QUICK START](#quick-start)
  - [PREREQUISITES](#prerequisites)
  - [RESOURCES](#resources)
  - [INSTALLATION](#installation)
- [LICENSE](#license)


## OVERVIEW
LinkedIn rewards writing that is **specific, structured, and discussion-worthy**. This skill produces LinkedIn-native content designed to earn meaningful engagement (comments, saves, shares) by combining:
- hook engineering (strong first 1–2 lines)
- skimmable structure (short paragraphs, deliberate pacing)
- real substance (clear claims, examples, decision rules)
- integrity guardrails (no fake citations, no invented stats)

This skill is built for creators who want high-performing content that still reads like a human with a (smart) brain wrote it.

## WHO THIS HELPS
- Entrepreneurs building audience and pipeline
- Thought leaders building authority and trust
- LinkedIn content creators optimizing output quality and consistency

## FEATURES
- ✅ Generates **posts** with alternate hooks, short version, CTAs, and optional hashtags
- ✅ Generates **polls** with distinct options and a discussion-starter pinned comment prompt
- ✅ Generates **articles** with titles, outline, intro, one full section, and closing CTA
- ✅ Includes **anti–AI slop** rules (no filler, no rambling, no template-y phrasing)
- ✅ Enforces **integrity** (no fake sources, citations, quotes, stats, or invented credibility)

---

## USAGE GUIDE

### HOW TO TRIGGER THIS SKILL

This skill should activate when a user asks for:

“Write a LinkedIn post about…”

“Create a LinkedIn poll about…”

“Draft a LinkedIn article about…”

“Rewrite this LinkedIn post to be tighter / more engaging / less generic”

“Give me hooks / angles / post ideas for LinkedIn”

Best Results: Provide These Inputs

### TOPIC

High-leverage additions:
- Audience (who it’s for)
- Goal (comments, saves, shares, clicks, leads)
- Angle (tactical, contrarian, story-led, teardown, framework)
- Proof point (a real example, number, observation, or lesson learned)
- CTA (comment keyword, follow, DM, newsletter, consult)

## OUTPUT FORMATS

### LINKEDIN POST (DEFAULT)

You should receive:
- Primary draft
- Two alternate hooks
- Short version (≤ 900 characters)
- CTA options (3)
- Optional hashtags (max 5; niche-specific)

### LINKEDIN POLL

You should receive:
- Poll question (one sentence)
- Four distinct options (no overlap)
- Short description (context)
- Pinned-comment prompt (invites thoughtful replies)

### LINKEDIN ARTICLE

You should receive:
- Title options (3)
- Subtitle (1)
- Outline (H2/H3 structure)
- Intro (150–250 words)
- One fully written section
- Closing CTA

## WHAT THIS SKILL WILL NOT DO

❌ Invent citations, studies, stats, quotes, or “proof”
❌ Ramble to sound smart
❌ Produce generic motivational filler
❌ Guarantee outcomes or “virality”

### TESTING

See:
- testing-notes.md for trigger tests, refusal tests, and quality checks
- examples.md for realistic scenarios and expected output patterns

---

## QUICK LINKS (AGAIN)

1. [READ THE SKILL](./SKILL.md)
2. [HOW TO USE IT](./README.md)
3. [SEE REAL EXAMPLES](./examples/examples.md)
4. [CHECK TEST COVERAGE](./docs/testing-notes.md)

## REFERENCE LIBRARY

- [RESEARCH](./docs/research.md)
- [BEST PRACTICES](./docs/best-practices.md)

## TEMPLATES

- [HOOK TEMPLATES](./templates/hook-templates.md)
- [CONTENT FRAMEWORKS](./templates/content-frameworks.md)
- [CTA EXAMPLES](./templates/cta-examples.md)
- [CAROUSEL TEMPLATE](./templates/carousel-template.md)
- [PROFILE TEMPLATES](./templates/profile-templates.md)


### PREREQUISITES
- Claude 3.5 Sonnet or above
- A working Claude skills setup (local path installation)

### INSTALLATION
1. Create the skill directory:
   ```bash
   mkdir -p /mnt/skills/user/linkedin-content-builder

---

### LICENSE
This repository is licensed under **Creative Commons Attribution 4.0 International (CC BY 4.0)**.

This skill uses the **repo-level** license.
- [LICENSE](../../../LICENSE)

© 2026 STUDIO BRITTANY™


