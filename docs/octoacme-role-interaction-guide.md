# OctoAcme Role Interaction Guide

## Purpose
This guide describes how each role at OctoAcme interacts with others throughout a project lifecycle. Use it to understand collaboration points, handoff expectations, and communication cadence between roles.

---

## Role Interaction Matrix

The table below summarizes the primary collaboration points between roles. Each cell describes the nature of the interaction.

| Role | Project Manager | Product Manager | Developer | Scrum Master | UX/UI Designer | DevOps Engineer | Business Analyst | QA/Testing | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|
| **Project Manager** | — | Weekly alignment on scope, timeline, priorities | Sprint and milestone planning | Blocker escalation and delivery coordination | Design milestone tracking | Release scheduling and deployment risk | Requirements clarity and planning support | QA schedule and acceptance sign-off | Status reporting and escalation |
| **Product Manager** | Roadmap and scope trade-offs | — | Backlog refinement and feature specs | Sprint goal alignment | Design validation and user research priorities | Informs on infra constraints affecting timelines | Requirements translation and story refinement | Acceptance criteria definition | Stakeholder briefings and roadmap updates |
| **Developer** | Sprint commitments and status | Feature clarification and backlog grooming | — | Daily standups and impediment removal | Design handoff review and implementation questions | CI/CD usage and infra-as-code contributions | Requirement clarification during implementation | PR review and test support | — |
| **Scrum Master** | Cross-team blocker escalation | Backlog readiness and sprint goal alignment | Agile coaching and impediment removal | — | Ceremony participation | Ceremony participation | Ceremony participation | Ceremony participation | — |
| **UX/UI Designer** | Milestone and scope communication | Requirements translation and design validation | Design handoff and implementation review | Sprint ceremony participation | — | Environment requirements for design tooling | Requirements workshops | UI acceptance validation | Design reviews and usability feedback |
| **DevOps Engineer** | Release readiness and operational risk | Infrastructure constraint advisement | Build and deployment tooling support | Sprint ceremony participation | Environment support for design tooling | — | — | Test environment maintenance | — |
| **Business Analyst** | Planning inputs and requirements clarity | Roadmap priorities and requirements alignment | Requirements clarification during delivery | Sprint ceremony participation | Requirements workshops | — | — | Acceptance criteria validation | Requirements elicitation and sign-off |
| **QA/Testing** | Acceptance schedule and sign-off | Acceptance criteria definition | PR and code review collaboration | Sprint ceremony participation | UI acceptance against design specs | Test environment requests | Acceptance criteria validation | — | — |
| **Stakeholders** | Status updates and escalation approvals | Roadmap and priority inputs | — | — | Design feedback and usability review | — | Requirements and sign-off | — | — |

---

## Key Collaboration Points by Lifecycle Phase

### Initiation
- **Project Manager + Product Manager**: align on problem statement, success metrics, and high-level scope
- **Business Analyst + Stakeholders**: elicit initial requirements and business objectives
- **Scrum Master + Project Manager**: establish team structure, Agile ceremonies, and initial sprint cadence

### Planning
- **Product Manager + Business Analyst + Developers**: refine backlog and define user stories with acceptance criteria
- **UX/UI Designer + Product Manager**: kick off user research and initial design concepts
- **DevOps Engineer + Project Manager**: assess infrastructure readiness and deployment strategy
- **Project Manager + all roles**: confirm resource availability and milestone schedule

### Execution
- **Scrum Master**: facilitates daily standups, sprint planning, reviews, and retrospectives for all roles
- **UX/UI Designer → Developers**: design handoff with annotated specs before implementation begins
- **Business Analyst + Developers**: ongoing requirements clarification as implementation progresses
- **DevOps Engineer**: maintains CI/CD pipelines; responds to deployment issues raised by developers or PM

### Review & Release
- **QA/Testing + UX/UI Designer**: validate implementation against design specs and acceptance criteria
- **DevOps Engineer + Project Manager**: confirm deployment readiness and release window
- **Business Analyst + Stakeholders**: obtain acceptance sign-off before release
- **Product Manager + Stakeholders**: communicate release outcomes and success metrics

### Retrospective
- **Scrum Master**: facilitates retrospective; all team members participate
- **Project Manager**: captures action items and updates process documentation
- **All roles**: contribute learnings to continuous improvement cycle

---

## Handoff Points and Expectations

| Handoff | From | To | Artifact / Output |
|---|---|---|---|
| Design to Development | UX/UI Designer | Developer | Annotated mockups, component specs, asset files |
| Requirements to Development | Business Analyst | Developer | User stories with acceptance criteria, process flow diagrams |
| Sprint Goal Agreement | Product Manager | Scrum Master + Team | Prioritized sprint backlog with clear goals |
| Deployment Approval | DevOps Engineer | Project Manager | Deployment readiness checklist, rollback plan |
| Acceptance Sign-off | QA/Testing + Business Analyst | Project Manager | Acceptance test results, stakeholder approval |
| Post-Release Metrics | DevOps Engineer + Product Manager | Stakeholders | Release notes, dashboards, outcome metrics |

---

## Communication Cadence Summary

| Cadence | Participants | Purpose |
|---|---|---|
| Daily standup | All delivery roles (Developers, QA, Scrum Master, BA, DevOps) | Progress, blockers, dependencies |
| Sprint planning | All delivery roles + Product Manager | Backlog refinement and sprint commitment |
| Sprint review / demo | All delivery roles + Product Manager + Stakeholders | Demonstrate increment and gather feedback |
| Sprint retrospective | All delivery roles + Scrum Master | Continuous improvement |
| Weekly PM + PdM sync | Project Manager + Product Manager | Scope, timeline, and priority alignment |
| Design review | UX/UI Designer + Product Manager + relevant Developers | Validate design direction before handoff |
| Monthly stakeholder update | Project Manager + Product Manager + Stakeholders | Status, risks, and roadmap progress |
