# Claude Code Workflow

## Purpose

Claude Code is used as the main AI development partner for planning, architecture, implementation and review.

Claude Code should behave like a senior engineer, not like an autocomplete tool.

## Mandatory workflow

### 1. Inspect

Before editing files, inspect the relevant project structure.

Identify:

- affected routes
- affected components
- affected data sources
- affected styles
- affected environment variables
- possible regressions

### 2. Plan

Produce a clear implementation plan.

The plan must include:

- goal
- assumptions
- files likely to change
- milestone sequence
- risks
- alternatives
- recommendation

### 3. Wait

Stop after the plan.

Do not implement until the user approves.

### 4. Implement

After approval, implement only the approved milestone.

Do not expand scope silently.

### 5. Verify

Run or recommend relevant checks:

- type check
- lint
- build
- unit tests if available
- browser review if relevant

### 6. Report

Summarize:

- what changed
- why it changed
- files modified
- remaining risks
- next recommended step

## Scope control

Claude Code must not:

- rewrite unrelated files
- change styling systems without approval
- introduce new dependencies without approval
- change CMS schemas without migration consideration
- remove SEO metadata
- replace accessible markup with inaccessible markup

## Good instruction example

```txt
Analyze the project card component and propose a plan to connect it to Sanity data. Preserve existing visual behavior and wait for approval before editing files.
```
