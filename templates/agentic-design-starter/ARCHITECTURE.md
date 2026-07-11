# ARCHITECTURE.md

## Core architecture

```txt
Figma / reference websites
        ↓
Senior UX planning by Claude
        ↓
Ship Studio scaffold
        ↓
Next.js application
        ├── Sanity content
        ├── Formspark forms
        ├── Resend email
        ├── optional integrations
        └── Vercel deployment
                ↓
              GitHub
```

## Application principles

- Next.js App Router
- TypeScript
- Server Components by default
- Client Components only for genuine interaction
- Sanity as the structured content source
- environment variables for all secrets
- preview deployments for review
- small, reusable components
- design tokens instead of arbitrary styling values

## Suggested application structure

```txt
app/
components/
  ui/
  sections/
  forms/
  integrations/
lib/
  sanity/
  formspark/
  resend/
sanities/
  schemaTypes/
  queries/
types/
styles/
public/
docs/
```

Adapt the structure to the actual project instead of creating empty folders automatically.

## Content architecture

Sanity should own:

- editorial pages
- reusable content
- blog posts
- navigation
- global site settings
- SEO defaults
- social publishing settings when enabled

Code should own:

- design system implementation
- interaction behavior
- validation rules
- integration logic
- security-sensitive configuration

## Forms and email

Formspark receives and stores or forwards form submissions.

Resend handles branded transactional email when required, for example:

- confirmation email to the sender
- internal notification
- double opt-in or workflow messages when legally appropriate

Do not expose Resend or Formspark secrets in client code.

## Optional integrations

Optional modules must be isolated behind clear interfaces so they can be added or removed without destabilizing the core website.
