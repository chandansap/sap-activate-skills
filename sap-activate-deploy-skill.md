---
name: sap-activate-deploy
description: Guide for the SAP Activate DEPLOY phase — final go-live preparation, cutover execution, production data migration, end-user training delivery, hypercare setup, and transition to operations for an S/4HANA program. Use when the user is planning or running cutover, doing a dress rehearsal, executing production data load, preparing go-live readiness/sign-off, delivering training, or standing up hypercare and support handover. Trigger on "cutover", "go-live", "dress rehearsal", "production migration", "hypercare", "go/no-go", "transition to operations", "deploy readiness".
---

# SAP Activate — Deploy Phase

Deploy moves the tested solution into production and hands it to the business and support. It is
mostly logistics and nerve: a well-run cutover is boring because everything was rehearsed. The test
of success: **production is live, data is validated, users are trained, and hypercare is catching
issues before they hurt.**

## Entry criteria
- Realize gate passed: build complete, SIT/UAT passed, data migration validated in test, cutover
  plan approved.

## Key activities (by workstream)
- **Transition / Cutover** — finalize and execute the cutover plan: a minute-by-minute runbook with
  owners, dependencies, timings, and rollback points. Run at least one full **dress rehearsal**
  against production-like conditions before the real event.
- **Data Management** — execute the **production data migration** and reconcile against source;
  formal data sign-off gates the go-live.
- **Go-live readiness & go/no-go** — run the readiness assessment and a documented go/no-go decision
  with clear criteria and named decision-makers.
- **OCM & Enablement** — deliver end-user training and ensure comms, floor-walkers, and quick
  reference guides are in place for day one.
- **Operations** — stand up **hypercare**: elevated support, a triage process, daily standups, and a
  fast path from issue to fix. Complete the **transition-to-operations** handover to the run/support
  team (runbooks, monitoring, known issues).

## Key deliverables (checklist)
- [ ] Final cutover plan / runbook, rehearsed
- [ ] Dress rehearsal completed and lessons applied
- [ ] Production data migrated and reconciled; data sign-off
- [ ] Go-live readiness assessment and documented go/no-go
- [ ] End-user training delivered
- [ ] Production system live; cutover executed and closed out
- [ ] Hypercare structure operating (triage, standups, SLAs)
- [ ] Transition-to-operations handover complete
- [ ] Go-live sign-off obtained

## Quality gate: Deploy → Run
- Cutover executed and closed; production stable.
- Go-live signed off; data reconciled.
- Hypercare running; support team formally owns the solution.

## Common pitfalls
- A cutover plan that was never fully rehearsed — surprises land on go-live night.
- No rollback / contingency plan or unclear go/no-go authority.
- Training delivered too early (forgotten) or too late (users unready).
- Hypercare with no triage or exit criteria, so it drifts for months.
- Handover to support treated as a formality, leaving run teams blind to known issues.

## Useful prompts for daily work
- "Turn this cutover task list into a timed runbook with owners and rollback points."
- "Draft go/no-go criteria and a decision template for our steering committee."
- "Design a two-week hypercare model with triage tiers and daily standup structure."
- "Write a transition-to-operations handover checklist for the support team."
