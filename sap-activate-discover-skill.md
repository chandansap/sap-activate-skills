---
name: sap-activate-discover
description: Guide for the SAP Activate DISCOVER phase — building the business case, scoping, and choosing an implementation strategy for an S/4HANA program before the project formally starts. Use when the user is in early / pre-project work: trialing the solution, estimating value, deciding Greenfield vs Brownfield, running a Digital Discovery Assessment, or writing a business case. Trigger on phrases like "business case", "should we move to S/4HANA", "trial system", "value assessment", "implementation strategy", "scoping the program".
---

# SAP Activate — Discover Phase

Discover happens before the project is funded. The goal is a defensible decision: **is this worth
doing, roughly what is the scope, and how will we do it?** Consultants add the most value here by
being honest about complexity, not by overselling a clean go-live.

## Entry criteria
- A business trigger exists (ECC end-of-maintenance, M&A, growth, cost, capability gap).
- Executive sponsor identified.

## Key activities (by workstream)
- **Solution / product experience** — get stakeholders into a trial or reference system so the
  decision is grounded in the real product, not slideware.
- **Value discovery** — quantify the value case: process KPIs, cost of the status quo, expected
  benefits, and a rough TCO. For conversions, run **SAP Readiness Check** on the ECC system to
  surface custom-code impact, simplification items, and sizing.
- **Digital Discovery Assessment (DDA)** — for cloud/RISE, capture scope, integrations, data
  volumes, and localization to shape the deal and the delivery plan.
- **Implementation strategy** — decide the deployment approach (New Implementation / System
  Conversion / Selective Data Transition), cloud vs on-prem, phasing (big-bang vs rollout), and
  a high-level timeline and team shape.

## Key deliverables (checklist)
- [ ] Business case / value case with quantified benefits and TCO
- [ ] High-level scope (in/out, geographies, processes, systems)
- [ ] Deployment approach and rationale
- [ ] SAP Readiness Check output (conversions) or DDA (cloud)
- [ ] High-level roadmap, budget range, and team model
- [ ] Documented risks and assumptions

## Exit / decision point
Discover ends when leadership approves the business case and the program is funded — the trigger
to formally initiate the project in **Prepare**.

## Common pitfalls
- Committing to a date before scope and approach are understood.
- Skipping Readiness Check on a conversion and discovering custom-code and simplification pain in
  Realize.
- A value case with no baseline KPIs, so nobody can prove value in Run.
- Confusing "we bought S/4HANA" with "we have a plan" — Discover produces the plan.

## Useful prompts for daily work
- "Draft a business-case outline for moving from ECC to S/4HANA for a mid-size manufacturer."
- "Compare Greenfield vs Brownfield for this situation and list the deciding factors."
- "Turn these Readiness Check findings into a plain-English risk summary for the steering committee."
