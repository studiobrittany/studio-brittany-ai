# Universal Keyword Research

A Claude skill that teaches Claude a complete, platform-agnostic keyword research methodology: how to find the actual words real people search for, tag the intent behind them, validate them against real data, and prioritize them, before any content gets written.

This is a research process, not a content generator. It produces a validated, ranked keyword list. What you do with that list (write the blog post, build the pin, draft the listing) happens after, using whatever other tools or skills you already use for that.

## Who this is for

Anyone creating content for a search-driven platform: bloggers, Etsy/Gumroad/Shopify sellers, Pinterest creators, YouTubers, course creators, newsletter writers, or anyone optimizing content for AI search tools (ChatGPT, Perplexity, Google AI Mode). No coding knowledge required. No paid tools required, though the skill covers both free and paid options.

## What's included

```
universal-keyword-research/
├── SKILL.md                                   (entry point, read this first)
├── README.md                                  (this file)
├── EXAMPLES.md                                (9 worked examples across platforms)
├── RESEARCH.md                                (sources and verification dates for every stat/claim)
├── CHANGELOG.md                                (version history)
├── TESTING-NOTES.md                            (how this was validated, known limitations)
├── LICENSE.txt                                 (MIT license)
└── references/
    ├── core-keyword-fundamentals.md           (intent types, metrics, scoring, the validation rule)
    ├── pinterest-keyword-research.md          (Pinterest-specific tools and process)
    ├── blog-website-seo-keywords.md           (blog/website SEO-specific process)
    └── aeo-ai-search-keywords.md              (AI search / answer engine optimization)
```

## What this skill actually does

Tell Claude what you're creating content for (a blog post, a Pinterest pin, an Etsy listing, anything search-driven), and the skill walks Claude through:

1. Generating seed keywords in the actual words a searcher would use
2. Expanding that seed list (autocomplete, related-term tools, brainstorming)
3. Tagging the search intent behind each keyword (informational, navigational, commercial investigation, transactional)
4. Validating brainstormed keywords against real data instead of presenting guesses as facts
5. Scoring and ranking the list so you know what to act on first
6. Handing over a finished, organized keyword list ready for whatever you write next

It also includes platform-specific depth for Pinterest, blog/website SEO, and AI search optimization, since each of those has its own quirks that a generic process misses.

## Requirements

- A Claude plan with code execution / file creation enabled (Free, Pro, Max, Team, or Enterprise), or Claude Code
- No paid keyword tools required. The skill works with free tools (search engine autocomplete, Pinterest's own free features, Google Trends) and covers paid tools as optional upgrades, not requirements

## Installation

### Option A: Claude.ai, Claude Desktop, or Cowork

1. Download this repository as a ZIP, or clone it, then re-zip just the `universal-keyword-research` folder so the ZIP contains the folder itself at its root (not the files loose inside the ZIP)
2. In Claude, go to **Settings > Capabilities** and make sure **Code execution and file creation** is turned on
3. Go to **Customize > Skills**
4. Click the **+** button, then **+ Create skill**
5. Select **Upload a skill**
6. Upload the ZIP file
7. The skill will appear in your skills list. Toggle it on
8. Test it by asking Claude something like "do keyword research for a blog post about meal prepping"

### Option B: Claude Code

1. Download or clone this repository
2. Copy the `universal-keyword-research` folder into one of these locations:
   - `~/.claude/skills/universal-keyword-research/` to make it available in every project on your machine
   - `<your-project>/.claude/skills/universal-keyword-research/` to make it available only inside one project
3. Restart Claude Code
4. Run `/skills` to confirm it loaded
5. Test it by asking Claude something like "do keyword research for a blog post about meal prepping"

## How to use it

Just describe what you need in plain language. Some examples:

- "Do keyword research for a Pinterest pin about budget meal planning"
- "I need a content calendar for a fitness blog focused on home workouts, give me a full keyword cluster map"
- "What keywords should I use for an Etsy listing for a digital wedding invitation template"
- "Help me figure out what questions to target so ChatGPT actually cites my article on remote work productivity"
- "What should I title this YouTube video about air fryer recipes"

Claude will ask what platform(s) and what the content is for if it isn't already clear, then run the actual research process described in `SKILL.md` and the relevant `references/` file.

## A note on accuracy

Every statistic and tool claim in this skill's reference files was checked against a named, current source as of the date in `SKILL.md`'s frontmatter (`last_updated`). See `RESEARCH.md` for the full source list. Tool pricing especially changes without notice, so always confirm current pricing at the vendor's own site before it goes into a real budget decision. If you're reading this well after the `last_updated` date, treat every number in this skill as a starting point to re-verify, not a current fact.

## Troubleshooting

**Claude isn't using the skill when I ask a keyword question.**
Check that the skill is toggled on (Claude.ai/Desktop/Cowork: Customize > Skills; Claude Code: run `/skills` to confirm it's loaded). If it's on and still not triggering, be more explicit: "use the universal keyword research skill to..." Claude decides whether to invoke a skill partly based on how closely your request matches the skill's description, so a vague request can sometimes get missed.

**The ZIP upload failed in Claude.ai/Desktop/Cowork.**
The most common cause is folder structure: the ZIP must contain the `universal-keyword-research` folder itself as the root of the ZIP, not the files sitting loose at the ZIP's top level. Re-zip the folder (not its contents) and try again. Also confirm the folder name and the `name` field in `SKILL.md`'s frontmatter match.

**Claude Code doesn't show the skill after I copied the folder in.**
Restart Claude Code completely after copying the folder; skills are loaded at startup. Then run `/skills` to confirm. Double-check the folder path: it must be `~/.claude/skills/universal-keyword-research/` or `<project>/.claude/skills/universal-keyword-research/`, with `SKILL.md` directly inside that folder, not nested in an extra subfolder.

**A tool mentioned in the reference files no longer exists, or its pricing is wrong.**
This is expected over time. SaaS tools change pricing and features without notice. Treat any specific price or feature claim as a snapshot from the `last_updated` date and re-confirm at the vendor's own site. If you want to fix it for your own copy, the relevant claim and its original source are listed in `RESEARCH.md`, so you can find exactly what to update and where.

**A statistic seems off or outdated.**
Check `RESEARCH.md` first; it lists the source and verification date for every claim. If you find a more current figure, update both the reference file containing the claim and the corresponding row in `RESEARCH.md` so they stay in sync.

**I want to use this for a platform that isn't covered (TikTok, Amazon, App Store, etc.).**
The core process in `references/core-keyword-fundamentals.md` (seed generation, intent tagging, validation, scoring) applies to any search-driven platform, even without a dedicated reference file. Tell Claude which platform you're working with and ask it to apply the same process using that platform's own native search/autocomplete features as the validation source.

**I don't know which file does what.**
Start with `SKILL.md`; it has a routing table that points to the right reference file for whatever you're working on. You generally don't need to read the reference files yourself; Claude reads them when the skill is invoked.

## License

MIT License. See `LICENSE.txt`. Free to use, modify, and redistribute, including commercially, with attribution preserved per the license terms.

## Credit

Built by Studio Brittany (Brittany Parks).
