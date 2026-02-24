# OctoAcme — Role Handoffs & Interfaces

This document provides a compact RACI-style responsibility matrix and explicit handoff signals for each lifecycle stage. Use it alongside [Roles & Personas](octoacme-roles-and-personas.md) and the [Project Management Overview](octoacme-project-management-overview.md).

**RACI Key:** R = Responsible, A = Accountable, C = Consulted, I = Informed

---

## Lifecycle RACI Matrix

| Activity | PM | PdM | Dev | QA | UX | DevOps | Security | Support Lead | BA | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|---|
| **Initiation** | | | | | | | | | | |
| Define problem statement & success metrics | C | A/R | I | I | C | I | I | I | C | C |
| Identify stakeholders & sponsors | A/R | C | I | I | I | I | I | I | C | I |
| Initial risk & compliance assessment | C | C | I | I | I | C | R | I | C | I |
| **Planning** | | | | | | | | | | |
| Backlog creation & prioritization | C | A/R | C | C | C | C | C | C | C | I |
| Requirements & acceptance criteria | C | R | C | C | C | I | C | I | A/R | I |
| UX research & design | I | C | C | I | A/R | I | I | I | I | I |
| Infrastructure & environment planning | C | I | C | I | I | A/R | C | I | I | I |
| Security threat modeling | C | C | C | I | I | C | A/R | I | I | I |
| Release plan & milestones | A/R | C | C | C | I | C | C | I | C | I |
| **Execution** | | | | | | | | | | |
| Feature implementation | I | I | A/R | C | C | C | C | I | I | I |
| Design review & implementation fidelity | I | C | R | I | A/R | I | I | I | I | I |
| CI/CD pipeline & build health | I | I | C | C | I | A/R | C | I | I | I |
| Security scanning & code review | I | I | C | C | I | C | A/R | I | I | I |
| QA & acceptance testing | C | C | C | A/R | C | C | C | I | C | I |
| Status reporting | A/R | C | I | I | I | I | I | I | C | I |
| **Release** | | | | | | | | | | |
| Release readiness sign-off | A/R | C | C | C | I | C | C | I | I | I |
| Deployment execution | C | I | C | C | I | A/R | C | I | I | I |
| Security release sign-off | C | I | I | C | I | C | A/R | I | I | I |
| Release notes & user communication | C | C | I | I | I | I | I | A/R | C | I |
| Post-deploy verification | C | I | C | R | I | R | C | I | I | I |
| **Retrospective** | | | | | | | | | | |
| Facilitate retrospective | A/R | C | C | C | C | C | C | C | C | I |
| Capture action items | A/R | C | C | C | C | C | C | C | C | I |
| Support feedback synthesis | I | C | I | I | I | I | I | A/R | C | I |
| Metrics & business value review | C | R | I | I | I | I | I | C | A/R | C |

---

## Handoff Signals by Stage

### Initiation → Planning

| From | To | Output / Signal |
|---|---|---|
| Product Manager | Business Analyst | Approved problem statement, business goals, and draft success metrics |
| Business Analyst | Product Manager & PM | Validated requirements doc with KPIs and business case |
| Security Analyst | PM & PdM | Initial compliance and threat landscape summary |
| Project Manager | All roles | Kickoff meeting scheduled; project charter draft shared |

### Planning → Execution

| From | To | Output / Signal |
|---|---|---|
| Product Manager | Developers & QA | Prioritized backlog with acceptance criteria |
| Business Analyst | Developers | Detailed functional requirements and data flow diagrams |
| UX Designer | Developers | Finalized design specs, prototypes, and asset handoff |
| DevOps Engineer | Developers & QA | Environments provisioned; CI/CD pipeline ready; runbooks published |
| Security Analyst | Developers & DevOps | Threat model and required security controls documented |
| Project Manager | All roles | Sprint plan confirmed; roles and DRI (Directly Responsible Individual) assigned |

### Execution → Release

| From | To | Output / Signal |
|---|---|---|
| Developers | QA | Feature branches merged; staging deployment complete |
| QA | Project Manager & PdM | Test results and acceptance sign-off (pass/fail report) |
| UX Designer | QA & Developers | Design review sign-off confirming implementation fidelity |
| Security Analyst | Project Manager | Security sign-off (or documented risk acceptance for any open findings) |
| DevOps Engineer | Project Manager & QA | Deployment window confirmed; rollback plan documented |
| Business Analyst | PdM & PM | Business acceptance criteria verified |

### Release → Retrospective

| From | To | Output / Signal |
|---|---|---|
| DevOps Engineer | All roles | Post-deploy monitoring summary; incident flag (if any) |
| Customer Support Lead | PdM & PM | Post-release feedback summary; top user issues |
| Project Manager | All roles | Retro scheduled; retrospective notes and action items published |
| Business Analyst | Stakeholders & PdM | Outcomes vs. KPIs dashboard or summary |

---

## Role Interaction Quick Reference

| Role pair | Primary interface |
|---|---|
| PM ↔ PdM | Weekly sync; scope, timeline, and priority trade-offs |
| PdM ↔ UX Designer | Problem framing, research insights, design validation |
| PdM ↔ Business Analyst | Requirements alignment, success metrics, business value |
| Developers ↔ UX Designer | Design spec handoff, implementation review |
| Developers ↔ DevOps | Build tooling, pipeline issues, environment support |
| Developers ↔ Security Analyst | Secure code review, vulnerability remediation |
| DevOps ↔ Security Analyst | Pipeline hardening, secrets management, scanning |
| PM ↔ Security Analyst | Risk register updates, release sign-off |
| PM ↔ DevOps | Deployment scheduling, incident escalation |
| PdM ↔ Customer Support Lead | User feedback loops, release communication |
| PM ↔ Customer Support Lead | Critical issue escalation, support SLAs |

---

## Related Docs
- [Roles & Personas](octoacme-roles-and-personas.md)
- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Release & Deployment](octoacme-release-and-deployment.md)
- [Risks & Communication](octoacme-risks-and-communication.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
