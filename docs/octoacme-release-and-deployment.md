# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged (Product Owner sign-off)
- Passing CI and security scans (Technical Lead review)
- Release notes drafted (Communications Lead)
- Rollback / mitigation plan documented (Technical Lead + PM)
- Smoke tests prepared and executed (Quality Assurance Lead)

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) - PM
- [ ] Backup or snapshot (if applicable) - Technical Lead
- [ ] Deploy to staging and run smoke tests - QA Lead
- [ ] Deploy to production (automated pipeline preferred) - Technical Lead
- [ ] Run post-deploy verifications - QA Lead
- [ ] Announce release to stakeholders and support - Communications Lead
- [ ] Monitor adoption and feedback (if new feature) - Change Manager

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
