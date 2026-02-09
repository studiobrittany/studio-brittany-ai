---
name: skill-validator
description: Quality assurance checklist and workflow for validating skills before release. Covers YAML, markdown, examples, documentation, and packaging.
metadata:
  creator: Studio Brittany™
  version: 1.0.2  
  copyright: © 2026 Studio Brittany™
license: CC BY 4.0
---

# SKILL VALIDATOR

A systematic quality-assurance workflow for “skills” (markdown-based instruction packs) so they ship clean, usable, and reproducible.

This validator is intentionally opinionated about structure and completeness because the fastest way to make a skill unusable is to ship it with:
- Broken YAML
- Broken markdown
- Vague triggers
- Thin examples
- Missing supporting docs

## WHEN TO USE

Use this validator:
- After creating a new skill
- After editing an existing skill
- Before publishing a release
- Before sharing a skill repo publicly

Do **not** use this as a replacement for functional testing. This validates **structure, clarity, and packaging**, not runtime correctness.

## OUTPUT

A validation report with:
- ✅ PASSED checks
- ⚠️ WARNINGS (non-blocking)
- ❌ FAILURES (must fix)

Plus a complete, consistent documentation package ready for GitHub.

---

# VALIDATION CHECKLIST

## 1. YAML FRONTMATTER

### REQUIRED STRUCTURE
- [ ] File begins with `---` on line 1
- [ ] YAML ends with `---` before any markdown content
- [ ] YAML parses (valid indentation, no tabs)
- [ ] No content appears above the first `---`

### REQUIRED FIELDS
- [ ] `name` (kebab-case, no spaces)
- [ ] `description` (clear, under ~300 characters)

### RECOMMENDED FIELDS
- [ ] `metadata.creator`
- [ ] `metadata.version` (semantic versioning)
- [ ] `license` (if distributing publicly)

### ROOT KEY RULE
Only use these root keys:
- `name`, `description`, `license`, `allowed-tools`, `compatibility`, `metadata`

If you need custom fields, nest them under `metadata`.

## 2. MARKDOWN TECHNICAL QUALITY

### HEADERS & STRUCTURE
- [ ] Uses ATX headers (`#`, `##`, `###`)
- [ ] Header hierarchy is logical (no H1 → H3 skipping)
- [ ] No duplicate headings that would collide in anchors

### LINKS & CODE BLOCKS
- [ ] Code fences open/close correctly
- [ ] Code fences include language identifiers where possible
- [ ] Internal links point to real sections
- [ ] Tables render correctly (pipes handled properly)

### FORMATTING BASICS
- [ ] Lists use standard markdown (`-`, `*`, `1.`)
- [ ] Inline code uses balanced backticks
- [ ] No malformed markdown that breaks rendering

## 3. CONTENT QUALITY

### TRIGGERS
- [ ] Clear “When to use” triggers
- [ ] Clear “When NOT to use” boundaries
- [ ] Distinguishes this skill from adjacent skills/tools

### INSTRUCTIONS
- [ ] Step-by-step and actionable
- [ ] Defines technical terms on first use
- [ ] States assumptions and constraints
- [ ] Defines success criteria

### EXAMPLES
- [ ] Minimum 3–5 examples (10+ for complex/public skills)
- [ ] Examples include setup/context + input + expected output
- [ ] Includes at least 1 edge case / failure mode example
- [ ] Complexity ramps (simple → advanced)

## 4. DOCUMENTATION COMPLETENESS

A publishable skill package includes these files:

1. **SKILL.md** (the skill itself)
2. **README.md** (quick start)
3. **EXAMPLES.md** (5–10 scenarios)
4. **RESEARCH.md** (design rationale + references)
5. **CHANGELOG.md** (Keep a Changelog format)
6. **TESTING-NOTES.md** (what was checked + limitations)

Checks:
- [ ] All files exist
- [ ] Each file has real content (not placeholders)
- [ ] Troubleshooting guidance exists somewhere (README or SKILL)

## 5. TONE & AUDIENCE FIT

For public GitHub distribution, keep the language:
- Clear and direct
- Free of inside jokes, internal names, or private processes
- Helpful to a stranger with no context

