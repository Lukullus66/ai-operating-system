# Webflow to Headless Migration

## Purpose

Use this guide only for existing Webflow projects that are being migrated away from Webflow.

Webflow is the visual and content source. It is not the target architecture.

## Goals

- preserve visual quality
- preserve SEO value
- preserve useful content
- improve technical architecture
- replace Webflow CMS with Sanity
- replace platform-specific forms and interactions

## Migration order

1. Audit the existing Webflow project
2. Document pages, templates and CMS collections
3. Export or document assets
4. Map URLs, slugs and redirects
5. Design the new Sanity content model
6. Build reusable Next.js components
7. Import content into Sanity
8. Replace forms
9. Rebuild critical interactions
10. Test SEO, responsiveness and performance
11. Deploy to Vercel
12. Switch domain only after QA

## Do not copy blindly

Avoid recreating:

- unnecessary wrapper divs
- layout-specific CMS fields
- Webflow interaction complexity
- duplicated sections
- platform-specific form logic

## CMS migration

Analyze each Webflow Collection:

- What content type does it represent?
- Is it still needed?
- Should it merge with another type?
- Which fields are editorial?
- Which fields are only presentation?
- Which fields belong to SEO?

## SEO checklist

- preserve high-value URLs
- create redirects for changed URLs
- preserve titles and descriptions where useful
- preserve image alt text where available
- generate sitemap
- test canonical URLs

## Form migration

Replace Webflow forms with:

- Formspark
- Next.js server actions
- route handlers
- another explicit backend

Always include validation, loading, success and error states.
