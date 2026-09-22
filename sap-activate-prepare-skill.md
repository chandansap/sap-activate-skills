---
name: sap-activate-prepare
description: Guide for the SAP Activate PREPARE phase — project initiation, governance, team enablement, ways of working, and provisioning the starter/sandbox system for an S/4HANA program. Use when the user is kicking off a project, setting up governance or a project plan, onboarding/enabling the team, standing up Cloud ALM or the starter system, or planning the kickoff. Trigger on "project kickoff", "project charter", "governance", "team onboarding", "starter system", "ways of working", "sprint 0", "set up Cloud ALM".
---

# SAP Activate — Prepare Phase

Prepare turns a funded decision into a project that can actually run. The test of success is
blunt: **can the team do real Explore work tomorrow morning?** If governance, environments, and
enablement aren't ready, Explore stalls.

## Entry criteria
- Business case approved and program funded (Discover complete).
- Sponsor and core team named.

## Key activities (by workstream)
- **Project Management** — initiate the project: charter, governance model, RACI, project plan &
  schedule, risk/issue log, budget baseline, reporting cadence, and the delivery cadence (sprint
  length, ceremonies).
- **Ways of working** — agree how the team runs: agile roles (product owner, scrum master),
  backlog tooling, definition of ready/done, decision-making and escalation paths.
- **Team enablement** — onboard and train the team on Best Practices content, the target solution,
  and the tooling so Explore workshops are productive from day one.
- **Technical Architecture** — provision the **starter/sandbox system** loaded with Best Practices;
  set up landscape, transport/change strategy, and access.
- **Tooling setup** — configure **SAP Cloud ALM** (or SolMan): scope, requirements, tasks, and the
  project structure that later phases build on.
- **OCM & Adoption** — establish the change-management approach and stakeholder map early;
  don't defer it.

## Key deliverables (checklist)
- [ ] Project charter and governance model (RACI, steering structure)
- [ ] Project plan / schedule with phases, sprints, and milestones
- [ ] Ways-of-working / delivery standards documented
- [ ] Starter (Best Practices) system provisioned and accessible
- [ ] Cloud ALM / ALM tooling configured with initial scope
- [ ] Team enabled (enablement plan executed)
- [ ] Risk & issue log started; OCM approach drafted
- [ ] Kickoff completed

## Quality gate: Prepare → Explore
- Governance and plan approved.
- Team enabled and available.
- Starter system live; tooling ready.
Only pass the gate when all three hold — a "soft start" into Explore with no environment is the
most common early slip.

## Common pitfalls
- Kicking off Explore workshops before the starter system exists, so nothing can be shown live.
- No agreed definition of done — later phases argue about "complete" forever.
- Treating enablement as optional; unprepared business users derail Fit-to-Standard.
- OCM and data-migration leads not mobilized in Prepare, then rushed later.

## Useful prompts for daily work
- "Draft a project charter and RACI for a Public Cloud S/4HANA implementation."
- "Build a Prepare-phase checklist tailored to a Brownfield conversion."
- "Write a kickoff agenda and a definition of ready/done for our backlog."
