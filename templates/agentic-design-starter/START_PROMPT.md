# START_PROMPT.md

Use this prompt when starting a new project in Claude Code or Ship Studio.

```txt
Read the following files before doing anything:

- CLAUDE.md
- PROJECT.md
- ARCHITECTURE.md
- MODULES.md
- REFERENCE_SITES.md
- INTEGRATIONS.md

Act first as a senior UX designer and product strategist, then as a senior frontend architect.

Do not write code yet.

Phase 1:
1. Summarize the business goal and target audience.
2. Identify missing or weak project information.
3. Analyze the approved reference websites and extract transferable design principles without copying their branding, text, imagery or complete layouts.
4. Propose information architecture and primary user journeys.
5. Propose page structure and reusable component families.
6. Propose the Sanity content model.
7. Explain how Formspark, Resend, Vercel and GitHub fit into the architecture.
8. Evaluate the optional modules selected in MODULES.md.
9. Identify risks and dependencies.
10. Create a milestone-based implementation plan.

Stop after the plan and wait for explicit approval.

After approval, implement one milestone at a time. At the end of every milestone, explain what changed, which files were modified, how the result was verified and what remains.
```

## Ship Studio project kickoff

When Ship Studio is used to generate the initial codebase, add:

```txt
Treat Ship Studio output as a starting point. Preserve the approved design direction, but review all generated code for semantic HTML, accessibility, responsive behavior, component reuse, performance and compatibility with the planned Sanity content model.
```