Checks:
- [ ] No internal-only references (“ask X”, “send to Y”, private links)
- [ ] Avoid hype language and vague promises
- [ ] Instructions are usable by first-time readers

## 6. PACKAGING REQUIREMENTS

### REQUIRED DIRECTORY LAYOUT
```
skill-name/
├── SKILL.md
├── README.md
├── EXAMPLES.md
├── RESEARCH.md
├── CHANGELOG.md
└── TESTING-NOTES.md
```

### OPTIONAL (WHEN APPLICABLE)
- `evals/` for automated checks
- `scripts/` for helpers
- `references/` for PDFs or supporting materials

---

# VALIDATION WORKFLOW

## STEP 1: READ THE SKILL END-TO-END
- Scan YAML
- Scan headers
- Verify links and code blocks
- Identify missing sections (triggers, examples, troubleshooting)

## STEP 2: RUN THE CHECKLIST
Mark each item as ✅ / ⚠️ / ❌.

## STEP 3: FIX FAILURES FIRST
Resolve anything that would:
- Break rendering
- Confuse users
- Prevent reproducible use

## STEP 4: ADDRESS WARNINGS
Warnings aren’t blockers, but they often become bug reports later.

## STEP 5: COMPLETE THE DOCS
If anything is missing, generate it before release.

## STEP 6: UPDATE CHANGELOG
Use Keep a Changelog structure. Include dates and clear notes.

## STEP 7: PUBLISH
Create the release, tag the version, and ensure the repo root is readable for first-time visitors.

---

# VALIDATION REPORT TEMPLATE

```markdown
# VALIDATION REPORT: <SKILL NAME>

**DATE:** <YYYY-MM-DD>
**SKILL VERSION:** <X.Y.Z>
**VALIDATOR VERSION:** <X.Y.Z>

## YAML FRONTMATTER
| CHECK | STATUS | NOTES |
|------|--------|------|
| DELIMITERS PRESENT | ✅/⚠️/❌ | |
| PARSES CLEANLY | ✅/⚠️/❌ | |
| REQUIRED FIELDS PRESENT | ✅/⚠️/❌ | |
| ROOT KEYS VALID | ✅/⚠️/❌ | |

## MARKDOWN TECHNICAL QUALITY
| CHECK | STATUS | NOTES |
|------|--------|------|
| HEADER HIERARCHY | ✅/⚠️/❌ | |
| CODE FENCES | ✅/⚠️/❌ | |
| LINKS VALID | ✅/⚠️/❌ | |
| TABLES RENDER | ✅/⚠️/❌ | |

## CONTENT QUALITY
| CHECK | STATUS | NOTES |
|------|--------|------|
| TRIGGERS CLEAR | ✅/⚠️/❌ | |
| STEP-BY-STEP INSTRUCTIONS | ✅/⚠️/❌ | |
| EXAMPLES SUFFICIENT | ✅/⚠️/❌ | |

## DOCUMENTATION
| CHECK | STATUS | NOTES |
|------|--------|------|
| ALL 6 FILES PRESENT | ✅/⚠️/❌ | |
| TROUBLESHOOTING INCLUDED | ✅/⚠️/❌ | |
| CHANGELOG UPDATED | ✅/⚠️/❌ | |

## OVERALL RESULT
**RESULT:** PASSED / PASSED WITH WARNINGS / FAILED

**FAILURES TO FIX:**
- <LIST>

**WARNINGS TO CONSIDER:**
- <LIST>

**NOTES:**
- <ANYTHING IMPORTANT>
```

---

# COMMON ISSUES AND FIXES

## MISSING YAML DELIMITERS
**FIX:** Ensure the file starts with `---` on line 1 and closes YAML with `---`.

## DISALLOWED YAML ROOT KEYS
**FIX:** Move extra fields under `metadata`.

## BROKEN INTERNAL LINKS
**FIX:** Ensure the anchor matches the real header text.

## TOO-FEW EXAMPLES
**FIX:** Add examples with context + inputs + expected outputs + variations.

## VAGUE INSTRUCTIONS
**FIX:** Replace “do X” with explicit steps, including filenames/commands where relevant.

© 2026 STUDIO BRITTANY™
https://studiobrittany.com 
