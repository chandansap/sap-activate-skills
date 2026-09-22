---
name: sap-activate-explore
description: Guide for the SAP Activate EXPLORE phase — running Fit-to-Standard (or Fit/Gap) workshops, confirming solution fit, capturing delta requirements and gaps, building and prioritizing the backlog, and producing solution design for an S/4HANA program. Use when the user is preparing or facilitating fit-to-standard workshops, writing user stories, logging gaps, deciding WRICEF/extensions, designing integrations or data migration, or baselining scope. Trigger on "fit-to-standard", "fit gap", "workshop agenda", "backlog", "user stories", "delta requirements", "solution design", "WRICEF", "exit criteria for explore".
---

# SAP Activate — Explore Phase

Explore is where a program is won or lost. Through **Fit-to-Standard** workshops the team validates
the Best Practices solution against how the business actually works, keeps standard where it can,
and captures only the true deltas as gaps. The discipline that matters: **default to standard,
justify every gap.** Every gap accepted here is cost and risk carried through Realize, Deploy, and
Run.

## Entry criteria
- Prepare gate passed: team enabled, starter system live, tooling ready.

## Fit-to-Standard vs Fit/Gap
- **Fit-to-Standard** (cloud / Best-Practice-led): show the standard process in the system, confirm
  fit, capture deltas. The process leads; configuration follows.
- **Fit/Gap** (on-prem / more custom): compare requirements to capabilities and document gaps.
Use Fit-to-Standard language for cloud/RISE; Fit/Gap for heavily customized on-prem.

## Running good workshops
- Prepare per process area: agenda, the Best Practice scenario to demo, sample data, and the
  business SMEs who can actually decide.
- Demo the standard **live** in the starter system, then ask "what stops this from working for you?"
- Capture outcomes in three buckets: **Fit** (adopt standard), **Delta** (config change),
  **Gap** (needs extension/WRICEF or a process change).
- Log every decision and its owner. Undocumented verbal agreements are future disputes.

## From workshops to backlog
- Turn deltas and gaps into **user stories** with acceptance criteria and priority
  (MoSCoW or business value).
- Classify build work as **WRICEF**: Workflows, Reports, Interfaces, Conversions, Enhancements,
  Forms — each needs a functional and technical design.
- Sequence the backlog into releases and sprints for Realize.

## Design the cross-cutting streams now, not later
- **Integration** — target architecture, interfaces, middleware (e.g. SAP Integration Suite),
  and the interface inventory.
- **Data Migration** — source systems, objects, volumes, cleansing responsibilities, and the
  migration approach/tooling; agree who owns data quality.
- **Analytics, Security/Authorizations, Extensibility** — capture the design intent so Realize
  isn't surprised.

## Key deliverables (checklist)
- [ ] Fit-to-Standard workshop results and decisions log
- [ ] Confirmed scope (baselined) with in/out clearly stated
- [ ] Prioritized backlog of user stories with acceptance criteria
- [ ] Gap list with WRICEF classification and effort estimates
- [ ] Solution design documents (functional + technical) for gaps
- [ ] Integration design and interface inventory
- [ ] Data migration design and data-quality plan
- [ ] Security/authorization concept; analytics requirements
- [ ] Release and sprint plan for Realize

## Quality gate: Explore → Realize
- Backlog prioritized and **signed off** by the business.
- Solution design approved; scope baselined with change control in force.
- Delta/gap list agreed with effort and impact.
Do not start building until the backlog is baselined — open scope in Realize is the number-one
cause of overrun.

## Common pitfalls
- "Recreating ECC" — customizing the standard back to the old system and losing the value case.
- Accepting gaps without challenging the requirement or offering a standard alternative.
- Workshops attended by people who can't make decisions, so nothing is confirmed.
- Deferring integration and data-migration design, then discovering the hard parts in Realize.
- Vague user stories with no acceptance criteria — untestable in Realize.

## Useful prompts for daily work
- "Draft a Fit-to-Standard workshop agenda for Order-to-Cash and list the SMEs to invite."
- "Turn these workshop notes into prioritized user stories with acceptance criteria."
- "Classify these gaps as WRICEF and flag which ones I should push back on as standard."
- "What are my exit criteria for Explore, and what's still open?"
