# Sanity Standards

## Principle

Sanity is the source of truth for structured content.

It should model meaning, not layout implementation.

## Do not recreate legacy CMS blindly

Before building schemas, analyze:

- content types
- editorial workflows
- reusable blocks
- global settings
- SEO fields
- navigation
- localization needs

## Recommended document types

Common starting point:

- `page`
- `post`
- `project`
- `service`
- `person`
- `testimonial`
- `navigation`
- `siteSettings`
- `seo`

## Content vs presentation

Good field:

- `headline`
- `intro`
- `slug`
- `featuredImage`
- `relatedServices`

Weak field:

- `leftColumnText`
- `blueCardHeadline`
- `section3Button`

Presentation-specific naming makes future redesigns harder.

## SEO

Every indexable document should support:

- meta title
- meta description
- canonical override if needed
- Open Graph image
- robots settings if needed

## Editorial experience

Schemas should be understandable for non-technical editors.

Use clear titles, descriptions, validation and previews.

## Migration checklist

- Map old fields to new fields
- Identify duplicate content
- Normalize inconsistent naming
- Preserve slugs
- Preserve image alt text where available
- Preserve publish dates where relevant
