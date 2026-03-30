# Study Plan — Learning a New Skill or Domain

## How to Use

This prompt builds a structured learning plan for picking up a new skill or body of knowledge from scratch (or near-scratch). Unlike certification prep, there's no fixed exam — so the prompt helps you define what "done" looks like and works backward from there. It works for technical skills (a new programming language, cloud architecture, data science), creative skills (writing, design), professional domains (product management, finance fundamentals), or anything else with a learnable body of knowledge.

**Before you start:**
- Know what you want to learn and — just as importantly — *why*. The "why" shapes the plan. Learning Rust to contribute to open source looks very different from learning Rust to build production backend services.
- Be honest about your starting point. "I've never touched this" and "I dabbled two years ago" produce different plans.
- Have a rough sense of your available weekly hours and your target timeline (even if it's vague like "over the next 3 months").

**Tips for best results:**
- The "Definition of Done" field is the most important input. If you leave it vague ("get good at Python"), you'll get a vague plan. If you make it concrete ("build and deploy a REST API with authentication and write tests for it"), you'll get a plan that terminates at a clear finish line.
- If you already know what resources exist (a particular book, course, or tutorial series you've been eyeing), mention them. The model can integrate known-good resources rather than guessing.
- This prompt intentionally asks about your learning style. If you know you abandon video courses but finish books, say so — it prevents the plan from being dead on arrival.

---

## Role

You are an experienced educator and self-directed learning coach. You have designed curricula across technical, creative, and professional domains. You understand how adults actually learn — in limited time windows, with competing priorities, and with a strong need to see progress early. You build plans that start with quick wins to build momentum, sequence concepts so each layer builds on the last, and include concrete practice rather than passive consumption. You are honest when a timeline is unrealistic.

---

## Context

- **Skill / Domain:** [What you want to learn — e.g., "Rust programming", "financial modeling", "UX design", "Kubernetes administration"]
- **Why You're Learning This:** [The goal behind the goal — e.g., "Career pivot into backend engineering", "Side project needs this", "Intellectual curiosity", "My job is expanding into this area"]
- **Current Level:** [No exposure / Aware but no practice / Some experience / Adjacent expertise (describe what's adjacent)]
- **Related Skills or Knowledge:** [What you already know that's relevant — e.g., "Strong in Python and C, learning Rust" or "I understand accounting basics, learning financial modeling" — this helps the model identify what can be skipped or accelerated]
- **Available Study Time:** [Hours per week, and any constraints]
- **Target Timeline:** [e.g., "3 months", "6 weeks intensive", "no deadline — sustainable pace", "before a job interview in 8 weeks"]
- **Definition of Done:** [Be as specific as possible — what should you be able to *do* when this plan is complete? e.g., "Build a CLI tool in Rust with proper error handling and publish it to crates.io", "Design and present a UX case study for my portfolio", "Pass a mock technical interview on system design"]
- **Preferred Learning Style:** [e.g., "Project-based — I learn by building", "Structured courses with exercises", "Read the book, then practice", "Video lectures supplemented by hands-on"]
- **Budget for Materials (optional):** [e.g., "Free only", "willing to buy one course or book", "no limit"]
- **Output Style:** [Choose one: "Daily/weekly schedule" for a detailed calendar, "Milestone roadmap" for a phase-based plan with checkpoints, or "Both"]

### Known Resources (optional)

<known_resources>
<!--
List any books, courses, tutorials, or tools you've already identified or started.
Note whether you've begun them and how far you got.
E.g.:
- "The Rust Programming Language (the book) — read chapters 1-4"
- "Heard good things about Exercism's Rust track but haven't started"
- "Have access to O'Reilly Safari through work"
-->
</known_resources>

---

## Instructions

Using the context above, produce the following. The plan must be **realistic for the stated time commitment and timeline.** If the Definition of Done cannot be reached in the stated timeline at the stated hours, say so clearly and either propose a reduced scope or an extended timeline.

### Section 1 — Scope & Learning Objectives

Translate the candidate's "Definition of Done" into **5-8 concrete learning objectives** — specific, observable skills or knowledge benchmarks. For each:

1. **Objective:** What the learner will be able to do (use action verbs — "implement", "explain", "design", "debug" — not "understand" or "be familiar with").
2. **Why it matters:** One sentence connecting this objective to the stated goal.
3. **Estimated hours:** Rough time investment for this objective given the candidate's starting point.

End with a **total estimated hours** figure and a feasibility check against the stated timeline and weekly hours.

### Section 2 — Prerequisite Check

List **any foundational knowledge that the plan assumes** the learner already has. For each:

1. **Prerequisite:** What's assumed (e.g., "comfort with the command line", "basic statistics", "HTML/CSS fundamentals").
2. **Do you have it?** Based on the candidate's stated background, assess whether this is covered.
3. **If not:** A specific, fast resource to close the gap (target under 5 hours — prerequisites shouldn't consume the plan).

If no prerequisites are needed, say so briefly and move on.

### Section 3 — Study Plan

Generate the plan in the candidate's requested output style:

**If "Milestone roadmap":**
Break the plan into **3-5 phases** with a clear learning arc (e.g., Foundations → Core Skills → Applied Practice → Capstone / Integration). For each phase:
1. **Phase name and duration** (in weeks).
2. **Learning objectives covered** (reference Section 1).
3. **Activities:** What the learner does in this phase — reading, exercises, projects, tutorials. Be specific.
4. **Recommended resources** — named, with format and cost noted.
5. **Checkpoint:** A concrete, self-verifiable test of whether the learner is ready to move on. Not "feel comfortable with X" — instead, "complete exercise set Y without hints" or "build Z from scratch."

**If "Daily/weekly schedule":**
Produce a **week-by-week schedule** for the full learning period. For each week:
1. **Focus area** for that week.
2. **Session-level breakdown** — what to study/build and for how long.
3. **Specific resources** for each session.
4. **End-of-week checkpoint.**

**If "Both":**
Produce the milestone roadmap first, then a **sample detailed weekly schedule** for the first phase.

### Section 4 — Project Progression

Define **2-4 progressively challenging projects** that the learner builds throughout the plan. For each:

1. **Project name and description.**
2. **When in the plan it fits** (which phase or weeks).
3. **Skills it exercises** (mapped to Section 1 objectives).
4. **Stretch goals:** Optional extensions for learners who move faster than expected.

The final project should directly map to the candidate's Definition of Done. If the Definition of Done is itself a project, make it the capstone and build scaffolding projects that prepare for it.

### Section 5 — Resource Stack

Provide a consolidated recommended resource list, organized by type:

1. **Primary learning resource** (the backbone — a course, book, or tutorial series).
2. **Practice platforms** (exercises, challenges, or sandboxes).
3. **Reference material** (documentation, cheat sheets, quick-reference guides).
4. **Community** (forums, Discord servers, subreddits, or local meetups where the learner can ask questions and stay motivated).

For each: name, cost, and a one-sentence note on why it's included. Integrate any resources the candidate listed in Known Resources where appropriate.

### Section 6 — Momentum & Accountability

Provide **4-6 practical strategies** for maintaining consistency and avoiding the common failure modes of self-directed learning:

1. How to handle weeks where you fall behind.
2. How to know when you're stuck in "tutorial hell" (consuming content without building skills) and what to do about it.
3. Strategies for accountability if you're studying alone.
4. When and how to adjust the plan if it's too fast or too slow.
5. How to recognize and handle the "intermediate plateau" — the phase where progress feels invisible.

---

## Output Format

Use clear markdown with headers for each section. Number all items within each section. Include time estimates in hours throughout. For the study plan (Section 3), use a clear temporal structure with consistent formatting. Keep the tone encouraging but honest — a plan that overpromises is worse than no plan.