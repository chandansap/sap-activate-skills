---
name: sap-activate-run
description: Guide for the SAP Activate RUN phase — operating the live S/4HANA solution, exiting hypercare into steady-state support, adopting continuous innovation and new releases, and tracking value realization. Use when the user is running operations post go-live, closing out hypercare, setting up a support/operations model, managing upgrades or cloud release cycles, building a continuous-improvement backlog, or measuring benefits against the business case. Trigger on "hypercare exit", "steady state", "operations model", "continuous improvement", "release management", "upgrade", "value realization", "adopt new features".
---

# SAP Activate — Run Phase

Run is where value is actually realized — and where most programs quietly under-deliver by treating
go-live as the finish line. The test of success: **the business runs smoothly, the solution keeps
absorbing innovation, and someone can prove the value case came true.**

## Entry criteria
- Deploy gate passed: live, stable, hypercare running, support owns the solution.

## Key activities (by workstream)
- **Hypercare exit** — transition from hypercare to steady-state support against clear exit criteria
  (defect rate, ticket trends, business confidence). Don't let hypercare run indefinitely.
- **Operations** — run the operations model: monitoring, incident/problem management, and (with
  **SAP Cloud ALM** for operations) health monitoring, job/integration monitoring, and alerting.
- **Continuous improvement** — maintain a backlog of enhancements and deferred gaps; feed it through
  the same agile cadence used in Realize.
- **Release / innovation adoption** — for cloud, plan for **continuous/quarterly updates**: review
  release info, regression-test, and adopt new capabilities. For on-prem/private, plan periodic
  upgrades and feature-package adoption. Keeping clean-core pays off here.
- **Value realization** — measure the KPIs baselined in Discover; report benefits vs the business
  case and target the next wave of value.
- **Adoption** — sustain OCM: reinforce new ways of working, monitor user adoption, close training gaps.

## Key deliverables (checklist)
- [ ] Hypercare exit sign-off against criteria
- [ ] Steady-state support / operations model in place
- [ ] Monitoring and alerting operational (Cloud ALM / SolMan)
- [ ] Continuous-improvement backlog established and prioritized
- [ ] Release / upgrade management cadence defined
- [ ] Value realization tracking against Discover KPIs
- [ ] Adoption metrics reviewed; enablement gaps closed

## Common pitfalls
- Declaring victory at go-live and never measuring the promised value.
- Hypercare with no exit criteria, so the project team never actually leaves.
- Falling behind on cloud releases until an adoption backlog becomes a mini-project.
- Custom code that breaks on every update because clean-core was ignored earlier.
- No owner for continuous improvement, so enhancements pile up unaddressed.

## Useful prompts for daily work
- "Draft hypercare exit criteria and a transition plan to steady-state support."
- "Design a continuous-improvement intake and prioritization process."
- "Build a quarterly release-adoption playbook for Public Cloud S/4HANA."
- "Create a value-realization scorecard mapped to our original business-case KPIs."
