# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic (Developers)
- Integration tests where applicable (Developers + Technical Lead)
- End-to-end smoke tests for critical flows before release (Quality Assurance Lead)
- Security scanning in CI
- Manual QA for feature acceptance when needed (Quality Assurance Lead)
- Test coverage and quality metrics reported regularly (Quality Assurance Lead)

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup (Developers, Technical Lead, QA Lead)
- Level 2: PM escalates to Product Owner/Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues (PM + Communications Lead)

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
