# CHANGELOG

All notable changes to this project will be documented in this file.

The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.

---

## [1.0.2] - 2026-02-09

### CHANGED
- Removed internal-only language and organization-specific voice so the validator is suitable for public GitHub distribution.
- Renamed “brand standards” checks to neutral “tone and audience fit” checks.

### ADDED
- Explicit CC BY 4.0 license line in SKILL frontmatter and README.

## [1.0.1] - 2026-02-09

### FIXED
- Moved `creator` and `version` fields under `metadata` to comply with allowed YAML root keys.

## [1.0.0] - 2026-02-09

### ADDED
- Initial release:
  - YAML frontmatter validation
  - Markdown technical validation
  - Content quality checks (triggers, steps, examples)
  - Documentation completeness requirements
  - Packaging structure guidance

---

## [UNRELEASED]

### PLANNED
- Optional automated checks (`evals/`)
- Link-check helper script
- Readability scoring (optional)

---

© 2026 STUDIO BRITTANY™
https://studiobrittany.com
