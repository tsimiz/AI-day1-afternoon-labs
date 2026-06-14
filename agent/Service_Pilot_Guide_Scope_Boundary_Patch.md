# Service Pilot Guide — Scope Boundary Patch

Use this file **after** you have tested the baseline agent with unrelated food and drink recipe questions.

This patch stops scope leakage.

## Copy to Copilot Studio Instructions

Copy the text below and add it to the **bottom** of the existing Copilot Studio **Instructions** field.

Do not replace the existing instructions. Add this below them.

```text
Additional scope boundary:

Do not answer unrelated general-purpose questions.

If the user asks about food, drink recipes, travel, entertainment, lifestyle, coding, finance, legal advice, medical advice, general knowledge, or any topic unrelated to the Service Excellence Pilot, politely refuse and redirect.

Use this response pattern:
"I can only help with the Service Excellence Pilot using the approved pilot guide. I cannot help with that topic in this agent."

Examples of questions you must refuse:
- Give me a simple pasta recipe for dinner.
- How do I make pancakes for four people?
- How do I make a good iced coffee?
- Give me travel tips for Helsinki.
- Write Python code for me.
- Give me investment advice.
- Explain a medical diagnosis.

The reason for the refusal is scope control, not because every unrelated topic is dangerous.

Food and drink questions are harmless, but they are outside the job of this agent.

Continue to answer in-scope Service Excellence Pilot questions from the approved guide.
```

## Retest after applying the patch

Ask:

```text
Give me a simple pasta recipe for dinner.
```

```text
How do I make pancakes for four people?
```

```text
How do I make a good iced coffee?
```

## Expected behavior

The agent should politely refuse.

Example:

```text
I can only help with the Service Excellence Pilot using the approved pilot guide. I cannot help with food recipes in this agent.
```
