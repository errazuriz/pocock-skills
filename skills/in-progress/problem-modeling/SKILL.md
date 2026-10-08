---
name: problem-modeling
description: "Build a shared understanding of an ill-defined problem, in any domain: separate symptoms from causes and facts from assumptions, and write it down in PROBLEM.md. Use when the user isn't sure what the real problem is, describes symptoms without a clear cause, or asks to understand, unpack, or frame a problem before solving it."
---

# Problem Modeling

Actively build a shared understanding of a problem before anyone solves it. The problem need not be software: a business, a process, a team, a piece of research. Understanding is the deliverable, so write it down the moment it crystallises.

## When grilling

If you are running `grilling` alongside this skill, the nodes of the tree are **unknowns**, not decisions: what is observed, who it affects, since when, what has been tried, what would count as solved. An unknown branches into the unknowns that hang off it. Your recommended answer is your current **hypothesis**, for the user to confirm or correct.

## File structure

```
/
├── PROBLEM.md
├── GLOSSARY.md
└── decisions/
    └── 0001-slug.md
```

Create files lazily: only when you have something to write. If the directory already has a `GLOSSARY.md`, use it rather than starting a second one.

## During the session

### Separate symptoms from causes

When the user names a cause, ask what they actually observed. "You say the cause is X. Did you see X, or are you inferring it from Y?" Keep symptoms and causes in separate lists until the evidence joins them.

### Tag every claim

Each claim is an **observed fact**, a **belief**, or an **assumption**. Say which, out loud, when it isn't obvious. An assumption nobody has stated is the most dangerous thing in the tree.

### Probe the boundary

Ask what is **not** the problem. Ask what would make it worse (inversion). Ask "why?" until the answer stops being about this problem. The explicit no-s are as valuable as the yes-s.

### Cross-reference with evidence

When the user states how something is, check whether the evidence agrees: files in the directory, data, notes, sources. Finding the evidence is your job, never the user's. If you find a contradiction, surface it: "Your notes say churn started in March, but you just said it started after the price change in June. Which is right?"

### Sharpen fuzzy language

When the user uses vague or overloaded terms, propose a precise canonical term. Resolved terms go in `GLOSSARY.md` right away, using the format in [GLOSSARY-FORMAT.md](./GLOSSARY-FORMAT.md). It is a glossary and nothing else: no hypotheses, no plans.

### Update PROBLEM.md inline

Don't batch updates: when a symptom, cause, constraint or criterion is settled, write it right there. Use the format in [PROBLEM-FORMAT.md](./PROBLEM-FORMAT.md).

### Record decisions sparingly

Understanding a problem sometimes forces a decision (what is in scope, which definition of success to use). Only offer to record one in `decisions/` when it is hard to reverse, surprising without context, and the result of a real trade-off. Use the format in [DECISION-FORMAT.md](./DECISION-FORMAT.md).

## Done

The session is done when you can restate the problem in one paragraph, in the glossary's terms, and the user confirms it is exactly the problem. If they don't, the gap is the next round. Put the confirmed paragraph at the top of `PROBLEM.md`.
