# End-of-Day Workshop — Agent Use Case Canvas

Time: 15:30–15:52  
Audience: All participants

## Purpose

This workshop turns the day into practical ideas.

You will work in mixed groups and identify one possible agent use case.

The use case should be small, scoped, and useful.

Avoid designing an agent that does everything.

## Group task

Discuss:

```text
Where could an agent help?
```

Pick one use case.

Then define:

1. Who is the user?
2. What problem does this solve?
3. What should the agent do?
4. What must the agent not do?
5. What knowledge source would it need?
6. What risks exist?
7. What governance or approval is needed?
8. What is the first small pilot step?

---

# Agent Use Case Canvas

Copy and fill this in:

```markdown
## Use case name

## User group

## Problem this solves

## What the agent should do

## What the agent must not do

## Knowledge sources needed

## Examples of good questions

## Examples of questions it should refuse

## Main risks

## Governance or approval needed

## Human owner

## First small pilot step
```

---

# Helpful discussion prompts

```text
What repeated questions or processes are painful enough to justify an agent?

What knowledge source would the agent need?

Who owns that knowledge source?

What should the agent refuse?

What would be the pancake question for this agent — harmless-looking, but out of scope?

What human approval point is needed?
```

---

# Example use cases

## Internal process guide agent

Helps employees find answers from approved internal process documentation.

Possible risks:

```text
Outdated documents
Unclear ownership
Overbroad answers
```

Governance needed:

```text
Named document owner
Review cycle
Approved source location
```

---

## Service-note quality assistant

Checks whether a synthetic service note contains required fields before escalation.

Possible risks:

```text
Users paste real service data
Agent overstates readiness
Missing fields are ignored
```

Governance needed:

```text
Synthetic-only training use
Clear human approval point
```

---

## Documentation navigator

Helps users find the right section across approved process guides.

Possible risks:

```text
Split documentation across systems
Obsolete files
Weak metadata
```

Governance needed:

```text
Source-of-truth decision
Lifecycle management
Content ownership
```

---

# Report-out

Each group shares:

```text
One use case
One thing the agent should refuse
One risk
One governance requirement
```

## Done when

Your group has one small, scoped agent use case and one clear refusal boundary.
