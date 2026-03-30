# Prompt Library — Standard Template

> This file defines the structural anatomy that every prompt in this collection follows.
> Use it as a starting point when creating new prompts. Delete this header block in the final version.

---

## How to Use

<!-- 2-4 sentences explaining what this prompt does, when to reach for it, and any prep the user should do before running it. Keep it scannable — this is the first thing a new user reads. -->

**Before you start:**
<!-- Bullet list of anything the user should have ready (resume, job posting, etc.) -->

**Tips for best results:**
<!-- 2-3 practical tips: e.g., "Be specific in the Context fields — vague inputs produce vague outputs." -->

---

## Role

<!--
  Tell the model WHO it is. This anchors tone, vocabulary, and depth.
  Pattern: "You are a [seniority] [profession] with [relevant expertise]."
  Keep it to 2-3 sentences max. More context goes in the next section.
-->

You are a ...

---

## Context

<!--
  Structured fields the user fills in. These are the INPUTS that make the prompt
  specific to the user's situation. Use bracketed placeholders: [like this].

  Design principles:
  - Every field should change the output meaningfully. If removing a field
    wouldn't change the result, cut it.
  - Use a mix of short fills (job title, company) and longer paste-in blocks
    (resume, job description) as appropriate.
  - Label optional fields explicitly with "(optional)".
-->

- **Field A:** [placeholder]
- **Field B:** [placeholder]
- **Field C (optional):** [placeholder]

### Supporting Material

<!--
  For longer paste-in content like resumes, job descriptions, or writing samples.
  Use a clearly labeled block so the model knows what it's reading.
-->

<experience>
<!-- Paste here -->
</experience>

---

## Instructions

<!--
  Tell the model WHAT to produce. This is the task specification.

  Design principles:
  - Break the output into clearly numbered sections.
  - For each section, specify: what to generate, how many items, and what
    format each item should follow.
  - If a section requires a specific method (STAR, pros/cons, etc.), name it
    explicitly and define it briefly — don't assume the model knows your
    preferred version.
  - Use bold for section headers so they survive copy-paste into any interface.
-->

Using the context and supporting material above, produce the following:

### Section 1 — [Name] ([count])

[What to generate and how to format each item.]

### Section 2 — [Name] ([count])

[What to generate and how to format each item.]

---

## Output Format

<!--
  Global formatting instructions that apply to the entire response.
  Examples: "Use markdown with headers", "Keep total length under 2000 words",
  "Number all items sequentially within their section."

  Only include constraints that matter. Don't over-specify formatting if the
  content is what matters.
-->

Use clear markdown with headers for each section. [Add any additional formatting constraints here.]

---

## Appendix — Template Field Reference

| Field | Purpose | Example |
|---|---|---|
| Role | Anchors model persona and expertise | "Senior technical recruiter with 15 years in FAANG hiring" |
| Context | User-specific inputs that shape the output | Job title, company, seniority level |
| Supporting Material | Longer content the model needs to reference | Resume, job description, writing sample |
| Instructions | Numbered task spec with format requirements | "Generate 10 questions in STAR format" |
| Output Format | Global formatting and length constraints | "Markdown, under 2000 words" |