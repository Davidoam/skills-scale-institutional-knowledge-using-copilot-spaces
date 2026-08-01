# OctoAcme Project Management Documentation

Welcome to OctoAcme's project management documentation. This collection of guides helps teams deliver projects consistently, track progress effectively, and continuously improve our processes. Use this README as the main entry point to find process docs, quick references, and how to contribute updates.

## Quick Navigation

### Core Guides
- **Project Management Overview** — docs/octoacme-project-management-overview.md
- **Roles & Personas** — docs/octoacme-roles-and-personas.md

### Project Lifecycle Guides
- **Project Initiation** — docs/octoacme-project-initiation.md
- **Project Planning** — docs/octoacme-project-planning.md
- **Execution & Tracking** — docs/octoacme-execution-and-tracking.md
- **Release & Deployment** — docs/octoacme-release-and-deployment.md
- **Retrospective & Continuous Improvement** — docs/octoacme-retrospective-and-continuous-improvement.md

### Cross-Cutting Guides
- **Risk Management & Communication** — docs/octoacme-risks-and-communication.md

(Each link above is the path under this repository's docs/ directory.)

## Brief overview of OctoAcme project management processes

OctoAcme follows a lightweight, iterative approach focused on delivering measurable customer value, reducing risk through small increments, and supporting continuous improvement.

High-level lifecycle:
1. Initiation — validate the problem, confirm stakeholders, and produce a Project One-pager with success metrics.
2. Planning — break approved work into backlog items, estimate, identify dependencies, and produce a release plan.
3. Execution & Tracking — implement in small increments, follow PR/CI practices, use the project board for flow (Backlog → Ready → In Progress → In Review → QA → Done), and track progress with velocity/burndown.
4. Release & Deployment — follow pre-release checks, run smoke tests, deploy via pipelines, and prepare rollback plans.
5. Close & Retrospective — hold retrospectives, capture action items, and measure the impact of improvements.

Core practices:
- Small, reviewable PRs with acceptance criteria and linked issue
- CI for tests, linting, and security checks
- Definition of Done and acceptance criteria for backlog items
- Regular demos, standups, and weekly PM/PdM syncs
- Maintain a Risk Register and clear escalation paths

## Quick reference: where to start
- New to process docs: start at docs/octoacme-project-management-overview.md
- Want to update a process doc: use the issue template at .github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml and link your suggested changes
- Need to initiate a new project: follow docs/octoacme-project-initiation.md
- Planning work and sprints: see docs/octoacme-project-planning.md
- Release checklist: see docs/octoacme-release-and-deployment.md

## How to contribute
1. Fill the "Add Content to Project Management Process Docs" issue template (.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) for new content or updates.
2. Attach example content or suggested wording in the issue.
3. Once reviewed and approved, create or update the appropriate file in docs/ and open a PR that references the issue.

## Owners & reviews
- Primary doc owner: Project Manager / Documentation owner (add specific owner in project context)
- Use the issue template to request reviews from product, engineering, or PM as needed.

## Acceptance criteria for this README
- Links to all docs in docs/ are present
- README provides a concise overview of OctoAcme processes
- Contribution instructions reference the issue template
- README is stored in docs/ as docs/README.md

---
