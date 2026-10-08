# GLOSSARY.md Format

## Structure

```md
# {Context Name}

{One or two sentence description of what this context is.}

## Language

**Churn**:
A paying customer who cancels within a billing period.
_Avoid_: Drop-off, attrition, lost user

**Trial user**:
Someone using the product before their first payment.
_Avoid_: Free user, lead
```

## Rules

- **Be opinionated.** When multiple words exist for the same concept, pick the best one and list the others under `_Avoid_`.
- **Keep definitions tight.** One or two sentences max. Define what it IS, not what it does.
- **Only include terms specific to this problem.** General vocabulary of the field doesn't belong, even if the conversation uses it constantly. Before adding a term, ask: is this a concept that means something particular here? Only the former belongs.
- **Group terms under subheadings** when natural clusters emerge.
- **Share it.** If the problem turns into a software build, this is the same format `domain-modeling` uses, so the build inherits the vocabulary.
