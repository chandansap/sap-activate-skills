---
name: sap-activate-realize
description: Guide for the SAP Activate REALIZE phase — iteratively configuring and building the S/4HANA solution, developing WRICEF/extensions and integrations, executing test data-migration loads, and running the test cycles (unit / string, integration/SIT, UAT) before go-live. Use when the user is configuring, building extensions, wiring integrations, planning or running test cycles, doing data-migration mock loads, setting up authorizations, or starting cutover planning. Trigger on "configure", "build", "sprint", "unit test", "integration test", "SIT", "UAT", "mock migration", "cutover plan", "test strategy", "realize exit criteria".
---

# SAP Activate — Realize Phase

Realize builds the solution the backlog described, in **iterations**. Each sprint configures a slice,
builds the gaps for it, and tests it — so quality is proven continuously, not discovered at the end.
The test of success: **the solution is built, integrated, and has passed testing, with a credible
plan to move it to production.**

## Entry criteria
- Explore gate passed: backlog baselined, design approved, scope under change control.

## Key activities (by workstream)
- **Configuration** — apply Guided/Expert Configuration in sprints, incrementally activating and
  adjusting Best Practices scope to match the confirmed design.
- **Extensibility / Development** — build the WRICEF backlog (workflows, reports, interfaces,
  conversions, enhancements, forms); use clean-core / side-by-side extensibility (BTP) in cloud to
  keep the core upgrade-safe.
- **Integration** — build and unit-test interfaces against the interface inventory; establish
  connectivity and error handling.
- **Data Management** — build migration objects and run **mock/test loads** in repeated cycles;
  reconcile results and drive data quality to a go/no-go standard.
- **Testing** — execute the test pyramid: unit/string tests each sprint, then **System Integration
  Testing (SIT)** end-to-end across processes and interfaces, then **User Acceptance Testing (UAT)**
  with the business. Track defects to closure.
- **Security & Authorizations** — build and test roles against real process flows.
- **Analytics** — build reports/dashboards and embedded analytics.
- **Transition / Cutover** — begin the cutover plan and sequence; schedule a dress rehearsal.
- **OCM & Enablement** — build training materials and prepare end-user training for Deploy.

## Key deliverables (checklist)
- [ ] Configured solution across in-scope processes
- [ ] WRICEF / extensions built and unit-tested
- [ ] Integrations built and tested
- [ ] Data migration executed and reconciled in test (mock loads)
- [ ] Test strategy + results: unit, SIT, and UAT signed off
- [ ] Defect log driven to acceptable closure
- [ ] Security roles built and tested
- [ ] Training materials prepared
- [ ] Cutover plan drafted; dress rehearsal scheduled
- [ ] Go-live readiness assessment started

## Quality gate: Realize → Deploy
- Build complete for baselined scope.
- SIT and UAT passed; open defects within agreed thresholds.
- Data migration validated in at least one full mock load.
- Cutover plan approved; go-live readiness confirmed.

## Common pitfalls
- Leaving integration and data migration to the last sprints — they always take longer than hoped.
- Weak UAT (business "clicks through" instead of testing real scenarios), so defects surface post-go-live.
- Scope creep via "small" change requests bypassing change control.
- Custom code that breaks clean-core, creating upgrade debt in Run.
- No mock cutover, so the real cutover is the first full rehearsal.

## Useful prompts for daily work
- "Draft a test strategy covering unit, SIT, and UAT for our Procure-to-Pay scope."
- "Generate UAT test cases from these user stories."
- "Build a data-migration mock-load plan with reconciliation checkpoints."
- "Draft a cutover plan skeleton with a dress-rehearsal sequence."
- "Are we ready for the Realize→Deploy gate? Check what's still open."
