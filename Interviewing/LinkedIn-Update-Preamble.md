# LinkedIn Profile Audit & Optimization

## How to Use

This prompt audits your LinkedIn profile through two lenses: **recruiter search visibility** (will you show up?) and **profile conversion** (once they land on your profile, will they reach out?). It produces specific rewrites and recommendations — not generic "be more active on LinkedIn" advice.

**Before you start:**
- Copy your current LinkedIn headline, About section, and your top 3-5 experience entries (including the bullet points or descriptions you wrote for each).
- Have a target role or direction in mind. LinkedIn optimization without a target is just polishing for no one.
- If you know specific job titles that recruiters search for in your field, include those in the Context section — they're gold for headline optimization.

**Tips for best results:**
- LinkedIn's headline has a 220-character limit. The model will respect this if you leave the limit in the instructions, but double-check the output length before pasting.
- The first ~300 characters of your About section appear "above the fold" (before the "see more" link). The model is instructed to front-load value there — verify this by counting characters in the output.
- If you have a specific industry or geography you want to be found in, say so. Recruiter searches are often filtered by location and industry.

---

## Role

You are a LinkedIn optimization specialist and recruiter who has sourced candidates across technology, finance, healthcare, government, consulting, and operations. You understand how LinkedIn Recruiter search works — including keyword matching, boolean search patterns, and how headline and title fields are weighted. You also understand that a profile has to convert: a recruiter who finds you still has to be compelled to click, read, and reach out. Your recommendations balance discoverability with genuine, human-sounding copy.

---

## Context

- **Target Role(s):** [Job title or titles you want to be found for, e.g., "Data Engineer, Analytics Engineer, ML Engineer"]
- **Industry / Sector:** [e.g., fintech, defense, SaaS, public sector]
- **Career Stage:** [Early-career / Mid-career / Senior / Executive / Career-changer]
- **Geographic Preference (optional):** [e.g., "Remote US", "Vienna, Austria", "Open to relocation"]
- **Key Skills You Want to Be Found For:** [List 5-10 core skills, tools, or domains — e.g., "Python, dbt, Snowflake, data modeling, ETL pipeline design"]
- **What Makes You Different:** [1-3 sentences on your specific edge — what you bring that most people with your title don't. E.g., "I bridge the gap between data engineering and policy analysis in international organizations." This is the raw material for a compelling About section.]
- **Common Recruiter Search Titles (optional):** [If you know what recruiters in your field actually type into LinkedIn Recruiter, list them here. E.g., "site reliability engineer", "SRE", "platform engineer", "DevOps engineer"]

### Current LinkedIn Profile

<linkedin_profile>
<!--
Paste the following from your current LinkedIn:
- Headline
- About / Summary section
- Top 3-5 Experience entries (title, company, dates, and whatever description/bullets you have)
- Skills list (optional but helpful)
- Any other sections you want reviewed (e.g., Featured, Certifications, Volunteer)
-->
</linkedin_profile>

### Resume (optional)

<resume>
<!-- If you have a resume with stronger content than your LinkedIn currently reflects, paste it here. The model can pull from it when strengthening your experience entries. -->
</resume>

---

## Instructions

Using the context and current profile above, produce the following. Write all copy so it sounds like a confident professional — not a marketing brochure and not a humble apology. LinkedIn is first-person ("I build..." not "Brandon builds...").

### Section 1 — Search Visibility Assessment

Analyze how well the current profile would surface in LinkedIn Recruiter searches for the target role(s). Address:

1. **Headline keyword coverage:** Which target search terms are present in the headline? Which critical ones are missing?
2. **Title-to-target alignment:** Do the job titles in the Experience section match or closely relate to what recruiters search for? Flag any titles that are accurate but obscure (e.g., "Associate II" when recruiters search "Data Analyst").
3. **Skills section alignment:** Are the listed skills consistent with the target role? Note any high-value skills that are missing from the formal Skills list.
4. **Overall search readiness:** A brief summary of how discoverable this profile is today for the stated target.

### Section 2 — Headline Rewrite (3 options)

Provide **3 headline options**, each within LinkedIn's **220-character limit**. For each:

1. **The headline** (with character count noted).
2. **Strategy:** One sentence on the approach — e.g., "keyword-dense for maximum search hits" vs. "narrative hook that sacrifices one keyword for memorability."

At least one option should prioritize pure keyword coverage for recruiter search. At least one should prioritize a compelling human-readable hook. Label which is which.

### Section 3 — About Section Rewrite

Write a complete replacement About section (1,200-2,000 characters). Structure it as follows:

1. **First 300 characters (above the fold):** This is the only part most visitors read. Lead with a clear statement of what you do, who you do it for, and what makes you effective. No throat-clearing ("I'm a passionate professional who..."). No mission statements. Value first.
2. **Body:** Expand on your core expertise, the types of problems you solve, and 2-3 specific proof points pulled from your experience. Use concrete language over adjectives.
3. **Close:** A brief line on what you're looking for or open to — make it easy for a recruiter to know whether to reach out. Include a call to action if appropriate ("Open to conversations about X — reach out at [email/DM].").

After the rewrite, provide **3 specific notes** explaining the choices you made and what the candidate should verify or personalize before publishing.

### Section 4 — Experience Entry Rewrites (Top 3)

Rewrite the **3 most important experience entries** on the profile. For each:

1. **Title:** If the actual title is obscure or non-standard, suggest a parenthetical clarification that LinkedIn allows (e.g., "Associate Member of Technical Staff (Software Engineer)"). Never fabricate a title — clarify, don't inflate.
2. **Description rewrite:** Replace vague responsibilities with specific, results-oriented descriptions. Follow the same **Accomplished [X] by doing [Y], resulting in [Z]** pattern used in resume bullets where the experience supports it. Keep each entry to 3-5 bullet points max — LinkedIn is a skim, not a read.
3. **Keyword integration:** Note which target keywords each rewritten entry now contains that the original was missing.

### Section 5 — Profile Completeness & Quick Wins

Identify **5-7 quick, high-impact changes** beyond the headline, About, and experience sections. These might include:

1. Skills to add or reorder (LinkedIn weights the top 3 skills).
2. Featured section recommendations (what to pin and why).
3. Custom URL cleanup.
4. Profile photo and banner image guidance (not design — just what signals professionalism in the candidate's industry).
5. Recommendations strategy (who to ask and what to ask them to emphasize).
6. Creator mode or newsletter considerations if relevant to the candidate's goals.
7. Any sections to remove or deprioritize (e.g., outdated certifications, irrelevant volunteer work that dilutes the professional focus).

### Section 6 — Before / After Summary

Provide a brief **before/after comparison table** showing:

| Element | Before (Current) | After (Recommended) | Why It Matters |
|---|---|---|---|
| Headline | [current] | [recommended] | [impact on search/conversion] |
| About (first line) | [current] | [recommended] | [impact on first impression] |
| Top 3 Keywords | [present/missing] | [integrated where] | [impact on recruiter search] |

This gives the candidate a quick visual of the transformation without re-reading every section.

---

## Output Format

Use clear markdown with headers for each section. Number all items within each section. Note character counts for the headline options and the About section's above-the-fold segment. Keep the tone of all rewritten copy professional but human — it should sound like the candidate on a good day, not like a copywriter.