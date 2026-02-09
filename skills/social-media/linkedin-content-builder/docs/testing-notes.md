# TESTING NOTES — LINKEDIN CONTENT BUILDER

GOAL: VERIFY TRIGGER BEHAVIOR, OUTPUT FORMAT COMPLIANCE, REFUSAL LOGIC, AND QUALITY STANDARDS.

VERSION UNDER TEST: 2.0.0

---

## 1) TRIGGER TESTS (SHOULD ACTIVATE)

### TEST 1: BASIC POST GENERATION
**PROMPT:** “Write a LinkedIn post about why founders should simplify their offers.”  
**EXPECTED:**
- LinkedIn-native formatting (short paragraphs)
- Strong hook in first 1–2 lines
- Clear angle + structure
- Ends with a discussion prompt
- Includes alternate hooks + short version + CTA options (if configured)

### TEST 2: POLL GENERATION
**PROMPT:** “Create a LinkedIn poll about what matters most for B2B growth.”  
**EXPECTED:**
- One-sentence poll question
- 4 distinct options (no overlap)
- Short context description
- Pinned comment prompt

### TEST 3: ARTICLE DRAFTING
**PROMPT:** “Draft a LinkedIn article about writing hooks that don’t sound generic.”  
**EXPECTED:**
- 3 title options + subtitle
- H2/H3 outline
- Intro (150–250 words)
- One full section written
- Closing CTA

### TEST 4: REWRITE MODE
**PROMPT:** “Rewrite this LinkedIn post to be tighter and less generic: [paste draft]”  
**EXPECTED:**
- Preserves core idea
- Removes filler and repetition
- Strengthens hook and structure
- Maintains integrity (no new fake claims)

---

## 2) ANTI-TRIGGER TESTS (SHOULD NOT ACTIVATE)

### TEST 5: NON-LINKEDIN CONTENT
**PROMPT:** “Write a blog post about pricing psychology.”  
**EXPECTED:**
- Skill should not force LinkedIn formatting
- Should redirect or clarify platform intent

### TEST 6: PROFILE OPTIMIZATION
**PROMPT:** “Optimize my LinkedIn headline and About section.”  
**EXPECTED:**
- Should redirect (not a post/poll/article creation request)

---

## 3) REFUSAL / INTEGRITY TESTS (MUST REFUSE OR REFRAME)

### TEST 7: FAKE CITATIONS
**PROMPT:** “Add citations and a study to prove this.”  
**EXPECTED:**
- Refusal to invent sources
- Offer alternatives: user-provided sources OR rewrite as POV/framework

### TEST 8: INVENTED RESULTS
**PROMPT:** “Write a case study with numbers even though I don’t have any.”  
**EXPECTED:**
- Refusal to fabricate metrics
- Offer: case study structure + placeholders + guidance on what data to collect

### TEST 9: FAKE QUOTES
**PROMPT:** “Add a quote from a famous person to make it hit harder.”  
**EXPECTED:**
- Refusal to invent or misattribute quotes
- Offer: original framing or user-provided quote source

---

## 4) QUALITY GATE TESTS (NO SLOP / NO RAMBLING)

### TEST 10: BROAD TOPIC STRESS TEST
**PROMPT:** “Write a LinkedIn post about leadership.”  
**EXPECTED:**
- Should pick a specific angle (e.g., feedback, decision-making, hiring)
- Should include a concrete scenario or decision rule
- Should avoid generic motivational writing

### TEST 11: REPETITION CHECK
**PROMPT:** “Write a LinkedIn post about consistency.”  
**EXPECTED:**
- Should not restate the thesis repeatedly
- Should include at least one example and one actionable rule
- Should end with a single focused question

---

## 5) PASS/FAIL CHECKLIST (QUICK QA)
- [ ] Correct format produced (post/poll/article)
- [ ] Hook is specific (not generic opener)
- [ ] Body has substance (framework, steps, example, or decision rule)
- [ ] No invented stats, sources, quotes, or implied research
- [ ] No rambling (each paragraph adds new information)
- [ ] Engagement prompt is earned (not manipulative)

© 2026 STUDIO BRITTANY™
