# RESEARCH

This document records the source and verification date for every statistic and tool claim used in this skill's reference files. It exists so anyone using this skill, or auditing it before relying on it, can check a claim against its original source instead of taking it on faith.

All claims below were checked in June 2026. Search-tool pricing, AI search statistics, and platform features change frequently. Anyone using this skill after that date should re-verify any number before quoting it in a real deliverable, especially pricing.

---

## Why this document exists

Keyword research lives or dies on accurate, current information. A skill that hands over stale tool pricing or a misattributed statistic isn't saving anyone time; it's creating rework. This document separates "this is a sourced, checked fact" from "this is general industry knowledge repeated without a specific source," so nothing in the reference files is presented as more certain than it actually is.

## Methodology

Each claim was checked against either the originating primary source (a vendor's own page, a research firm's own published study) or, where multiple independent sources converged on the same figure, against at least two independent sources. Where sources genuinely conflicted, that conflict is noted explicitly in the reference file itself rather than resolved by picking one number arbitrarily.

## Verified claims by reference file

### core-keyword-fundamentals.md

| Claim | Source | Verified |
|---|---|---|
| Ahrefs Keyword Difficulty bands (0-10 easy, 11-30 medium, 31-70 hard, 71-100 very hard) | ahrefs.com/blog/keyword-difficulty/ | June 2026 |
| Keysearch pricing: $24/mo Starter, $48/mo Pro | Keysearch's own pricing page, cross-checked against independent 2026 review/comparison sites | June 2026 |
| Ubersuggest pricing | Flagged as an unresolved conflict: independent sources disagree on current tier structure ($12-40/mo tiered vs. $29+/mo credit-based reported elsewhere) | June 2026, unresolved; confirm at neilpatel.com/ubersuggest directly |
| Tailwind's free Pinterest keyword tool exists and requires no account | tailwindapp.com/pinterest-marketing/tools/keyword-finder | June 2026 |

### pinterest-keyword-research.md

| Claim | Source | Verified |
|---|---|---|
| ~96-97% of Pinterest searches are unbranded | business.pinterest.com/insights/effective-reach/ (Pinterest's own Business page); cross-checked against independent Pinterest statistics roundups citing the same range | June 2026 |
| KeywordToPin pricing: $25/$35/$45 per month (Starter/Professional/Expert), 14-day free trial, no credit card required | keywordtopin.com, cross-checked against independent tool-comparison sites | June 2026 |
| PinClicks pricing: $29/mo (Pin Pro), $49/mo (Pin Plus), 5-day free trial | pinclicks.com/pricing | June 2026 |
| Pin Inspector pricing: $67 one-time, lifetime access, free updates | Cross-checked across multiple independent review sources; no single official vendor page was treated as sufficient on its own given this is a smaller, less centrally-documented tool, so convergence across sources was the bar used here | June 2026 |
| Pinterest Trends and Shopping Trends feature set and region availability (US/Canada/UK) | help.pinterest.com/en/business/article/pinterest-trends and Pinterest's own 2026 feature announcements | June 2026 |

### blog-website-seo-keywords.md

| Claim | Source | Verified |
|---|---|---|
| 90.63% of pages get zero organic traffic from Google (original, smaller Ahrefs study) | ahrefs.com/blog/search-traffic-study/ | June 2026 |
| 96.55% of pages get zero organic traffic from Google (newer, larger Ahrefs study, ~14 billion pages) | ahrefs.com/blog/search-traffic-study/, with Ahrefs' own stated caveat that the sample, while large, skews toward higher-quality pages already in their index and isn't a perfectly representative sample of the entire web | June 2026 |
| Yoast SEO's single focus-keyword model | Widely documented as Yoast's own design pattern across SEO industry sources; this is a description of an existing, observable product feature rather than a statistic requiring a primary citation | June 2026 |

### aeo-ai-search-keywords.md

| Claim | Source | Verified |
|---|---|---|
| Query fan-out: AI search systems decompose one query into roughly 8-12 sub-queries using an LLM | Search Engine Journal ("Query Fan-Out Technique in AI Mode: New Details From Google"), Semrush's own explainer, and independent SEO researcher Aleyda Solis's analysis, all converging on the same mechanism and sub-query range | June 2026 |
| 83% of AI citations on commercial queries come from pages updated within the past 12 months | AirOps "State of AI Search" 2026 report | June 2026 |
| 55% of Google AI Overview citations pull from the top 30% of a page (with 24% from the middle third, 21% from the bottom third) | CXL, "Where Google AI Overviews Cite From: A 100-Page Study" (cxl.com/blog/google-ai-overview-citation-sources/) | June 2026 |
| 44.2% of ChatGPT citations specifically come from the first third of a document (a distinct figure from the CXL/Google number above) | Kevin Indig's analysis of 18,000+ verified ChatGPT citations | June 2026 |
| 40-60 word direct-answer blocks are the most commonly cited "extractable" answer length for AI systems | Convergent finding across multiple independent 2025-2026 AEO research write-ups (Averi.ai, LoudFace, and others using comparable methodology) | June 2026 |
| 68.01% of Google searches in early 2026 ended without a click (roughly 32% click-through) | SparkToro, using Similarweb clickstream panel data, June 2026 study (sparktoro.com/blog/in-2026-less-than-one-third-of-google-searches-still-send-a-click/) | June 2026 |

## Known limitations

- **Pricing drifts fast.** Every tool price in this skill is a snapshot from June 2026. SaaS pricing changes without advance notice across the entire industry; this isn't specific to any one vendor.
- **The Ahrefs zero-traffic study sample isn't a perfect cross-section of the web.** Ahrefs has said as much about its own research. The headline point (most published content gets little to no organic traffic) is well-supported regardless, but the exact percentage shouldn't be treated as a precise measurement of "the entire internet."
- **AI search statistics are a young, fast-moving research area.** Methodologies differ between studies (sample size, which AI system was studied, how "citation" was defined), which is why this document deliberately keeps the Google AI Overview figure (55%) and the ChatGPT-specific figure (44.2%) separate rather than averaging them into one number.
- **Ubersuggest's pricing conflict was not resolved.** Independent sources disagreed enough that picking one figure would have meant presenting an unverified number as settled fact, which this skill's own validation rule explicitly prohibits. The reference file flags this directly instead.

## How to keep this current

Anyone maintaining a fork of this skill should periodically re-run the verification process described above: check vendor pricing pages directly, and re-search for newer versions of the cited studies (search engines and AI platforms publish updated research on these topics regularly). If a claim in this document is found to be outdated, update both the reference file and this document together so they stay in sync.
