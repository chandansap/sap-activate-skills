# SAP Activate Skills for Claude

A library of **Claude Skills** that turn the SAP Activate implementation methodology into an
interactive delivery coach. Point Claude at these and a consultant can ask where they are, what
"done" looks like for the current phase, what's due before the next quality gate, and where the
common traps are — grounded in the actual Activate structure instead of generic AI guesswork.

Built for day-to-day use by SAP consultants and delivery teams working on S/4HANA (Cloud, on-prem,
or RISE with SAP) implementations.

## What's in here

| Skill | Covers |
|-------|--------|
| `sap-activate-methodology` | **Start here.** The whole methodology: 6 phases, workstreams, quality gates, deployment approaches, tooling. Routes to the phase skills. |
| `sap-activate-discover` | Business case, scoping, deployment-approach decision, Readiness Check / DDA |
| `sap-activate-prepare` | Project initiation, governance, team enablement, starter system, Cloud ALM setup |
| `sap-activate-explore` | Fit-to-Standard workshops, backlog & user stories, gap/WRICEF classification, solution design |
| `sap-activate-realize` | Iterative configuration & build, integrations, test cycles (unit/SIT/UAT), mock data loads, cutover planning |
| `sap-activate-deploy` | Cutover execution, production migration, go/no-go, training, hypercare, transition to operations |
| `sap-activate-run` | Hypercare exit, steady-state operations, release/innovation adoption, value realization |

## Coverage vs the Activate methodology

These skills map 1:1 to the six official SAP Activate phases (Discover → Prepare → Explore →
Realize → Deploy → Run) and reference the cross-phase workstreams (Project Management, OCM, Solution
Adoption, Application Design & Configuration, Extensibility, Integration, Data Management, Testing,
Analytics, Technical Architecture, Security, Transition/Cutover, Operations). Each phase skill
includes entry criteria, activities by workstream, a deliverables checklist, the quality gate to the
next phase, common pitfalls, and ready-to-use prompts.

Deployment approaches covered: **New Implementation (Greenfield)**, **System Conversion (Brownfield)**,
and **Selective Data Transition**.

> If you have your own existing Activate skill(s), diff them against `sap-activate-methodology`
> (structure and gates) and the phase checklists to spot gaps — most homegrown versions are missing
> explicit **quality-gate criteria** and the **cross-phase workstreams** (OCM, data migration, and
> integration being started in Explore rather than Realize).

## How to use these

Each folder is a self-contained skill (`SKILL.md` with YAML frontmatter). Depending on where you run
Claude:

- **Claude.ai / Claude apps** — add a skill from Settings → Capabilities → Skills (where enabled for
  your account/org). Upload or point to a skill folder.
- **Claude Code** — place skill folders where your project or user skills live so they load
  automatically.
- **API / Agent SDK** — reference the skills in your skills configuration.

Once loaded, they trigger automatically when your request matches — e.g. "draft a fit-to-standard
agenda for Order-to-Cash" pulls in `sap-activate-explore`; "are we ready to go live?" pulls in
`sap-activate-deploy`. You can also just ask the coach directly: *"Which Activate phase am I in and
what's my next gate?"*

## Example prompts

- "Which phase am I in if we've signed off the backlog but haven't started building?"
- "Draft a Fit-to-Standard workshop agenda for Procure-to-Pay and who to invite."
- "Turn these workshop notes into prioritized user stories with acceptance criteria."
- "Build a cutover runbook skeleton with a dress-rehearsal sequence."
- "Draft hypercare exit criteria and a transition-to-steady-state plan."

## Repo layout

```
sap-activate-skills/
├── README.md
├── sap-activate-methodology/SKILL.md
├── sap-activate-discover/SKILL.md
├── sap-activate-prepare/SKILL.md
├── sap-activate-explore/SKILL.md
├── sap-activate-realize/SKILL.md
├── sap-activate-deploy/SKILL.md
└── sap-activate-run/SKILL.md
```

## Notes & contributing

Activate content (deliverable lists, tooling) evolves — SAP Cloud ALM is now the default ALM for new
cloud/RISE projects, replacing much of SAP Solution Manager's role. Treat the SAP **Roadmap Viewer**
and **SAP Cloud ALM** content as the authoritative source and refine these skills as your delivery
standards mature. PRs and phase-specific templates welcome.

---

*Not affiliated with or endorsed by SAP SE. "SAP", "S/4HANA", and "SAP Activate" are trademarks of
SAP SE. This is a community teaching aid.*
