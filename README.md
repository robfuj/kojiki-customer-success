# 06 — Customer Success

> Part of the **Kojiki Decision System**. This repo is the
> **Customer Success** line. It references the shared ontology in
> [`00-kojiki-ontology`](https://github.com/robfuj/kojiki-ontology) for the
> canonical schemas, taxonomy, decision-rights, and handoff standards.

## Primary question
> How do we retain and expand customer value?

## Purpose
Ensure customers realize expected value, remain successful, and identify expansion opportunities.

## Sub-functions
Onboarding, Customer Success, Account Management, Support, Implementation, Professional Services, Customer Experience, Voice of Customer

## Typical roles
Chief Customer Officer, VP Customer Success, Customer Success Director, Customer Success Manager, Account Manager, Support Director, Implementation Manager, CX Manager

## Inputs
Purchase motivation, usage, engagement, stakeholder changes, support history, commercial health.

## Outputs
Customer health, interventions, renewals, expansions, feedback, advocacy.

## Learning focus
Churn signals; retention drivers; adoption patterns; expansion signals; recovery strategies.

## Operating tree
```text
CUSTOMER ONBOARDING →
    EXPECTED VALUE →
    ACTUAL VALUE →
    HEALTH →
    RISK DETECTION →
    DIAGNOSIS →
    INTERVENTION →
    CUSTOMER RESPONSE →
    RECOVERY / EXPANSION / CHURN →
    LEARNING
```

## Decision states
```text
ONBOARDING → ACTIVE → HEALTHY → WATCH → AT-RISK → INTERVENTION → RECOVERING → EXPANDED → CHURNED
```

## Decision outputs
`Maintain · Intervene · Recover · Expand · Escalate · Churn`

## Critical prompts (what this function thinks about)
> Why did the customer buy?
> What outcome did they expect?
> Are they receiving that outcome?
> What has changed?
> What behavior indicates health?
> What behavior indicates risk?
> Who is the champion?
> Who is disengaging?
> What is the customer's current priority?
> What problem are they actually experiencing?
> Is this a product problem?
> Service problem?
> Expectation problem?
> Relationship problem?
> Customer-side problem?
> What intervention has the highest probability of recovery?
> What evidence proves recovery?
> Is there an expansion opportunity?
> What predicts future churn?

## Canonical record schema (docx Learning Ledger + Decision Object Fields)
Every decision in this line is recorded as:
- a **Decision Object** (docx S9) — see `schema/decision-object.json`
- a **Learning Ledger** entry (docx S7) — see `schema/learning-ledger.json`

and the agent must run the **Orientation Protocol** first (see `AGENT.md`).

## How to use
1. Read `AGENT.md` — the first-run Orientation Protocol.
2. Read `SCHEMA.md` — how this line maps to the universal schema.
3. Read `data/06-customer-success.json` — the machine-readable spec.
4. See `data/example.json` — one fully worked decision (Decision Object + Ledger).
5. Use `decision-graph.mmd` — agent-decodable operating tree + state model.
6. Validate new records: `python3 tools/validate.py data/<name>.json`
