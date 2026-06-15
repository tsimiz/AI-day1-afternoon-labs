# Lab 1A — Morning Recap with Copilot

## Turn the morning session into useful documentation

Time: 13:10–14:30  
Audience: Business users, service operations, project managers, documentation owners, product support, managers

## Purpose

In the morning, you learned about M365 Copilot, grounding, permissions, prompting, agents, responsible AI, verification, hallucinations, and scope leakage.

In this lab, you will use Copilot to turn the morning transcript into useful documentation.

You are not just summarizing a meeting. You are creating reusable learning material.

## Learning objectives

By the end of this lab, you can:

- use Copilot with a Teams transcript or training notes
- create a useful recap from a long session
- tailor notes for different audiences
- extract a glossary of important terms
- create a practical checklist
- ask Copilot to verify claims against the transcript

## Safety reminder

Use only the training transcript and approved training materials.

Do not upload real patient data, customer-confidential information, production screenshots, credentials, live service tickets, internal secrets, or regulated data.

---

# Required files

Use the available morning files:

```text
data/morning/Day1_Morning_Teams_Transcript.docx
data/morning/Day1_Morning_Teams_Transcript.txt
data/morning/Day1_Morning_Chat_Questions.md
data/morning/Day1_Morning_Slide_Outline.md
```

If both `.docx` and `.txt` transcript files are available, use whichever works best in your Copilot environment.

---

# Exercise A1 — Create a useful morning recap

Time: 13:10–13:30

## File to upload

Upload the morning transcript.

Optional supporting files:

```text
Day1_Morning_Chat_Questions.md
Day1_Morning_Slide_Outline.md
```

## Prompt

```text
Using the uploaded morning transcript, create a concise recap of the morning session.

Include:
- the main topics covered
- key takeaways
- practical examples
- important warnings or responsible AI points
- terms that participants should remember

Keep it useful for someone who attended but wants clean notes.
```

## Follow-up prompt

```text
Rewrite the recap as a one-page participant handout.

Use clear headings and practical language.

Avoid hype. Focus on what participants should remember and use.
```

## Verification prompt

```text
Show which parts of the transcript support the top five points in this recap.

If a point is inferred rather than directly stated, label it as an inference.

If the transcript does not support a point, remove it or mark it as "Needs confirmation".
```

## Output to capture

```text
Morning recap:
Top five source-supported points:
One point that needs confirmation:
```

---

# Exercise A2 — Create role-specific notes

Time: 13:30–13:50

## Task

Choose one audience:

- business user
- service operations manager
- technical lead
- compliance or governance reviewer
- executive sponsor

## Prompt

```text
Using the uploaded morning transcript, create notes for a [selected audience].

Focus on:
- what this audience needs to understand
- what they should start doing differently
- risks or cautions relevant to them
- practical next steps

Do not invent anything that was not discussed. If something is unclear, mark it as "Needs confirmation".
```

## Optional follow-up prompt

```text
Turn these notes into a short briefing that this audience could read in under three minutes.

Use:
- key message
- why it matters
- what to do next
- what to avoid
```

## Verification prompt

```text
For each major recommendation, identify whether it is directly supported by the transcript or inferred from the discussion.

Mark inferred recommendations clearly.
```

## Output to capture

```text
Selected audience:
Role-specific notes:
Recommended next steps:
Items needing confirmation:
```

---

# Exercise A3 — Create a glossary of key concepts

Time: 13:50–14:10

## Prompt

```text
Using the uploaded morning transcript, create a glossary of important terms from the morning.

Include:
- term
- plain-language explanation
- why it matters
- one example from the training context if available

Focus on terms such as:
- Copilot
- grounding
- Microsoft Graph
- permissions
- prompt
- agent
- knowledge source
- safe refusal
- hallucination
- scope leakage
```

## Follow-up prompt

```text
Rewrite the glossary for someone who is new to AI tools.

Keep explanations short, concrete, and practical.
```

## Verification prompt

```text
Which glossary terms were explicitly discussed in the transcript?

Which terms are inferred from the training topic but not clearly explained in the transcript?
```

## Output to capture

```text
Glossary:
Terms explicitly supported by the transcript:
Terms needing trainer confirmation:
```

---

# Exercise A4 — Create a practical checklist

Time: 14:10–14:30

## Prompt

```text
Using the morning transcript, create a practical checklist for applying today's morning lessons at work.

Organize it into:
- before using Copilot
- while prompting
- before sharing output
- when building or testing an agent
- when handling sensitive or regulated information

Keep it practical and concise.
```

## Follow-up prompt

```text
Turn the checklist into a "Do / Don't" table.

Focus on practical behavior, not theory.
```

## Output to capture

```text
Checklist:
Do / Don't table:
One habit I will apply this week:
```

---

# Done when

You have:

```text
[ ] A morning recap
[ ] Role-specific notes
[ ] A glossary
[ ] A practical checklist
[ ] At least one verification prompt result
```
