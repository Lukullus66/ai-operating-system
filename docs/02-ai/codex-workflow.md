# Codex Workflow

## Purpose

Codex is best used for focused code changes, reviews, debugging, tests and simplification.

Codex should not replace architecture planning.

## Best use cases

Use Codex for:

- reviewing a pull request
- fixing a specific bug
- improving type safety
- simplifying a component
- writing tests
- checking edge cases
- identifying dead code

## Workflow

### 1. Give narrow context

Codex performs best with a clear, bounded task.

Include:

- exact goal
- relevant files
- expected behavior
- constraints
- what must not change

### 2. Ask for review before change

For non-trivial changes, ask Codex to inspect and report first.

### 3. Apply small patches

Prefer small, reviewable changes.

### 4. Verify

Codex should explain how to verify the result.

## Codex review checklist

Ask Codex to check:

- correctness
- type safety
- error handling
- edge cases
- unnecessary complexity
- performance regressions
- accessibility regressions
- SEO regressions

## Good Codex prompt

```txt
Review the changed files in this PR. Focus on bugs, type safety, unnecessary complexity and regressions. Do not propose a full redesign unless the current approach is fundamentally broken.
```

## Anti-patterns

Avoid asking Codex to:

- redesign the whole architecture without context
- rewrite large parts of the app in one pass
- introduce dependencies casually
- change visual design without a design brief
