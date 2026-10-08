# PROBLEM.md Format

## Template

```md
# {Short name of the problem}

{The one-paragraph problem statement the user confirmed, in the glossary's terms. Leave a placeholder until it is confirmed.}

## Who it affects

{Who feels it, and how.}

## Symptoms

- {Something observed.} _(observed: {where or by whom})_

## Causes

- {A candidate cause.} _(hypothesis, {low | medium | high} confidence: {why})_

## Not the problem

- {Something explicitly out of scope, and why.}

## Constraints

- {A limit any solution must respect.}

## Solved looks like

{What would have to be true for the user to call this solved.}

## Open questions

- {An unknown still on the frontier.}
```

## Rules

- **Keep symptoms and causes apart.** A cause moves out of hypothesis only when the evidence supports it; say what the evidence is.
- **Tag confidence honestly.** A cause the user is sure of but nobody has checked is still a hypothesis.
- **Drop empty sections.** A section with nothing settled yet is noise, except `Open questions`.
- **No solutions.** `PROBLEM.md` describes the problem. Solutions belong to whatever comes next.
