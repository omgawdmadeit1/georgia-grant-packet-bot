---
name: georgia-grant-packet
description: Assemble SSI-safe Georgia grant and self-employment packets for OneGeorgia, GVRA, SBDC, DOBE, and PASS. Use when the user needs eligibility research, narrative, budget, attachment checklist, or a pre-submission compliance review. Never submit or send without an explicit human command.
license: MIT
metadata:
  version: "1.0.0"
  category: funding-grants
  income-priority: critical
---

# Georgia Grant Packet

## When to load

User asks to research, draft, edit, budget, or package a Georgia grant or disability-related self-employment application. Triggers include OneGeorgia, GVRA, SBDC, DOBE, PASS, rural development, SSI-safe self-employment, or grant packet.

## Process

### 1. Intake (do not skip)

Collect only what the packet needs, in the user's words:

- County / region in Georgia
- Entity type (sole prop, LLC, nonprofit, not formed yet)
- What the money buys (equipment, software, training, working capital)
- Low-physical constraints if relevant
- Whether SSI, SSDI, Medicaid, or a PASS is active (yes/no only — no dollar amounts)
- Deadline they already know (do not invent one)

If a fact is missing, ask. Do not fill gaps with a sample biography.

### 2. Official-source research

Fetch current pages. Preferred starting map is `references/program-map.md`.

For every program claim record:

- Program name
- Official URL fetched
- Fetch date
- Eligibility bullets copied from the page
- Deadline if the page states one, else `NOT STATED ON PAGE`
- Award range if the page states one, else `NOT STATED ON PAGE`

If fetch fails, write `HARD SOURCE FAILURE` and do not guess.

### 3. Fit score

Score 0-5 on eligibility, timeline, award usefulness, SSI/PASS safety, and submission friction. Recommend at most three programs. Say no when the fit is weak.

### 4. Draft artifacts

Write files in a folder the user names. Default `./grant-packet/<program-slug>/`.

Narrative rules:

- Truth only. No inflated revenue, jobs, or outcomes.
- SMART outcomes tied to the budget line items.
- Explicit SSI/PASS protection paragraph when benefits are active.
- Rural / disability-owned / digital self-employment framing only if the user stated those facts.

Budget rules:

- Every line has a vendor-class justification and a packet outcome.
- No personal living expenses disguised as business costs.
- Flag any line that could look like a countable resource.

### 5. Compliance gate (required before "ready")

Check all of:

- [ ] Every program fact cites a fetched official URL
- [ ] No SSN, bank, wallet, or medical record in the packet files
- [ ] SSI/PASS risk memo exists when benefits are active
- [ ] Submit channel is the official one, not a third-party form mill
- [ ] Human has not yet authorized send/submit
- [ ] Language does not promise an award

If any box fails, the packet is not ready.

### 6. Stop

Return the file list, the top risk, and the single next human action. Do not submit.

## Out of scope

Legal advice, SSA representation, medical diagnosis, guaranteed funding, auto-filing, collecting secrets.
