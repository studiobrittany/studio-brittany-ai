# SKILL VALIDATOR

A quality-assurance workflow for markdown “skills” so they’re clean, readable, and publishable.

## WHAT THIS IS

This repository provides a structured validation checklist and workflow that helps you ship skills that:
- Render correctly
- Explain themselves clearly
- Include enough examples to be reproducible
- Include complete supporting docs

## QUICK START

1. Open `SKILL.md`
2. Run through **VALIDATION CHECKLIST**
3. Fill out the **VALIDATION REPORT TEMPLATE**
4. Fix ❌ failures, then re-check
5. Confirm all required files exist:
   - `SKILL.md`
   - `README.md`
   - `EXAMPLES.md`
   - `RESEARCH.md`
   - `CHANGELOG.md`
   - `TESTING-NOTES.md`

## WHAT IT CHECKS

- YAML frontmatter correctness
- Markdown technical quality (headers, links, code fences)
- Content clarity (triggers, step-by-step instructions)
- Example coverage and reproducibility
- Documentation completeness
- Packaging readiness for GitHub

## WHAT IT DOES NOT CHECK

This does **not** execute code or verify runtime behavior. For that, add:
- `evals/` (automated checks)
- manual test scripts
- real-world dry runs

## REPOSITORY CONTENTS

- `SKILL.md` — the validator itself
- `EXAMPLES.md` — scenarios showing how validation works
- `RESEARCH.md` — methodology and design rationale
- `CHANGELOG.md` — version history
- `TESTING-NOTES.md` — what was tested and known limitations

## LICENSE

This repository is licensed under **CC BY 4.0**. Attribution is required.

---

© 2026 STUDIO BRITTANY™
https://studiobrittany.com
