# Next.js Standards

## Defaults

Use:

- App Router
- TypeScript
- Server Components by default
- Client Components only when interactivity requires them
- framework-native image and font optimization

## Architecture

Prefer a structure that makes product features understandable.

Example:

```txt
app/
components/
lib/
sanity/
types/
styles/
```

For larger projects, group feature-specific components close to the feature.

## Rendering

Use server rendering for content-heavy pages.

Use static generation where content changes infrequently.

Use dynamic rendering only when required.

## Data fetching

Keep data access in dedicated functions.

Do not scatter queries throughout components.

Use typed return values.

## Client Components

Use Client Components for:

- forms with client-side state
- menus
- modals
- interactive sliders
- animation triggers

Avoid turning full pages into Client Components unnecessarily.

## Metadata

Use Next.js metadata APIs for:

- title
- description
- canonical URL
- Open Graph
- robots

SEO must be considered before launch.

## Quality checklist

- Are components server-first?
- Is JavaScript minimized?
- Are images optimized?
- Are metadata fields complete?
- Are loading and error states handled?
- Are environment variables documented?
