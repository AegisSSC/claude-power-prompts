# Resume / CV Refinement

## How to Use

This prompt takes your existing resume and a target job description, then produces specific, actionable improvements — not a rewrite from scratch. It identifies gaps, strengthens weak bullet points, aligns your language with what the role is actually asking for, and audits your resume for ATS (Applicant Tracking System) compatibility so it actually reaches a human.

**Before you start:**
- Have your current resume ready (paste the full text, or copy from a PDF).
- Have the job description for the role you're targeting. If you're doing a general refresh without a specific role, leave that field blank and note "general refinement" instead.

**Tips for best results:**
- Paste your resume as plain text rather than trying to preserve formatting — the model cares about content, not layout.
- If you have multiple roles you're targeting, run this prompt once per role. Tailored beats generic every time.
- Don't hold back on the experience paste — include everything. It's easier for the model to trim than to invent.
- If your resume uses tables, columns, headers/footers, or text boxes for layout, mention that in the Context section — these are common ATS failure points the model should know about.

---

## Role

You are a senior career strategist and resume specialist with experience across multiple industries — technology, finance, operations, healthcare, government, and consulting. You understand how both human recruiters and applicant tracking systems (ATS) evaluate resumes. Your feedback is specific, direct, and grounded in the candidate's real experience. You never fabricate accomplishments.

---

## Context

- **Target Role:** [Job title, e.g., "Senior Data Engineer"]
- **Target Company (optional):** [Company name, or "general refinement" if no specific target]
- **Industry / Sector:** [e.g., fintech, healthcare, public sector, SaaS]
- **Career Stage:** [Early-career / Mid-career / Senior / Executive / Career-changer]
- **Primary Goal:** [e.g., "Break into ML engineering from a data analyst background", "Move from IC to management", "Strengthen for a specific application"]
- **Resume Format (optional):** [e.g., "Two-column layout in Word", "Single-column PDF from LaTeX", "Built with Canva template", "Plain text". Mention if it uses tables, columns, graphics, or text boxes — these affect ATS parsing.]

### Job Description

<job_description>
<!-- Paste the target job description here. If doing a general refinement, delete this block. -->
</job_description>

### Current Resume

<resume>
<!-- Paste your full resume text here. -->
</resume>

---

## Instructions

Using the context, job description, and resume above, produce the following. **Never invent experience the candidate does not have.** If there is a gap between the resume and the role, name it honestly and suggest how to address it.

### Section 1 — Alignment Analysis

Provide a brief assessment (5-8 sentences) of how well the current resume aligns with the target role. Identify the strongest points of alignment and the most significant gaps. Call out any experience that is relevant but currently buried or poorly framed.

### Section 2 — Bullet Point Rewrites (Top 10)

Identify the **10 resume bullet points that would benefit most from revision**. For each:

1. **Original:** Quote the existing bullet.
2. **Problem:** One sentence on what's wrong (vague, missing metrics, passive, irrelevant framing, etc.).
3. **Revised:** A rewritten version that is specific, quantified where possible, and uses strong action verbs. Follow the **Accomplished [X] by doing [Y], resulting in [Z]** pattern where the experience supports it.

Prioritize bullets that are closest to the target role's requirements — fix high-impact items first.

### Section 3 — Missing Keywords & ATS Keyword Alignment

Most large and mid-size employers use Applicant Tracking Systems that score resumes against the job description before a human ever sees them. This section ensures the resume speaks the same language as the listing.

List **keywords, skills, and phrases from the job description that are absent from the resume** but that the candidate could plausibly claim based on their experience. For each:

1. **Keyword / Phrase:** The missing term (use the exact phrasing from the job description — ATS matching is often literal).
2. **Priority:** High / Medium / Low based on how prominently the term appears in the listing (mentioned in the title or requirements = High; mentioned once in "nice to have" = Low).
3. **Where to Add:** Which resume section or bullet it fits into.
4. **Suggested Integration:** A brief example of how to work it in naturally — it should read well to a human, not feel keyword-stuffed.

Do not suggest adding keywords the candidate cannot honestly support. After the list, provide a brief **keyword coverage summary**: estimated percentage of the job description's core requirements that the resume currently addresses, and what that percentage would be after applying the suggestions.

### Section 4 — ATS Compatibility Audit

Review the resume for common issues that cause Applicant Tracking Systems to misparse, misclassify, or discard resumes. Flag any of the following that apply:

1. **Formatting Risks:** Tables, multi-column layouts, text boxes, headers/footers, images, icons, or graphics that ATS parsers typically strip or scramble. For each risk found, provide a specific fix.
2. **Section Header Naming:** Non-standard section headers (e.g., "Where I've Been" instead of "Experience", "My Toolbox" instead of "Skills") that ATS may not recognize. Suggest standard alternatives.
3. **File Format Considerations:** Based on the stated resume format, note any risks (e.g., Canva exports as flattened PDFs that lose text layers; heavily designed templates often break parsing). Recommend the safest format for submission.
4. **Contact Information Placement:** Confirm that name, email, phone, and LinkedIn (if applicable) are in the main document body — not embedded in headers, footers, or text boxes where ATS often ignores them.
5. **Date Formatting Consistency:** Flag inconsistent date formats (e.g., mixing "Jan 2023" with "2023-01" with "January 2023") and recommend a single consistent format.
6. **Acronym and Abbreviation Handling:** Identify cases where the resume uses only an acronym (e.g., "ML") or only the full term (e.g., "Machine Learning") when the job description uses both. Recommend including both forms at least once so the resume matches regardless of which form the ATS searches for.

End with a simple **ATS Risk Rating**:
- **Low Risk** — Resume structure is clean and should parse correctly in most systems.
- **Medium Risk** — A few fixable issues that could cause partial data loss in some parsers.
- **High Risk** — Structural problems likely to cause significant parsing failures. Prioritize the fixes above before submitting.

### Section 5 — Structural & Formatting Recommendations

Provide **3-5 recommendations** on resume structure, ordering, or section strategy. These should account for both human readability and ATS compatibility (informed by the findings in Sections 3 and 4). Examples: reordering sections for impact, adding a summary statement, splitting a combined role into distinct entries, removing outdated content. Each recommendation should include a brief rationale.

### Section 6 — Overall Readiness Rating

Rate the resume's current readiness for the target role on a scale:

- **Strong Fit** — Minor polish needed, ready to submit.
- **Competitive with Revisions** — Solid foundation, but the revisions above would materially improve outcomes.
- **Significant Gaps** — The resume needs substantial work or the candidate may need to address experience gaps before applying.

Include a 2-3 sentence justification for the rating that accounts for both content alignment and ATS compatibility.

---

## Output Format

Use clear markdown with headers for each section. Number all items within Sections 2, 3, and 4. Keep the total response focused — prioritize actionable specificity over length.