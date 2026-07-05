# Prompt Library

## Planning prompt

Use this before any implementation:

```txt
Analyze the current project and create an implementation plan before changing any files.

Include:
- affected files
- proposed architecture
- milestones
- risks
- alternatives
- recommended approach

Wait for approval before implementation.
```

## Refactoring prompt

```txt
Review this code for maintainability. Identify duplication, unclear naming, unnecessary complexity and opportunities to simplify. Do not change behavior unless explicitly approved.
```

## CMS modeling prompt

```txt
Analyze the content requirements and propose a Sanity content model. Do not recreate the old CMS blindly. Separate content, navigation, SEO and presentation concerns.
```

## Migration prompt

```txt
Analyze the legacy Webflow project as a visual and content source. Propose a migration plan to Next.js and Sanity. Preserve SEO, slugs, redirects and core visual identity. Do not copy unnecessary Webflow wrappers.
```

## Review prompt

```txt
Review the implementation against the plan. Check accessibility, performance, SEO, responsiveness, type safety and maintainability. Identify remaining risks.
```
