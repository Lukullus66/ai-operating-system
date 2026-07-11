# MODULES.md

Select optional modules before implementation.

## Core modules

These are part of the standard project foundation.

- [x] Next.js App Router
- [x] TypeScript
- [x] Sanity CMS
- [x] Vercel deployment
- [x] GitHub workflow
- [x] Formspark form delivery
- [x] Resend transactional email

## Optional: multilingual website

- [ ] Enabled

Decide before implementation:

- locales
- default locale
- URL strategy
- translated slugs
- fallback behavior
- Sanity translation model
- localized metadata
- hreflang strategy

Do not bolt multilingual support onto a finished architecture without review.

## Optional: Instagram content

- [ ] Enabled

Possible approaches:

- editorially selected Instagram posts stored in Sanity
- server-side retrieval through an approved API
- embeds for a small number of posts

Requirements:

- graceful failure when external data is unavailable
- no critical layout dependency on Instagram
- privacy and performance review
- caching strategy

## Optional: automatic social publishing

- [ ] Enabled

Target channels:

- [ ] Facebook Page
- [ ] Instagram
- [ ] LinkedIn
- [ ] Other:

Trigger:

- new Sanity blog post becomes published

Recommended architecture:

Sanity webhook -> secure Next.js route or automation service -> channel API -> delivery log

Requirements:

- manual opt-out per post
- channel-specific text fields or templates
- retry and error logging
- no duplicate publishing
- secure token storage
- preview or approval workflow when appropriate

## Optional: Relume React components

- [ ] Enabled

Rules:

- use Relume components as structured starting points
- adapt them to the project's design tokens and content model
- do not preserve unnecessary demo content or styling
- review semantics, accessibility and responsiveness
- avoid mixing incompatible styling conventions without a plan

## Optional module approval

Claude must explain architectural consequences before enabling a module.
