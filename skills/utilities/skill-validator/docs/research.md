# SKILL VALIDATOR RESEARCH AND METHODOLOGY

**CREATED:** 2026-02-09  
**PURPOSE:** Document the design rationale behind the validator and the standards it enforces.

## BACKGROUND

Skill repositories tend to fail in predictable ways:
- YAML frontmatter breaks loaders and parsers
- Markdown breaks rendering or navigation
- Instructions are too vague to reproduce
- Example coverage is too thin to learn from
- Supporting docs are missing or placeholder-only

This validator exists to reduce those failures by enforcing a repeatable quality bar.

## DESIGN GOALS

1. **STRUCTURAL CORRECTNESS**  
   Ensure skills render and parse reliably.

2. **REPRODUCIBILITY**  
   Ensure a stranger can follow the steps and get similar results.

3. **COMPLETENESS**  
   Ensure the supporting documentation package is present and useful.

4. **SCALABILITY**  
   Ensure the process works for both small and complex skills.

## METHODOLOGY

The validator uses a layered review model:

- **LAYER 1: STRUCTURE** (YAML + file layout)
- **LAYER 2: MARKDOWN TECHNICAL QUALITY** (headers, links, code fences)
- **LAYER 3: CONTENT QUALITY** (triggers, steps, success criteria)
- **LAYER 4: DOCUMENTATION** (required files + troubleshooting)
- **LAYER 5: AUDIENCE FIT** (public-readiness; no private context)

## WHY REQUIRE SIX FILES

Each file answers a different user question:

- **SKILL.md:** What does it do and how does it work?
- **README.md:** What’s the fastest path to first use?
- **EXAMPLES.md:** What does “good usage” look like?
- **RESEARCH.md:** Why is it designed this way?
- **CHANGELOG.md:** What changed and when?
- **TESTING-NOTES.md:** What was validated and what’s still risky?

## ALTERNATIVES CONSIDERED

### SCRIPT-ONLY VALIDATION
Fast, consistent, but cannot judge clarity and usability.

### CHECKLIST-ONLY
Flexible, but easy to apply inconsistently.

### HUMAN PEER REVIEW
High quality, but slow and hard to scale.

**Chosen approach:** A structured checklist with clear artifacts and report templates! Human-usable and repeatable.

## REFERENCES

- CommonMark specification (markdown)
- YAML 1.2 specification
- “Keep a Changelog” format
- Semantic Versioning

© 2026 STUDIO BRITTANY™
https://studiobrittany.com
