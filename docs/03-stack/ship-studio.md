# Ship Studio Workflow

## Purpose

Ship Studio is used to accelerate the initial transition from visual design to a working Next.js codebase.

It is a starting point, not the final architecture.

## Rules

Generated code must be reviewed before production use.

Do not assume generated components are:

- reusable
- accessible
- optimized
- semantically correct
- aligned with the final CMS model

## Recommended process

1. Generate or scaffold the initial project.
2. Commit the raw output.
3. Review structure and dependencies.
4. Identify reusable sections.
5. Convert repeated patterns into components.
6. Replace hardcoded content with Sanity data.
7. Remove unnecessary wrappers and styles.
8. Validate responsiveness.
9. Validate accessibility.
10. Validate performance.

## What to preserve

Preserve:

- visual direction
- spacing rhythm
- typographic hierarchy
- important interactions
- responsive intent

## What to improve

Improve:

- component naming
- prop structure
- semantic HTML
- CMS integration
- image handling
- SEO metadata
- accessibility
- maintainability

## AI prompt

```txt
Analyze this Ship Studio output. Identify what should remain, what should be refactored, and how to convert the generated sections into reusable Next.js components connected to Sanity. Do not edit files until the plan is approved.
```
