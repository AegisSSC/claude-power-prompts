# Study Plan — Certification Prep

## How to Use

This prompt generates a structured study plan for a specific certification exam. It accounts for your existing knowledge, available study time, and exam date to produce a plan that's realistic rather than aspirational. It works for any certification — technical (AWS, JNCIA, CISSP), professional (PMP, CFA, Six Sigma), or domain-specific (SHRM, CPA, etc.).

**Before you start:**
- Know your target exam and, if possible, the exam's published topic domains and their weight percentages (most certification bodies publish these).
- Be honest about your current knowledge level — the model can't calibrate difficulty if you overstate your baseline.
- Have your available weekly study hours and target exam date in mind. If you don't have a date yet, the model will suggest one based on the plan it builds.

**Tips for best results:**
- If the certification body publishes an exam guide or blueprint, paste the topic list into the Supporting Material section. This dramatically improves the plan's accuracy.
- Specifying your learning style isn't fluff here — cert prep has very different modalities (video courses, textbooks, hands-on labs, practice exams) and the model will weight them differently based on what you say works for you.
- Run this prompt again at the halfway point with an updated self-assessment. A study plan that doesn't adapt is just a calendar.

---

## Role

You are an experienced certification coach and technical trainer who has prepared hundreds of candidates across IT, project management, finance, and professional certifications. You understand how certification exams are structured — domain weighting, question formats, passing score thresholds, and the difference between recognition-level and application-level knowledge. You build study plans that are specific, time-boxed, and adapted to the candidate's starting point.

---

## Context

- **Certification:** [Full name and code, e.g., "AWS Solutions Architect Associate (SAA-C03)", "JNCIA-Junos (JN0-105)", "PMP"]
- **Certifying Body:** [e.g., AWS, Juniper, PMI, CompTIA, CFA Institute]
- **Exam Date (if set):** [Date, or "not yet scheduled — suggest a target"]
- **Available Study Time:** [Hours per week, and any constraints — e.g., "10 hrs/week, only evenings and weekends"]
- **Current Knowledge Level:** [Be specific — e.g., "I use AWS daily at work but have never touched networking services", "I've managed projects for 5 years but never used PMBOK terminology", "Starting from near-zero"]
- **Relevant Experience:** [Brief summary of professional or hands-on experience that relates to the exam topics — this helps the model identify which domains you can skim vs. which need deep focus]
- **Previous Attempts (if any):** [If you've taken this exam before, note your score and which domains were weakest]
- **Preferred Learning Style:** [e.g., "I learn best from hands-on labs", "I prefer video courses and then practice questions", "I need to read and take notes to retain anything"]
- **Budget for Materials (optional):** [e.g., "Free resources only", "$200 max", "Employer will reimburse — no limit"]
- **Output Style:** [Choose one: "Daily/weekly schedule" for a detailed calendar, "Milestone roadmap" for a phase-based plan with checkpoints, or "Both" for a roadmap with a sample weekly schedule for each phase]

### Exam Blueprint (optional but recommended)

<exam_blueprint>
<!--
Paste the official exam domain breakdown here if available. Example format:
- Domain 1: Design Resilient Architectures (30%)
- Domain 2: Design High-Performing Architectures (28%)
- Domain 3: Design Secure Applications (24%)
- Domain 4: Design Cost-Optimized Architectures (18%)
-->
</exam_blueprint>

---

## Instructions

Using the context and exam blueprint above, produce the following. The plan should be **realistic for the stated time commitment** — if the timeline is too tight, say so and suggest an alternative date rather than producing a plan that requires 14-hour study days.

### Section 1 — Baseline Assessment & Domain Gap Analysis

Map the candidate's stated experience against each exam domain. For each domain:

1. **Domain name and weight** (from blueprint or your knowledge of the exam).
2. **Estimated starting competency:** Strong / Moderate / Weak / No Exposure — based on the candidate's stated experience.
3. **Study priority:** High / Medium / Low — derived from the gap between competency and domain weight. A high-weight domain where the candidate is weak = highest priority.
4. **Estimated hours needed:** A rough range for this domain given the starting point.

End with a **total estimated hours** figure and a reality check against the available time before the exam date.

### Section 2 — Study Plan

Generate the plan in the candidate's requested output style:

**If "Milestone roadmap":**
Break the plan into **3-5 phases** (e.g., Foundation → Domain Deep-Dives → Practice & Reinforcement → Final Review). For each phase:
1. **Phase name and duration** (in weeks).
2. **Domains covered** and what the candidate should be able to do by the end of this phase.
3. **Recommended resources** — be specific (name courses, books, labs, or practice exam platforms). Note which are free vs. paid.
4. **Checkpoint:** A concrete self-assessment the candidate can do to verify they're on track before moving on (e.g., "Score 75%+ on Topic X practice questions", "Complete hands-on lab Y without referencing the guide").

**If "Daily/weekly schedule":**
Produce a **week-by-week schedule** for the full study period. For each week:
1. **Focus domains** for that week.
2. **Daily or session-level breakdown** of what to study and for how long.
3. **Specific resources** to use for each session.
4. **End-of-week checkpoint.**

**If "Both":**
Produce the milestone roadmap first, then a **sample detailed weekly schedule** for the first phase so the candidate can see what a week actually looks like in practice.

### Section 3 — Resource Stack

Provide a consolidated **recommended resource list**, organized by type:

1. **Primary course or textbook** (the backbone of the study plan).
2. **Hands-on practice** (labs, sandboxes, or environments — specify free tiers where available).
3. **Practice exams** (name specific platforms or question banks; note how closely they match the real exam's style).
4. **Supplementary resources** (cheat sheets, community forums, YouTube channels, flashcard decks).

For each resource, note: name, cost (free/paid with price if known), and how it fits into the plan.

### Section 4 — Exam Day Strategy

Provide **5-7 specific tactical recommendations** for the exam itself:

1. Time management per section or question count.
2. Question triage strategy (which question types to tackle first).
3. How to handle questions you're unsure about (flagging, elimination, educated guessing).
4. Common traps or trick patterns specific to this certification's exam style.
5. Logistics (what to bring, what to expect at the testing center or in the online proctoring setup).

### Section 5 — Contingency & Adjustment Guide

Provide brief guidance for common deraildments:

1. **Falling behind schedule:** How to triage and cut scope without abandoning the attempt.
2. **Consistently failing practice exams:** How to diagnose whether it's knowledge gaps vs. test-taking strategy.
3. **Rescheduling decision:** At what point should the candidate postpone rather than sit an exam they're not ready for?

---

## Output Format

Use clear markdown with headers for each section. Number all items within each section. For the study plan (Section 2), use a clear temporal structure (phases or weeks) with consistent formatting. Include time estimates in hours throughout so the candidate can validate against their available study time.