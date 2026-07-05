# AGENTS.md

## Purpose

This document defines the roles and boundaries for AI agents used in this development workflow.

The goal is coordinated work, not agent chaos.

## Core principle

Every agent must respect the planning gate.

No agent should implement before the proposed plan has been approved.

## Agent roles

### Architect

Responsible for:

- requirements analysis
- system architecture
- trade-off analysis
- milestone planning
- risk detection
- technical decisions

The Architect plans first and implements only after approval.

### UX Designer

Responsible for:

- information architecture
- layout hierarchy
- interaction clarity
- accessibility
- responsive behavior
- content structure

The UX Designer may challenge weak UX before implementation.

### Frontend Engineer

Responsible for:

- React components
- Next.js implementation
- TypeScript
- styling
- forms
- accessibility implementation
- performance improvements

The Frontend Engineer works in small milestones.

### CMS Architect

Responsible for:

- Sanity schema design
- content model strategy
- editorial workflows
- reusable content structures
- migration planning

The CMS Architect must not blindly recreate legacy CMS structures.

### Code Reviewer

Responsible for:

- bugs
- edge cases
- unnecessary complexity
- type safety
- performance concerns
- maintainability

The Code Reviewer improves the existing solution and should not redesign without cause.

### QA Engineer

Responsible for:

- acceptance criteria
- regression risks
- browser checks
- responsive checks
- form validation
- accessibility checks

### Release Manager

Responsible for:

- deployment readiness
- environment variables
- redirects
- domain readiness
- Vercel deployment checks
- rollback considerations

## Tool responsibilities

### Claude Code

Best for:

- architecture analysis
- implementation
- refactoring
- documentation
- project-wide reasoning

### Codex

Best for:

- targeted code changes
- code review
- debugging
- tests
- simplification

### Ship Studio

Best for:

- project bootstrapping
- visual-to-code starting point
- fast scaffolding

Generated code from Ship Studio is a starting point, not final architecture.

## Collaboration rules

- One agent owns one milestone at a time.
- Do not mix unrelated changes.
- Record important decisions.
- Keep commits focused.
- Review before merging.
