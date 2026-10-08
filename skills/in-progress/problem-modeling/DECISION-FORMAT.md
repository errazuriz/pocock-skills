# Decision Format

Decisions live in `decisions/` and use sequential numbering: `0001-slug.md`, `0002-slug.md`, etc. Create the directory lazily: only when the first decision is needed.

## Template

```md
# {Short title of the decision}

{1-3 sentences: what's the context, what did we decide, and why.}
```

That's it. The value is in recording *that* a decision was made and *why*, not in filling out sections. Add **Considered options** only when the rejected alternatives are worth remembering.

## When to offer one

All three must be true:

1. **Hard to reverse**: the cost of changing your mind later is meaningful
2. **Surprising without context**: a future reader will wonder "why did they frame it this way?"
3. **The result of a real trade-off**: there were genuine alternatives and you picked one for specific reasons

### What qualifies

- **Scope.** "We're treating churn in the enterprise tier as a separate problem."
- **The definition of success.** "Solved means retention back above 90%, not revenue recovered."
- **Which evidence counts.** "Survey answers are excluded because the sample was self-selected."
- **Deliberate deviations from the obvious framing.** Anything where a reasonable reader would assume the opposite.
