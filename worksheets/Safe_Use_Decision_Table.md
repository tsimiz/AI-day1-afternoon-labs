# Safe Use Decision Table

Use this table to decide whether a Copilot use case is appropriate and what must be verified.

| Situation | Can I use Copilot? | Source material allowed | What must I verify? | What data must I not include? | Human owner or reviewer |
|---|---|---|---|---|---|
| Meeting transcript summary | Yes, with approved or synthetic content | Uploaded transcript or approved meeting record | Decisions, owners, due dates, unresolved items | Patient data, customer-confidential data, sensitive internal data | Meeting owner or project lead |
| Project status report | Yes, with approved or synthetic files | Project plan, metrics, risk register | Metrics, status, risks, decisions needed | Confidential customer data, secrets, regulated data | Project manager |
| Email action plan | Yes, with approved or synthetic email thread | Email thread or exported conversation | Confirmed actions, owners, due dates, proposals vs decisions | Sensitive personal data, confidential customer info | Sender or project owner |
| Policy question | Only with approved policy source | Approved policy excerpt or official policy document | Exact source text, missing information, policy owner | Unapproved policy interpretations | Policy owner or compliance reviewer |
| Customer-facing communication | Draft only, human review required | Approved internal source and customer-safe facts | Tone, commitments, accuracy, legal/commercial implications | Patient data, confidential internal notes, unsupported commitments | Account owner, service owner, legal/commercial owner |
| Patient-adjacent information | Be very careful; usually avoid in training | Synthetic operational examples only | Whether data is truly synthetic and allowed | Patient names, identifiers, appointment details, clinical history | Compliance, privacy, or clinical owner |
| Agent answer from process guide | Yes, if agent is scoped and grounded | Approved process guide | Whether answer is in the guide, whether refusal is appropriate | Real tickets, screenshots, credentials, patient/customer data | Agent owner or process owner |

## Personal safe-use rule

Write one rule you will apply after this training:

```text

```
