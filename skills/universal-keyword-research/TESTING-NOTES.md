# Testing Notes

How this skill was validated before release, and what it does and doesn't cover.

## How this was validated

**Self-executability walkthrough:** every step described in `SKILL.md`'s core workflow and in each `references/` file was walked through manually against a realistic scenario (the same scenarios that became `EXAMPLES.md`) to confirm the instructions are followable as written, with no missing steps, no circular references, and no step that assumes information the process hasn't generated yet.

**Cross-file consistency check:** confirmed that every file referenced from `SKILL.md`'s routing table and every cross-reference between `references/` files (for example, the platform files pointing back to `core-keyword-fundamentals.md` for the scoring system) actually exists at the path named, with no dead links or references to files that aren't included in the package.

**Placeholder and dead-content scan:** checked every file for leftover bracketed placeholders, TODO markers, or unfinished sections. None remain. Every example, including the zero-budget edge case in `EXAMPLES.md` Example 9, uses a concrete worked keyword instead of bracketed placeholder text, so the method is demonstrated with a real-looking example rather than a fill-in-the-blank template.

**Fact verification:** every statistic and tool-pricing claim was checked against a named source rather than carried over from general knowledge. Full source list and verification dates are in `RESEARCH.md`. Where independent sources genuinely disagreed (Ubersuggest pricing), the conflict is stated directly in the reference file instead of being resolved by guessing.

**Description-length check:** `SKILL.md`'s frontmatter `description` field was counted programmatically to confirm it fits within platform limits.

## Known limitations

**Tool pricing and features will drift.** Every price quoted in this skill is a snapshot from June 2026. This is true of any document describing SaaS pricing; there's no way around it except periodic re-verification. `RESEARCH.md` lists exactly which claims need rechecking and where to check them.

**One pricing conflict was not resolved.** Independent sources disagree on Ubersuggest's current tier structure. Rather than presenting a guess as fact, the reference file states this is unresolved and points to the vendor's own pricing page. If you're choosing between tools and Ubersuggest is a candidate, confirm its actual current pricing directly before deciding.

**AI search statistics are from a young, fast-moving research field.** The AEO/AI-search-citability figures in `references/aeo-ai-search-keywords.md` come from a small number of independent studies (CXL, Kevin Indig, AirOps, SparkToro) rather than a large, settled body of research the way classic SEO statistics are. These are the best current sources available, but expect newer, larger studies to appear and potentially shift these specific numbers, especially as AI search products themselves continue to change.

**This skill doesn't call any live API or tool.** It's a research methodology, not an integration. It does not pull live search volume, run an actual Ahrefs/Semrush query, or check Pinterest Trends for you. Every "validate against real data" step in this skill means manually checking a tool or platform yourself (or asking Claude to do so via whatever browsing or tool access it has in your specific setup), not an automatic lookup this skill performs on its own.

**English-language search behavior only.** All search-intent patterns, platform behavior notes, and examples assume English-language search. Search behavior, autocomplete quality, and platform feature availability can differ meaningfully in other languages, and this skill hasn't been tested against non-English keyword research.

**No built-in scoring automation.** The 4-axis prioritization system (relevance, volume, winnability, business potential) is a manual scoring framework Claude applies through judgment and whatever data is available, not a calculated formula pulling from a live dataset. Two different research passes on the same keyword could reasonably produce slightly different scores depending on what data was available at the time.

## What to independently verify before relying on this skill

- Any tool price, before it goes into a budget or a client-facing recommendation
- Any search volume, keyword difficulty, or traffic statistic, before it goes into a real strategy document. Treat skill-cited industry statistics (zero-click rate, AI citation patterns, and similar) as directional context, not as a substitute for checking your own specific keyword in an actual tool
- Whether a named tool still exists and still does what's described here. Tools in this space get acquired, rebranded, or discontinued
- Platform feature availability in your specific region. Some Pinterest features mentioned (Shopping Trends, for example) are region-limited as of this skill's last update
