# INTEGRATIONS.md

## Formspark

Use Formspark for reliable form submission handling when a custom backend is not required.

Requirements:

- server-side or protected submission strategy where appropriate
- validation
- loading, success and error states
- spam protection
- hidden context fields
- privacy review

## Resend

Use Resend for transactional email only.

Typical use cases:

- internal form notification
- sender confirmation
- account or workflow email

Requirements:

- verified sending domain
- reusable email templates
- environment variables
- clear sender and reply-to behavior
- error logging

## Sanity

Sanity is the editorial source of truth.

Requirements:

- content model planned before implementation
- editor-friendly labels and previews
- reusable SEO object
- global navigation and settings
- preview workflow when required

## Instagram

Treat Instagram as an optional external content source.

Do not make critical content dependent on its availability.

Prefer curated content and cached server-side retrieval over heavy client-side widgets.

## Automatic social publishing

Preferred event flow:

```txt
Sanity publish event
  -> webhook
  -> authenticated route or workflow
  -> channel adapter
  -> publish
  -> store status and external post ID
```

Each blog post should support:

- publish to social toggle
- per-channel copy override
- image selection
- publication status
- error message
- external post URL or ID

## Facebook

Automatic publishing should target a Facebook Page, not a personal profile.

Tokens, permissions, review requirements and API limits must be verified during implementation.

## Relume React

Relume React components may be imported or adapted as accelerators.

They must be aligned with:

- project design tokens
- approved UX structure
- Sanity content model
- accessibility requirements
- selected styling architecture

Do not let the component library determine the product strategy.
