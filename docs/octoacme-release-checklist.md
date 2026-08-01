# OctoAcme Release Checklist

Purpose: A compact checklist to confirm readiness to deploy and to document required owners for each item.

Pre-release
- [ ] Release Manager assigned (owner)
- [ ] Release window scheduled and stakeholders notified (PM + Release Manager)
- [ ] All PRs merged, CI green, and security scans completed (Developers, QA, Security Liaison)
- [ ] Release notes drafted and reviewed (Release Manager, PM)
- [ ] Rollback plan and runbook available (Release Manager, Platform Owner)
- [ ] Monitoring & dashboards in place for critical signals (Data Analyst)

Staging validation
- [ ] Deploy to staging succeeded (Platform Owner)
- [ ] Run smoke tests and post-deploy validations (QA, Dev)
- [ ] UX/Accessibility quick check (UX Researcher/Designer)
- [ ] Sign-off from Product (PdM) and Release Manager

Production deployment
- [ ] Final release sign-off (Release Manager - A, PdM - C, PM - R)
- [ ] Execute deployment plan (Platform Owner / Release Manager)
- [ ] Post-deploy smoke tests passed (QA, Dev)
- [ ] Monitoring confirmed (Data Analyst)
- [ ] Announce release to stakeholders and support (PM, Customer Success)

Post-release
- [ ] Monitor for regressions and critical alerts for first 24–72 hours (Platform Owner, Data Analyst)
- [ ] Capture post-release notes and lessons learned (PM)
- [ ] Close any follow-up tasks in backlog
