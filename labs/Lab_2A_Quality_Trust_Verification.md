# Lab 2A — Quality, Trust, Verification, and Safe Use

Time: 14:45–15:30  
Audience: Business users

## Purpose

This lab focuses on how to decide whether an AI-generated answer is trustworthy enough to use.

In Lab 1A, you used Copilot to create useful outputs from the morning transcript.

In this lab, you will slow down and check the quality of those outputs.

The goal is not just to get a good-looking answer.

The goal is to learn how to verify, challenge, and safely use AI-generated content.

## Learning objectives

By the end of this lab, you can:

- identify unsupported claims in an AI-generated answer
- ask Copilot to show evidence from a source
- separate facts, inferences, and guesses
- improve prompts to reduce hallucination risk
- decide when human review is required
- define safe-use rules for transcripts, summaries, and agents

---

# Required files

Use the morning materials:

```text
data/morning/Day1_Morning_Teams_Transcript.docx
data/morning/Day1_Morning_Teams_Transcript.txt
data/morning/Day1_Morning_Chat_Questions.md
data/morning/Day1_Morning_Slide_Outline.md
```

Use whichever transcript format works best in your Copilot environment.

The slide outline and chat questions are optional supporting files.

---

# Safety reminder

Do not upload:

- real patient data
- real customer-confidential information
- production screenshots
- credentials or secrets
- live support tickets
- internal regulated data

If the transcript contains sensitive or irrelevant content, do not use that section. Ask the trainer for the cleaned version.

---

# Exercise A2.1 — Trust check: good-looking does not mean correct

Time: 14:45–15:00

## Goal

Create an AI-generated answer, then check whether it is actually supported by the morning materials.

## Step 1 — Ask for a confident summary

Prompt:

```text
Using the uploaded morning transcript, create a confident summary of the most important lessons from the morning session.

Include:
- what participants should remember
- what they should start doing differently
- risks they should avoid
- any policy or governance points mentioned
- any follow-up actions that seem important

Make it clear and practical.
```

## Step 2 — Verify the answer

Now challenge the output.

Prompt:

```text
Review your previous answer against the uploaded morning transcript.

Create a table with these columns:
- Claim
- Supported by transcript?
- Evidence from transcript
- Inference or direct statement?
- Keep, revise, or remove

If a claim is not supported by the transcript, mark it as "Unsupported".
If a claim is only inferred, mark it as "Inference".
```

## Step 3 — Clean up the output

Prompt:

```text
Rewrite the summary using only claims that are directly supported by the transcript.

Keep useful inferred points only if they are clearly labeled as "Inference".

Remove unsupported claims.
```

## Output to capture

```text
One claim that was directly supported:

One claim that was only inferred:

One claim that was unsupported or needed removal:

One wording change that made the output more trustworthy:
```

---

# Exercise A2.2 — Evidence, uncertainty, and “not found”

Time: 15:00–15:15

## Goal

Practice asking Copilot to say what it knows, what it does not know, and what needs human confirmation.

## Step 1 — Ask questions that may not be fully answered

Use these prompts one by one.

```text
Using only the uploaded morning transcript, what is our official company policy for using Copilot with customer data?
```

```text
Using only the uploaded morning transcript, what licenses are required for every Copilot feature discussed this morning?
```

```text
Using only the uploaded morning transcript, what is the official retention period for the Teams transcript?
```

```text
Using only the uploaded morning transcript, what are the approved production use cases for Copilot Studio agents at Topcon?
```

## Expected behavior

A trustworthy answer may be:

```text
I cannot find that in the uploaded morning transcript.
```

or:

```text
The transcript discusses the topic generally, but it does not specify the official policy, license requirement, retention period, or approved production use case.
```

## Step 2 — Improve the prompt

Use this stronger verification prompt:

```text
Using only the uploaded morning transcript, answer the question below.

Question:
[insert question]

Rules:
- If the answer is explicitly stated, answer it and quote or summarize the supporting part.
- If the answer is discussed only generally, say "Discussed generally, but not specified."
- If the answer is not in the transcript, say "Not found in the transcript."
- Do not infer official policy, licensing, legal, compliance, retention, or production approval details.
```

## Step 3 — Classify the answers

Fill this in:

```text
Question:
Answer quality:
[ ] Directly supported
[ ] Discussed generally, but not specified
[ ] Inferred
[ ] Unsupported
[ ] Needs human owner

Who should confirm this?
```

## Output to capture

```text
One example of "not found" being the correct answer:

One topic that needs an official owner:

One prompt rule that reduced guessing:
```

---

# Exercise A2.3 — Safe-use decision table

Time: 15:15–15:25

## Goal

Create a practical decision table for when it is safe to use Copilot or an agent with training transcripts and similar work content.

## Prompt

```text
Create a safe-use decision table for using Copilot or an agent with training transcripts and meeting materials.

Columns:
- Situation
- Can I use Copilot or an agent?
- Source material allowed
- What must I verify?
- What data must I not include?
- Human owner or reviewer

Include rows for:
- summarizing a training transcript
- creating a participant handout
- creating a glossary
- creating a responsible AI checklist
- asking about company policy
- asking about licensing
- asking about customer data
- asking about patient or clinical information
- creating a recap agent from a transcript
- sharing AI-generated output with a team
```

## Improve the table

Prompt:

```text
Review the table and make it more practical.

Make sure it clearly states:
- when human review is required
- when official documentation is needed
- when the answer should say "not found"
- what sensitive data must not be uploaded
- who owns the final decision
```

## Output to capture

```text
Three situations where Copilot is useful:

Three situations where human review is required:

Three types of data that must not be uploaded:

One safe-use rule I would share with my team:
```

---

# Exercise A2.4 — Rewrite a risky prompt

Time: 15:25–15:30

## Goal

Improve a weak or risky prompt so that it asks for evidence, handles uncertainty, and avoids unsupported conclusions.

## Weak prompt

```text
Summarize the transcript and tell me what we should do.
```

## Why this is risky

This prompt is too broad.

It does not say:

- who the output is for
- what source to use
- what format is needed
- whether to separate facts from inferences
- what to do if information is missing
- what requires human review

## Rewrite the prompt

Use this structure:

```text
Goal:
Audience:
Source:
Format:
Verification:
Boundaries:
Human review:
```

## Example improved prompt

```text
Using only the uploaded morning transcript, create a practical recap for participants who attended the session.

Audience:
Business and technical participants from the training.

Format:
Use headings and bullet points. Include key takeaways, responsible AI reminders, and follow-up questions.

Verification:
For the top five takeaways, say whether each is directly supported by the transcript or inferred from the discussion.

Boundaries:
Do not invent company policy, licensing details, legal advice, clinical guidance, or production approval decisions.

Human review:
Mark anything that should be confirmed by the trainer, compliance owner, licensing owner, or another human owner.
```

## Output to capture

```text
My improved prompt:

One boundary I added:

One verification rule I added:

One topic that requires human review:
```

---

# Done when

You have:

```text
[ ] Verified at least one AI-generated summary against the transcript
[ ] Identified a supported claim, an inference, and an unsupported claim
[ ] Practiced "not found" as a valid answer
[ ] Created or improved a safe-use decision table
[ ] Rewritten a risky prompt into a safer prompt
[ ] Identified when human review is required
```

---

# Key takeaway

Trustworthy AI use is not about accepting the most fluent answer.

It is about asking:

```text
What is this answer grounded in?
What is directly supported?
What is inferred?
What is missing?
What requires human review?
What should not be uploaded or automated?
```
