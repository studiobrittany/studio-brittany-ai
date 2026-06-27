# AEO / AI SEARCH KEYWORD RESEARCH

This file covers finding the right questions and queries for AI-driven search (ChatGPT, Perplexity, Google AI Mode, Google AI Overviews): the research layer that happens before any on-page execution (schema markup, FAQ formatting, E-E-A-T signals). This file is strictly about the keyword and query research that happens before any of that gets written.

---

## 1. HOW AEO KEYWORD RESEARCH DIFFERS FROM CLASSIC SEO

Classic SEO keyword research is volume-led: find what gets searched most, target it. AEO (answer engine optimization) keyword research is question-led, intent-led, and answer-format-led. An AI answer engine isn't matching a query to a ranked list of links; it's synthesizing one answer from multiple sources, so the research question shifts from "what do people type" to "what question is actually being asked, and what would a complete, citable answer to it look like."

## 2. FUNNEL-STAGE KEYWORDS (TOFU / MOFU / BOFU)

| Stage | Searcher mindset | Example query |
|---|---|---|
| TOFU (top of funnel) | Just learning, no decision made | "what is a notion template" |
| MOFU (middle of funnel) | Comparing options | "best notion template for content creators" |
| BOFU (bottom of funnel) | Ready to act | "buy notion content planner template" |

AI answer engines pull different source types for each stage: TOFU answers lean on definitional/educational content, BOFU answers lean on comparison and review content with specific named options. Map keyword research to all three stages rather than only the stage that converts, since AI answer engines often cite TOFU content even for users who are further along, simply because it answers the underlying question most directly.

## 3. QUERY FAN-OUT: THE CORE AEO DISCOVERY TECHNIQUE

Confirmed as a real, current, well-documented mechanism behind how AI search actually works as of 2026 (covered in detail by Search Engine Journal, Semrush, and independent SEO researchers including Aleyda Solis): when someone asks an AI search tool a single question, the system doesn't just match that one query. Google has confirmed it uses a custom version of its Gemini model to generate synthetic sub-queries, decomposing the original question into roughly 8 to 12 related sub-queries, running each one, and merging the results into a single synthesized answer. This is not unique to Google; ChatGPT Search, Perplexity, and other AI search tools use comparable approaches. A search for "best pinterest keyword tool" might silently fan out into sub-queries like "pinterest keyword tool pricing," "pinterest keyword tool vs ahrefs," "free pinterest keyword tools," and "pinterest keyword tool reviews 2026," and the final answer pulls from sources that answered each of those, not just the literal phrase typed in.

**How to use this for keyword research:** treat the main query as a parent topic and manually brainstorm its likely fan-out sub-queries: pricing, comparisons, alternatives, reviews, "is it worth it," "how to," and "vs" framings are the most common fan-out shapes. Each sub-query is a candidate H2, FAQ entry, or supporting section. A handful of free tools and browser extensions can surface a model's actual sub-queries directly rather than guessing at them. Worth checking when the budget allows, but manual fan-out brainstorming gets most of the value for free.

## 4. VALIDATING AI-BRAINSTORMED QUERIES AGAINST REAL DATA

The same non-negotiable rule from `core-keyword-fundamentals.md` Section 7 applies here, with extra weight: a fan-out sub-query brainstormed by an LLM (including the one running this skill) is a hypothesis about what an AI search tool might ask itself, not confirmed behavior. Before treating a fan-out list as final:

- Check whether real searchers ask variations of it (autocomplete, AnswerThePublic, "people also ask" boxes)
- Where possible, actually run the parent query across ChatGPT, Perplexity, and Google AI Mode and note how each one rephrases or follows up. Free, takes a few minutes, and is the most direct confirmation available without a paid tool
- Never present a brainstormed fan-out list as if it were observed AI behavior. Label it clearly as a hypothesis until checked

## 5. WHAT MAKES CONTENT CITABLE (RESEARCH-STAGE CONSIDERATIONS)

A few sourced patterns worth keeping in mind while choosing which queries/keywords to actually build content around, since they affect whether the research effort pays off. Every figure below is cited to a specific named source rather than presented as general industry knowledge, and all were checked in June 2026:

- Direct-answer content performs best when the actual answer appears in a tight 40 to 60 word block within the first 150 words. Multiple 2025-2026 AEO studies converge on this range as the most "extractable" answer length for AI systems to quote directly. A query worth targeting is one that can be answered that directly, not one that requires several paragraphs of setup first.
- Freshness carries real weight for commercial and evaluation queries specifically. The AirOps "State of AI Search" 2026 report found 83% of AI citations on commercial queries came from pages updated within the past 12 months, which makes "evergreen but never revisited" content a weaker AEO bet than it is for classic SEO.
- A CXL study analyzing 100 pages of Google AI Overview citations found 55% of citations pulled from content in the top 30% of the page, with another 24% from the middle third and the remaining 21% from the bottom third (cxl.com/blog/google-ai-overview-citation-sources/). A separate, larger study of ChatGPT citations specifically (Kevin Indig's analysis of over 18,000 verified citations) found a comparable but distinct figure of 44.2% from the first third of a document. These are two different AI systems with two different exact numbers; both point the same direction, but they shouldn't be quoted interchangeably.
- Click-through behavior on Google has continued to decline as AI Overviews expand. A June 2026 SparkToro study, using Similarweb clickstream data, found 68.01% of Google searches in the first four months of 2026 ended without any click, meaning roughly 32% of searches now send a click at all, down from about 60% zero-click in 2024 (sparktoro.com/blog/in-2026-less-than-one-third-of-google-searches-still-send-a-click/). A growing share of search behavior gets fully answered inside the search/AI surface itself, which is a real argument for treating visibility and citation as a legitimate goal even when it doesn't produce a click.

## 6. WORKFLOW

1. Identify the core question or topic
2. Map it to TOFU/MOFU/BOFU and confirm which stage(s) actually matter for this content
3. Brainstorm likely fan-out sub-queries (pricing, comparison, alternatives, "how to," "is it worth it," "vs")
4. Validate the sub-queries against real autocomplete, "people also ask," or a direct check across 2 to 3 AI search tools
5. Rank the validated list using the 4-axis scoring system in `core-keyword-fundamentals.md`
6. Hand the validated query list to whatever on-page SEO/content step comes next for execution (schema markup, FAQ formatting, direct-answer blocks)
