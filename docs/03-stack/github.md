# GitHub Workflow

## Purpose

GitHub is the source of truth for project history, collaboration and review.

## Branching

Use branches for meaningful work:

- `main` for production-ready state
- `feature/...` for new work
- `fix/...` for bug fixes
- `docs/...` for documentation

## Commits

Commits should be small and intentional.

Good:

```txt
feat: add Sanity project schema
fix: preserve canonical metadata on project pages
docs: add migration checklist
```

Weak:

```txt
update
changes
fix stuff
```

## Pull requests

Every non-trivial change should include:

- summary
- changed areas
- screenshots if visual
- testing notes
- risks
- follow-up tasks

## AI review

Use Codex for targeted PR review.

Prompt:

```txt
Review this PR for bugs, regressions, type safety, accessibility, SEO and unnecessary complexity. Keep suggestions focused and actionable.
```

## Protecting main

For client or production projects, use:

- pull requests
- required review
- preview deployment checks
- protected main branch

## Release discipline

Do not merge when:

- environment variables are missing
- redirects are untested
- forms are untested
- SEO metadata is incomplete
- build fails
