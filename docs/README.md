# OctoAcme Project Management Docs

Welcome to the OctoAcme project management documentation. This README provides a brief overview of how OctoAcme runs projects and links to every process document in this directory.

## Project Management Processes Overview

OctoAcme uses an iterative, customer-first approach to deliver projects successfully. All cross-functional initiatives follow a structured lifecycle with five stages: **Initiation** (defining the problem, stakeholders, and high-level timeline), **Planning** (scoping work, setting milestones, and mapping dependencies), **Execution & Tracking** (building, testing, and iterating in short cycles), **Release & Deployment** (shipping, verifying, and announcing), and **Retrospective & Continuous Improvement** (capturing learnings and driving lasting process improvements). Key artifacts used throughout this lifecycle include Project Charters, roadmaps, sprint backlogs, risk registers, and retrospective notes.

Each project is staffed with clearly defined roles to ensure accountability and alignment. The **Project Manager (PM)** coordinates delivery, schedules, risks, and communications. The **Product Manager (PdM)** owns the product vision, prioritizes the backlog, and measures success. **Developers** implement features and maintain quality through code reviews and automated testing. **QA/Testing** validates acceptance criteria and release readiness. **Stakeholders** provide business inputs and approvals at key checkpoints.

OctoAcme maintains a consistent communication cadence to keep all parties informed and aligned. The PM and PdM meet weekly for alignment, the delivery team holds twice-weekly standups, and stakeholders receive monthly status updates. A standardized status report template (owner, summary, milestones, risks, next steps) serves as the single source of truth for project health. Escalation paths are documented in each project's risk register so blockers reach the right decision-makers quickly.

Quality is built into every phase. Pull requests require peer review before merging, and CI checks (linting, automated tests, security scans) must pass before code reaches the main branch. Testing spans unit, integration, and end-to-end coverage. A formal release-readiness checklist—covering feature completion, regression testing, rollback planning, and stakeholder sign-off—gates every production deployment. Post-release monitoring confirms that releases meet the defined success metrics before a project is formally closed.

## Documentation Index

| Document | Description |
|---|---|
| [OctoAcme Project Management Overview](octoacme-project-management-overview.md) | High-level introduction to principles, roles, artifacts, and the project lifecycle |
| [Project Initiation Guide](octoacme-project-initiation.md) | How to kick off a new project: problem statement, charter, and stakeholder alignment |
| [Project Planning Guide](octoacme-project-planning.md) | Scope definition, milestone planning, dependency mapping, and resource allocation |
| [Execution & Tracking Guide](octoacme-execution-and-tracking.md) | Sprint cadence, progress tracking, and managing in-flight work |
| [Risk Management & Communication](octoacme-risks-and-communication.md) | Risk identification, mitigation strategies, and communication templates |
| [Release & Deployment Guide](octoacme-release-and-deployment.md) | Release readiness checklist, deployment steps, and post-release monitoring |
| [Retrospective & Continuous Improvement Guide](octoacme-retrospective-and-continuous-improvement.md) | Running retrospectives and turning learnings into lasting process improvements |
| [Roles and Personas](octoacme-roles-and-personas.md) | Detailed responsibilities and communication patterns for each project role |

## How to Use and Update These Docs

- **Reading:** Start with the [Overview](octoacme-project-management-overview.md) if you are new to OctoAcme's project management approach, then explore the phase-specific guides relevant to your current work.
- **Updating:** Open a pull request against `main` and reference the related issue in your PR description. Keep changes focused and aligned with the existing structure.
- **Artifacts:** Store project-specific artifacts (charters, risk registers, retrospective notes) in the `docs/` folder of your project repository. To make documents available as Copilot Spaces context, copy or symlink them into the `.copilot/` directory.

Closes #2
