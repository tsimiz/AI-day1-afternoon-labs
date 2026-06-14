# Lab 2A — Quality, Trust, and Verification

Time: 14:45–15:30  
Audience: Business users

## Purpose

This lab focuses on quality and trust.

You will practice checking Copilot outputs, improving prompts, and accepting that “not specified” can be the correct answer.

## Learning objectives

By the end of this lab, you can:

- identify unsupported claims
- ask Copilot to show evidence
- reduce hallucination risk through prompt design
- create a safe-use decision table
- decide what should not be uploaded or automated

---

# Exercise A2.1 — “Not specified” is a good answer

Time: 14:50–15:05

## File to upload

```text
07_Service_Excellence_Pilot_Data_Handling_Policy_Excerpt.docx
```

## First prompt

```text
According to the uploaded Service Excellence Pilot policy excerpt, what is the required retention period for pilot escalation notes? Answer briefly.
```

## Verification prompt

```text
Show the exact source text that supports that retention period.

If no source text exists, say that the policy excerpt does not specify it.
```

## Improved prompt

```text
Using only the uploaded policy excerpt, answer this question:

What is the required retention period for pilot escalation notes?

If the uploaded excerpt does not explicitly specify the retention period, say:
"Not specified in the uploaded excerpt."

Do not infer or guess.
```

## Expected answer

```text
Not specified in the uploaded excerpt.
```

## Reflection

Answer:

```text
Did Copilot guess?
Did the verification prompt change the answer?
What wording helped prevent guessing?
```

---

# Exercise A2.2 — Safe-use decision table

Time: 15:05–15:20

## Prompt

```text
Create a safe-use decision table for using Copilot in this training context.

Columns:
- Situation
- Can I use Copilot?
- Source material allowed
- What must I verify?
- What data must I not include?
- Human owner or reviewer

Include rows for:
- meeting transcript summary
- project status report
- email action plan
- policy question
- customer-facing communication
- patient-adjacent information
- agent answer from process guide
```

## Validation

Check that the table says:

```text
[ ] Customer-facing communication requires human review
[ ] Patient-adjacent information has strong restrictions
[ ] Policy questions require source evidence
[ ] Agent answers should be checked against the approved guide
[ ] The table is practical enough to reuse
```

---

# Exercise A2.3 — Rewrite one weak prompt

Time: 15:20–15:30

## Weak prompt

```text
Summarize this and tell me what to do.
```

## Rewrite it using

```text
Goal:
Context:
Source:
Format:
Verification:
```

## Example improved prompt

```text
Using only the uploaded email thread, create an action tracker for the Service Excellence Pilot.

Context:
This is for a project manager preparing a follow-up message.

Format:
Use a table with Action, Owner, Due date, Evidence, and Confidence.

Verification:
Mark anything unclear as Needs confirmation. Do not invent missing owners or dates.
```

## Done when

You have:

- one safer prompt
- one verification habit
- one safe-use decision table
