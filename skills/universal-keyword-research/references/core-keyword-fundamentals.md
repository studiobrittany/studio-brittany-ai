# CORE KEYWORD FUNDAMENTALS

Universal concepts that apply no matter what's being researched: a blog post, a Pinterest pin, an Etsy listing, an email subject line, a YouTube title, an AI Overview answer block. Read this file first for any keyword research request. Route to the platform-specific files for the execution layer.

---

## 1. SEED KEYWORDS, WHERE RESEARCH STARTS

A seed keyword is the broad starting phrase everything else branches from ("notion templates," "meal planning," "freelance contracts"). Generate seeds from:

- The product, service, or post topic itself, stated the way a customer or searcher would say it, not the way the business describes it internally
- Customer language: actual questions asked in DMs, comments, reviews, or support requests
- Competitor titles and listings for the same topic or product
- Autocomplete on the platform in question (Google, Pinterest, YouTube, Etsy, and Amazon all have their own autocomplete and it's free)

Free brainstorming sources, all still active and free as of this writing:
- Google/YouTube/Pinterest/Etsy/Amazon search bar autocomplete (the best free source there is, and it's platform-specific phrasing)
- Google Trends (trends.google.com): free, shows relative interest over time and by region
- AnswerThePublic (answerthepublic.com): free tier capped at 3 searches/day, visualizes question-based and preposition-based variations
- Ahrefs' free Keyword Generator: free tier, capped results, still useful for a quick seed expansion

## 2. SEARCH INTENT, THE FOUR TYPES

Every keyword carries an intent. Matching content to the wrong intent is the single most common reason content ranks but doesn't convert.

| Intent | What the searcher wants | Example | Best-fit content |
|---|---|---|---|
| Informational | An answer or explanation | "how does pinterest seo work" | Blog post, guide, FAQ |
| Navigational | A specific brand/site/page | "acme studio etsy shop" | Branded landing page |
| Commercial investigation | Comparing options before buying | "best notion template for content creators" | Comparison post, review, roundup |
| Transactional | Ready to buy/download/sign up now | "buy notion content planner template" | Product/sales page, listing |

Most keyword tools also tag a fifth label, branded vs. unbranded: whether the query contains a brand name. This matters most for Pinterest (see `pinterest-keyword-research.md`) and for any competitive-gap work, since unbranded queries are where new audience actually gets found.

## 3. MATCHING TERMS VS. RELATED TERMS

A distinction that shows up across most paid tools (Ahrefs calls it this explicitly, Semrush and others use the same logic under different labels):

- **Matching terms:** keywords that literally contain the seed phrase ("notion template" → "notion template for creators," "free notion template")
- **Related terms:** keywords that don't contain the seed phrase but rank for the same intent or get searched by the same audience ("notion template" → "digital planner," "content system notion")

Related terms are where the actual content gaps live. Matching-terms-only research produces an obvious, crowded keyword list. Related-terms research finds the angle nobody else is targeting.

## 4. CLUSTERING AND PARENT TOPICS

Keywords cluster around a single "parent topic" when they'd realistically be answered by the same piece of content. The parent topic "pinterest keyword research," for example, might cluster: "pinterest seo," "pinterest keywords for etsy," "how to find pinterest keywords," "pinterest keyword tool." Building one strong piece of content per cluster (a pillar page, a comprehensive blog post, a deep board) beats writing five thin pieces that all compete with each other for the same intent.

## 5. THE SIX METRICS, AND WHEN EACH ONE ACTUALLY MATTERS

| Metric | What it measures | When to weight it heavily |
|---|---|---|
| Search Volume | Estimated monthly searches | Top-of-funnel, awareness content |
| Traffic Potential | Estimated total traffic the top-ranking page gets across ALL keywords it ranks for, not just the one searched | Planning a pillar/cornerstone piece |
| Keyword Difficulty (KD) | How hard it is to rank, generally modeled off the number/strength of referring domains pointing at the current top results | Any time budget or domain authority is limited, which describes most small or solo-run sites |
| CPC | What advertisers pay per click | Signal for commercial intent and real buyer interest, even without running ads yourself |
| Growth | Trend direction over time | Catching something rising before competition catches up |
| Business Potential | 0 to 3 scale, how directly a keyword's content could promote what's actually being sold | The metric that matters most for a small business or solo creator. High volume with zero business potential is a vanity metric |

KD bands, confirmed against Ahrefs' own published scale (ahrefs.com/blog/keyword-difficulty/) as of June 2026: 0-10 = easy, 11-30 = medium, 31-70 = hard, 71-100 = very hard. "Hard" and above is generally out of reach for a site without a strong existing backlink profile, though low KD doesn't guarantee easy competition either; KD is a starting signal, not the only one.

## 6. PRIORITIZATION SCORING, THE PRACTICAL VERSION

For a solo creator or small team without an enterprise tool budget, score every keyword candidate 1 to 5 on four axes and rank by total:

1. **Relevance:** does this keyword's intent actually match what's being sold or written?
2. **Volume:** is there a real audience searching this (even directionally, without an exact number)?
3. **Winnability:** realistic chance of actually showing up for this, given current domain/account strength
4. **Business potential:** would ranking or showing up for this actually move someone toward a sale, subscribe, or save?

A keyword scoring 4-5-3-5 beats a keyword scoring 5-5-1-1 almost every time. Volume without winnability or business potential is noise.

## 7. THE NON-NEGOTIABLE VALIDATION RULE

AI-brainstormed keyword ideas (from Claude, ChatGPT, or any LLM) are a starting list, never a finished one. An LLM can suggest a keyword phrase nobody actually searches, or miss the exact phrasing real searchers use. Before any keyword goes into a final deliverable:

- Check it against real autocomplete on the actual platform (incognito/logged-out, so personalization doesn't skew it)
- Cross-check volume/difficulty in an actual tool where one is available
- Flag clearly, in the deliverable itself, which keywords are tool-validated vs. brainstormed-and-not-yet-verified. Never present a brainstormed guess with the same confidence as verified data

## 8. THE 2026 TOOL LANDSCAPE

Every price and feature claim below was checked against the vendor's own site or a converging set of independent sources in June 2026. Pricing changes without much notice industry-wide; confirm current pricing on the vendor's own site before it goes into a budget conversation or a client-facing document.

**Free, no payment info required:**
- Google Keyword Planner: free with a Google Ads account, range-based volume bands (no exact number without active ad spend), still the most reliable free baseline for Google search behavior
- Google Trends: free, relative interest over time, regional breakdowns
- AnswerThePublic: free tier, 3 searches/day cap, limited volume/CPC depth, 30-keyword export cap
- Ahrefs Free Keyword Generator: free, capped result list, decent for quick seed expansion
- Pinterest Trends (trends.pinterest.com): free, built into every Pinterest business account (see `pinterest-keyword-research.md`)
- Tailwind's Pinterest keyword tool: free, no account required, generates keyword suggestions from a website URL. Useful as a no-cost first pass if Pinterest scheduling is already part of the workflow

**Paid, market-leading:**
- Ahrefs: largest market share in the category, deep keyword and backlink database, the most complete version of the six-metrics view above
- Semrush: close competitor to Ahrefs, comparable depth, added AI-visibility tracking features in 2026

**Paid, budget-friendlier:**
- Keysearch: $24/month (Starter) or $48/month (Pro) as of June 2026, with annual billing discounts available; frequently used by solo creators and small blogs
- Ubersuggest: pricing varies meaningfully by source at the time of writing (some list a $12 to 40/month tiered structure, others a $29+/month credit-based structure). This is a genuine source conflict, not settled. Confirm directly at neilpatel.com/ubersuggest before quoting a number

**Pinterest-specific:** see `pinterest-keyword-research.md` for third-party Pinterest tools and their current pricing.

## 9. COMMON MISTAKES

- Keyword stuffing: modern search (and AI search) rewards natural phrasing that answers the actual query, not repetition
- Chasing high volume with zero business potential: traffic that can't convert isn't worth the effort it costs
- Going straight for "hard" difficulty keywords with no existing authority to back it up
- Dismissing long-tail keywords as "too small to matter": long-tail, lower-volume, high-intent keywords convert at a much higher rate and are realistically winnable
- Treating one platform's keyword data as universal: Pinterest search phrasing, Google search phrasing, and AI chat phrasing are three different languages for the same intent (see the platform-specific reference files)
- Presenting an unverified, brainstormed keyword as if it were confirmed search data
