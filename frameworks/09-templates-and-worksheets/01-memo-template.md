# Memo Template — Copy & Paste Ready

Use this template for every decision. Copy, fill, archive.

---

```markdown
# [Memo title — short, distinct, searchable]

**Author:** [Name]
**Date:** [YYYY-MM-DD]
**Status:** Draft / Review / Decided / Implemented
**Read time:** [X min]
**Pre-read for meeting:** [date / "no meeting needed"]

---

## TL;DR

[2–3 sentences. The recommendation in one sentence + main reasoning.]

---

## Story so far

[Chronology of relevant events / facts in 5–8 bullets. What led here? Who was involved? Which decisions were already made?]

- [Event 1]
- [Event 2]
- [Event 3]
- [...]

---

## The Issue

**What exactly are we solving?**
[One clear question or decision in 1–2 sentences.]

**What are we not solving?**
[Optional but helpful: what's explicitly *not* in scope?]

---

## Options

### Option A: [Name]
- **What:** [Description in 2–3 sentences]
- **Pro:** [Bullets]
- **Con:** [Bullets]
- **Effort:** [Low / Medium / High]
- **Reversible?** [Yes / No / Partly]

### Option B: [Name]
- **What:** [...]
- **Pro:** [...]
- **Con:** [...]
- **Effort:** [...]
- **Reversible?** [...]

### Option C: [Name]
[...]

---

## Recommendation

[Name one option, with clear reasoning in 3–5 sentences. Why this and not the other?]

---

## Risks & accepted trade-off

**Worst case:**
[Specific. Realistic. Not sugar-coated.]

**Can we live with this?**
[Yes / No, and why.]

**Safety nets we build first:**
- [Measure 1]
- [Measure 2]

---

## Open questions

[What can't I decide / answer myself? What do I need from whom?]

- [Question 1] — addressed to [Person]
- [Question 2] — addressed to [Person]

---

## Next steps

| Step | Who | By when | Re-evaluation trigger |
|---|---|---|---|
| [Step 1] | [Name] | [Date] | [What would have to fail] |
| [Step 2] | [Name] | [Date] | [...] |

---

## Appendix

[Optional: data, diagrams, external links. Only if needed.]

---

## Reactions / Disagreements

[Comments by team. If no disagreement within 48h — silence = consent.]

---

## Lessons learned (retrospective, after implementation)

[After implementation: what did we learn? Was the recommendation right? What would we do differently?]
```

---

## Quick variants

### Quick Memo (10 min, small decision)

```markdown
# Quick: [Title]
**Author:** [Name] | **Date:** [YYYY-MM-DD]

**Recommendation:** [One sentence]
**Story so far:** [3 bullets]
**Reasoning:** [3 bullets]
**Disagree within 24h, otherwise proceed.**
```

### Decision Memo (for clear decisions)

```markdown
# Decision: [Title]
**Author:** [Name] | **Date:** [YYYY-MM-DD]

**Recommendation:** [One sentence]
**Reasoning:** [3 main reasons]
**Risk acceptance:** [What we deliberately accept]
**Implementation:** [Who, what, when]
**Disagree-and-commit deadline:** 48h
```

---

## AI workflow

**Prompt for ChatGPT / Claude:**

> *Here are my unsorted thoughts on [topic]: [content]. Structure into our memo template (TL;DR, Story so far, Issue, Options with Pro/Con, Recommendation, Risks, Open questions, Next steps). Keep it tight and concrete. If I omitted information, mark the gap explicitly.*

→ Refine the output, then archive.

---

## Where to file memos

```
your-business/Memos/
└── 2026/
    └── Q2/
        └── 2026-04-28-[short-name].md
```

→ chronological + quarter-navigable.
