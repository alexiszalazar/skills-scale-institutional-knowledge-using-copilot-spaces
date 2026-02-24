# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## UX Designer

### Role Summary
UX Designers advocate for the user experience throughout the product lifecycle. They translate user research into actionable designs and work closely with Product and Engineering to ensure solutions are both usable and feasible.

### Responsibilities
- Conduct user research and usability testing
- Create wireframes, prototypes, and design specifications
- Define and maintain design standards and component libraries
- Provide design feedback on implementation fidelity
- Advocate for accessibility and inclusive design

### Goals
- Deliver intuitive, accessible user experiences
- Reduce user friction and support adoption
- Ensure design intent is preserved through development

### Typical Communication
- Design reviews and prototype walk-throughs with Product and Engineering
- Usability testing summaries shared with Product Manager
- Inline design annotations and Figma/design-tool links in tickets

### Interactions & Handoffs
- **Product Manager:** co-defines problem statements and validates solution concepts; receives prioritization inputs for design work.
- **Developers:** hands off design specs and assets; reviews implementation against design intent.
- **Project Manager:** surfaces design-related risks, dependencies (e.g., design library availability), and timeline constraints.
- See [Role Handoffs & Interfaces](octoacme-role-handoffs-and-interfaces.md) for stage-by-stage detail.

---

## DevOps Engineer / Platform Engineer

### Role Summary
DevOps Engineers own the CI/CD pipelines, release automation, infrastructure reliability, and developer tooling. They bridge development and operations to enable fast, safe, and repeatable deployments.

### Responsibilities
- Design, build, and maintain CI/CD pipelines and deployment automation
- Manage cloud infrastructure, environments, and configuration-as-code
- Monitor system health, set up alerting, and drive incident response processes
- Enforce infrastructure security policies (secrets management, access controls)
- Support developers with build tooling, local environments, and performance profiling

### Goals
- Enable rapid, low-risk deployments
- Maximize system uptime and reliability
- Reduce toil through automation

### Typical Communication
- Release readiness confirmations with Project Manager and QA
- Incident reports and post-mortem write-ups
- Infrastructure change requests and runbook updates

### Interactions & Handoffs
- **Developers:** provides build and deployment tooling; reviews PRs for infrastructure-impacting changes.
- **Security Analyst:** collaborates on pipeline security scanning and hardening.
- **Project Manager:** flags infrastructure risks and deployment window requirements.
- **QA/Testing:** provisions staging environments and supports smoke test execution.
- See [Role Handoffs & Interfaces](octoacme-role-handoffs-and-interfaces.md) for stage-by-stage detail.

---

## Security Analyst / Security Champion

### Role Summary
Security Analysts identify, assess, and help remediate security and compliance risks across the product and infrastructure. They embed security practices into the development lifecycle rather than treating them as a final gate.

### Responsibilities
- Conduct threat modeling and security reviews during planning and design
- Manage vulnerability triage and track remediation progress
- Define and maintain security testing standards (SAST, DAST, dependency scanning)
- Advise on compliance requirements (e.g., GDPR, SOC 2) and track control status
- Develop and maintain incident response and escalation playbooks

### Goals
- Shift security left — catch issues early in the lifecycle
- Maintain a low vulnerability exposure and fast mean-time-to-remediate
- Ensure compliance requirements are met without blocking delivery

### Typical Communication
- Security review sign-off before major releases
- Vulnerability reports and remediation tracking updates
- Risk exceptions and acceptance documentation shared with Project Manager

### Interactions & Handoffs
- **Developers:** conducts code/design reviews; provides secure coding guidance; reviews fixes for security issues.
- **DevOps Engineer:** collaborates on pipeline scanning and secrets management.
- **Product Manager:** surfaces compliance constraints that impact feature design.
- **Project Manager:** escalates unmitigated high-severity risks and tracks security milestones.
- See [Role Handoffs & Interfaces](octoacme-role-handoffs-and-interfaces.md) for stage-by-stage detail.

---

## Customer Support Lead

### Role Summary
The Customer Support Lead aggregates user feedback, incident reports, and support trends to give Product and Engineering visibility into real-world product impact. They are the voice of the customer post-release.

### Responsibilities
- Triage and escalate critical user issues to engineering
- Synthesize support ticket trends and user pain points into actionable insights
- Co-author and maintain user-facing release notes, FAQs, and help documentation
- Coordinate communication to users during incidents and outages
- Participate in retrospectives to surface recurring support themes

### Goals
- Reduce time-to-resolution for user-impacting issues
- Provide Product with actionable, data-backed feedback loops
- Improve self-service through up-to-date help content

### Typical Communication
- Monthly support health reports to Product Manager and Stakeholders
- Escalation alerts for critical production issues
- Post-release feedback summaries shared after each release

### Interactions & Handoffs
- **Product Manager:** delivers synthesized user feedback and feature request signals; reviews release notes for accuracy.
- **Project Manager:** escalates critical user issues that require resourcing or timeline changes.
- **Developers:** routes reproducible bugs with support context; confirms fixes resolve the user-reported issue.
- See [Role Handoffs & Interfaces](octoacme-role-handoffs-and-interfaces.md) for stage-by-stage detail.

---

## Business Analyst

### Role Summary
Business Analysts bridge business strategy and technical execution. They translate business requirements into clear, measurable objectives and help teams understand the value and impact of their work.

### Responsibilities
- Elicit, document, and validate business and functional requirements
- Map business processes and identify improvement opportunities
- Define KPIs and success metrics aligned to business outcomes
- Produce business cases, cost-benefit analyses, and impact assessments
- Support acceptance testing by verifying business requirements are met

### Goals
- Ensure delivered solutions address the underlying business need
- Reduce rework caused by misunderstood requirements
- Provide clear traceability from business goals to delivered features

### Typical Communication
- Requirements workshops and review sessions with Product Manager and Stakeholders
- Business case documents and KPI dashboards shared with Sponsors
- Acceptance sign-off notes at the end of each iteration

### Interactions & Handoffs
- **Product Manager:** collaborates on problem framing and success metrics; validates prioritization against business value.
- **Project Manager:** clarifies scope boundaries and reports progress against business objectives.
- **Developers:** provides detailed acceptance criteria and answers requirement questions during development.
- **Stakeholders/Sponsors:** presents business cases and progress updates.
- See [Role Handoffs & Interfaces](octoacme-role-handoffs-and-interfaces.md) for stage-by-stage detail.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- For cross-role handoffs and a lifecycle RACI matrix, see [Role Handoffs & Interfaces](octoacme-role-handoffs-and-interfaces.md).

