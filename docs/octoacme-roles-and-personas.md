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

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Personas (recommended additions)

Below are recommended persona entries to add to the document. For each persona include: Role Summary, Responsibilities, and Interactions with existing roles.

### Technical Lead
Role Summary
- Senior engineer responsible for architectural direction and technical decisions for the project.

Responsibilities
- Make or coordinate key technical design decisions and trade-offs.
- Ensure implementation aligns with architecture and non-functional requirements (scalability, maintainability).
- Mentor developers and review complex PRs.
- Own technical risk identification and mitigation.

Interactions
- Works closely with Developers on design and implementation, with the PM to surface technical constraints affecting scope/timeline, and with the Product Manager to align technical approach with product goals.

---

### Release Manager
Role Summary
- Coordinates release planning, deployment windows, rollbacks, and release communications.

Responsibilities
- Maintain release calendar and deployment checklists.
- Coordinate staging/production smoke tests and rollback plans.
- Author or review Release Notes and post-release verifications.
- Ensure rollback and mitigation steps are documented and rehearsed.

Interactions
- Works with Developers and QA to verify release readiness, with PM for scheduling and stakeholder communication, and with Platform/Infrastructure Owner for deployment support.

---

### UX Researcher / Designer
Role Summary
- Represents user needs through research, prototypes, and usability validation.

Responsibilities
- Run user interviews, usability tests, and synthesize findings.
- Provide wireframes, acceptance criteria tied to UX, and validation plans.
- Advise on accessibility and usability requirements.

Interactions
- Partners with Product Manager to define success metrics and acceptance criteria, with Developers on implementation details, and with QA on UX acceptance testing.

---

### Security Liaison
Role Summary
- Point of contact for security-related questions, threat modeling, and compliance requirements.

Responsibilities
- Conduct security reviews, coordinate vulnerability scans, and ensure mitigation plans.
- Advise on data handling, access controls, and compliance obligations.
- Coordinate with Security team for incident detection and response.

Interactions
- Works with Developers and Technical Lead on secure design, with PM on risk/mitigation communication, and with Security on incident response and escalations.

---

### Data Analyst / Analytics Owner
Role Summary
- Owns measurement, instrumentation, and reporting for project success metrics.

Responsibilities
- Define metrics, ensure event instrumentation is implemented, and build dashboards/reports.
- Validate experiments and help interpret results.
- Maintain data quality and track critical signals post-release.

Interactions
- Works with Product Manager to define success metrics, with Developers to implement events, and with PM to include reporting in release criteria.

---

### Platform / Infrastructure Owner
Role Summary
- Responsible for operational reliability, tooling, and platform constraints the project depends on.

Responsibilities
- Provide guidance on platform limitations, capacity planning, and required environment configurations.
- Support deployment and incident response.
- Maintain environment provisioning and CI/CD health.

Interactions
- Works with Release Manager and Developers during deployments, with PM on scheduling and with Technical Lead on architectural implications.

---

### Customer Success / Support Liaison
Role Summary
- Represents post-release user impact, escalations from customers, and support readiness.

Responsibilities
- Prepare support playbooks, triage incoming issues post-release, and collect qualitative feedback.
- Coordinate urgent customer communications and escalations.

Interactions
- Works with PM for communication, with QA for reproducing issues, and with Product Manager to prioritize fixes or improvements.

---

### Business Analyst / Requirements Analyst (optional)
Role Summary
- Helps translate stakeholder requirements into clear acceptance criteria and user stories.

Responsibilities
- Capture detailed requirements, model workflows, and maintain traceability to business outcomes.
- Provide clear acceptance criteria and edge-case specifications.

Interactions
- Works with Product Manager and PM during planning, and with Developers/QA to clarify acceptance criteria.

---

## Interactions & Handoffs (short checklist)
- Each newly defined role should include explicit handoff points with other roles (who informs whom and at what moment).
- Add decision gates for cross-role approvals (e.g., release sign-off, security sign-off, and product acceptance).
- Include contact or escalation points for operational roles (Platform, Security, Support).

---

## Suggested RACI-style ownership matrix (sample)

| Activity / Role | PM | PdM | Dev | Tech Lead | QA | Release Mgr | Security Liaison | Data Analyst | Support |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Define success metrics | A | R | I | C | I | I | I | R | C |
| Acceptance criteria | C | R | C | C | A | I | I | C | I |
| Architecture decisions | I | C | R | A | I | I | C | I | I |
| Release sign-off | R | C | C | C | A | R | C | I | C |
| Security review | I | I | C | C | I | I | A | I | I |
| Instrumentation & dashboards | I | R | C | I | I | I | I | A | I |
| Incident triage | R | C | C | C | I | I | A | I | R |

Legend: R = Responsible, A = Accountable, C = Consulted, I = Informed

---

Notes:
- For each new persona added above, we should add a short "Decision points & Handoffs" subsection showing the exact moment in the flow where this role must be engaged (e.g., Security Liaison before merging high-scope changes; Release Manager 1 week before scheduled production deployments).
- Consider adding these new roles to the "How these personas are used in the exercise" section as persona prompts for Copilot Spaces and for onboarding templates.
