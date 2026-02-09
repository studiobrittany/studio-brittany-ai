# SKILL VALIDATOR EXAMPLES

Realistic scenarios showing how to apply the validator to a skill.

## EXAMPLE 1: SIMPLE SKILL VALIDATION

### CONTEXT
A small skill exists to generate topic ideas. It’s internally consistent but light on examples.

### WHAT YOU CHECK
- YAML parses
- Headers render
- “When to use” is clear
- Examples are at least 3–5

### COMMON RESULT
⚠️ Warning: Only 2 examples  
✅ Fix: Add 3 more examples (simple, advanced, edge case)

---

## EXAMPLE 2: YAML ROOT KEY VIOLATION

### CONTEXT
A skill includes `creator` and `version` at the root level.

### FAILURE
❌ Disallowed YAML root keys

### FIX
Move into `metadata`:

```yaml
metadata:
  creator: Example Org
  version: 1.0.0
```

---

## EXAMPLE 3: BROKEN INTERNAL LINK

### CONTEXT
README links to `#advanced-tactics` but the header is `## ADVANCED STRATEGIES`.

### FAILURE
❌ Link target does not exist

### FIX
Update the link to match the real anchor.

---

## EXAMPLE 4: VAGUE “WHEN TO USE”

### CONTEXT
Skill says “Use this for content,” but doesn’t define boundaries.

### WARNING / FAILURE
⚠️ Users won’t know when to use it  
✅ Fix: Add “When to use / When not to use” with 3–6 bullets each.

---

## EXAMPLE 5: EXAMPLES THAT AREN’T REPRODUCIBLE

### CONTEXT
Example says: “Use this to write better posts.”

### FAILURE
❌ No inputs, no outputs, no setup, not reproducible

### FIX
Provide:
- Setup (platform, audience, goal)
- Input (prompt/config)
- Expected output (sample)
- Variations (tone, length, constraints)

---

## EXAMPLE 6: MISSING REQUIRED DOCS

### CONTEXT
Repo has only `SKILL.md` and `README.md`.

### FAILURE
❌ Missing EXAMPLES.md, RESEARCH.md, CHANGELOG.md, TESTING-NOTES.md

### FIX
Create the missing files with non-placeholder content, then re-run validation.

---

## EXAMPLE 7: HEADER HIERARCHY BREAK

### CONTEXT
File jumps from `#` to `###` without a `##` section.

### WARNING
⚠️ Harder to navigate; anchor structure is messy

### FIX
Insert the missing level or re-balance headings.

---

## EXAMPLE 8: TABLE RENDERING BREAKS

### CONTEXT
A table includes pipes inside code snippets and renders incorrectly.

### WARNING / FAILURE
⚠️/❌ Table unreadable on GitHub

### FIX
- Escape pipes where needed
- Or move complex content out of tables

---

## EXAMPLE 9: PUBLIC RELEASE READABILITY CHECK

### CONTEXT
Skill references internal people, private links, or internal processes.

### FAILURE
❌ Not usable for external readers

### FIX
- Remove internal references
- Replace with generic roles (“maintainer”, “reviewer”)
- Ensure steps work with no private context

---

## EXAMPLE 10: MULTI-ISSUE CLEANUP

### CONTEXT
A skill has:
- Missing YAML version
- Broken link
- Only 2 examples
- Missing RESEARCH.md

### WORKFLOW
1. Fix YAML first
2. Fix markdown structure + links
3. Expand examples to 5+
4. Generate missing docs
5. Update CHANGELOG
6. Re-run checklist

### EXPECTED OUTCOME
✅ PASSED (or PASSED WITH WARNINGS if anything remains subjective)

© 2026 STUDIO BRITTANY™
https://studiobrittany.com 
