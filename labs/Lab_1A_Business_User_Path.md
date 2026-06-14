# Lab 1A — Business User Path

## From demo pattern to useful work output

Time: 13:10–14:30  
Audience: Business users, service operations, project managers, documentation owners, product support, managers

## Purpose

In the morning demos, you saw how Copilot can summarize, structure, and verify information.

In this lab, you will apply the same pattern, but you will not simply repeat the demos. You will choose an audience, choose an output, and verify the result.

## Learning objectives

By the end of this lab, you can:

- upload local synthetic files into Copilot
- use the Goal, Context, Source, Format, Verification pattern
- create role-specific work outputs
- ask Copilot to show evidence
- identify where human judgment is still required

## Safety reminder

Use only the synthetic files provided.

Do not upload real patient data, customer-confidential information, production screenshots, credentials, live service tickets, internal secrets, or regulated data.

---

# Exercise A1 — Same meeting, different audience

Time: 13:10–13:30

## File to upload

```text
01_Service_Excellence_Pilot_Meeting_Transcript.docx
```

## Task

Choose one audience:

- senior stakeholder
- service operations manager
- quality/compliance reviewer
- documentation owner

Create a summary for that audience.

## Prompt option — Service operations manager

```text
Using the uploaded meeting transcript, create a summary for a service operations manager.

Focus on:
- decisions that affect service operations
- actions owned by service operations
- risks related to triage and handover
- unresolved questions that could block the pilot

Keep it under 250 words.
```

## Prompt option — Quality/compliance reviewer

```text
Using the uploaded meeting transcript, create a summary for a quality/compliance reviewer.

Focus on:
- data-handling risks
- guardrails
- unsafe uses that were ruled out
- unresolved governance decisions
- items that need evidence or review

Use concise bullet points.
```

## Prompt option — Documentation owner

```text
Using the uploaded meeting transcript, create a summary for the documentation owner.

Focus on:
- what documentation must be created
- what sections the guide should include
- open questions about source of truth
- actions and due dates related to documentation

Create a practical task list.
```

## Verification prompt

```text
Show which parts of the transcript support the top three points in your summary.

If any point is an inference, label it as an inference.
```

## Output to capture

```text
Audience:
Summary:
Top three source-supported points:
One item needing confirmation:
```

---

# Exercise A2 — Build the artifact the stakeholder needs

Time: 13:30–13:55

## Files to upload

```text
02_Service_Excellence_Pilot_Pilot_Plan.docx
03_Service_Excellence_Pilot_Service_Metrics.xlsx
04_Service_Excellence_Pilot_Risks_and_Dependencies.docx
```

## Task

Choose one output:

- steering committee status report
- quality/compliance risk brief
- project manager action dashboard
- service operations update email

## Prompt option — Steering committee status report

```text
Using the uploaded files, create a steering committee status report for the Service Excellence Pilot.

Include:
- overall status
- progress
- key metrics
- top risks
- decisions needed
- next steps

Use a calm, professional tone.

Do not invent dates or metrics. Mark missing information clearly.
```

## Prompt option — Quality/compliance risk brief

```text
Using the uploaded files, create a quality and compliance risk brief.

Focus on:
- data-handling risks
- governance gaps
- agent or Copilot misuse risks
- decisions that require human approval
- recommended controls

Use a table with Risk, Evidence, Impact, Mitigation, and Owner.
```

## Prompt option — Project manager action dashboard

```text
Using the uploaded files, create a project manager action dashboard.

Include:
- action
- owner
- due date
- dependency
- status
- risk if delayed

Use a table.
Do not invent missing owners or dates.
```

## Prompt option — Service operations update email

```text
Using the uploaded files, draft a short internal update email for service operations.

The email should explain:
- what the pilot is about
- what changes for service operations
- what risks or open questions remain
- what people should do next

Keep it practical and under 300 words.
```

## Verification prompt

```text
Add a Source Notes section.

For each major claim, say which uploaded file supports it.

If the claim is inferred from multiple files, label it as an inference.
```

## Output to capture

```text
Chosen artifact:
Draft output:
Source notes:
One gap requiring confirmation:
```

---

# Exercise A3 — Email thread to communication package

Time: 13:55–14:15

## File to upload

```text
05_Service_Excellence_Pilot_Email_Thread.docx
```

## Task

Create two outputs:

1. internal action tracker
2. reply email confirming decisions and asking for clarification

## Prompt 1 — Action tracker

```text
Using the uploaded email thread, create an internal action tracker.

Include:
- confirmed action
- owner
- due date
- evidence from the thread
- confidence level
- open dependency

Do not assign ownership if the thread is unclear.
```

## Prompt 2 — Reply email

```text
Draft a short reply email that confirms the agreed action plan.

The reply should:
- confirm completed or agreed actions
- politely ask for clarification on unresolved items
- avoid overclaiming certainty
- sound professional but not robotic
```

## Prompt 3 — Improve tone

```text
Make the reply email slightly warmer and more human, but keep it concise.

Do not add new facts.
```

## Verification prompt

```text
Which email confirms Sofia completed the required-fields action?

Which item still needs confirmation?
```

## Output to capture

```text
Action tracker:
Reply email:
One verified action:
One unresolved item:
```

---

# Exercise A4 — Apply the pattern to your own safe work scenario

Time: 14:15–14:30

Do not upload real work content.

Fill this out:

```text
A real work situation where Copilot could help me:
Source material I would use:
Output I would ask for:
What I must verify:
What data I must not upload:
Who owns the final decision:
```

## Optional prompt

```text
Help me design a safe Copilot prompt for this situation.

Situation:
[describe the situation without sensitive data]

Source material:
[describe the type of source]

Desired output:
[describe the output]

Constraints:
- do not invent facts
- mark uncertainty
- include source notes
- keep the output business-readable
```

## Done when

You have:

- one useful work artifact
- one verification habit
- one safe prompt idea for your own work
