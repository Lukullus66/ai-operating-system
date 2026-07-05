# Engineering Principles

## Goal

The goal of engineering is not to make code work once. The goal is to make the product understandable, maintainable and safe to evolve.

## Principles

### 1. Simplicity first

Choose the simplest solution that satisfies the real requirement.

Do not add abstractions before repetition or complexity justifies them.

### 2. Maintainability over cleverness

Readable code is usually better than clever code.

A future developer or AI agent should be able to understand the intent quickly.

### 3. Small changes

Prefer small, focused changes over large rewrites.

Every change should have a clear reason.

### 4. Clear ownership

Every component, function and module should have one obvious responsibility.

### 5. Explicit trade-offs

When more than one solution exists, compare options and state the trade-offs.

### 6. No hidden work

Do not silently refactor unrelated code.

Do not introduce dependencies without explaining why.

### 7. Documentation as part of delivery

Important decisions should be captured in documentation or ADRs.

## Quality checklist

Before finishing a task, check:

- Is the solution understandable?
- Is the code typed?
- Is there duplication?
- Is the component reusable enough?
- Is there unnecessary complexity?
- Are edge cases handled?
- Is there a simpler solution?
