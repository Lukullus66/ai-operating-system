# Context Engineering

## Purpose

AI-assisted development works best when the model receives the right context, constraints and decision history.

Context engineering is the practice of preparing that information deliberately.

## Required context for every task

Before asking an AI agent to implement, provide:

- business goal
- affected page or feature
- existing architecture
- design intent
- content model if relevant
- constraints
- acceptance criteria
- what must not change

## Bad prompt

Build the page.

## Better prompt

Analyze the current project structure and propose a plan to implement the new landing page using existing components where possible. Preserve SEO metadata, avoid unrelated refactors and wait for approval before implementation.

## Context hierarchy

Use this order:

1. Project rules
2. Architecture decisions
3. Feature requirements
4. Design references
5. Existing code
6. Acceptance criteria

## Context hygiene

Remove outdated instructions.

Do not mix conflicting requirements.

Keep project-specific rules in `PROJECT.md` and general rules in `CLAUDE.md` or `AGENTS.md`.

## Agent memory files

Recommended files:

- `CLAUDE.md`
- `AGENTS.md`
- `PROJECT.md`
- `docs/05-project/decisions.md`
- `docs/05-project/todo.md`
