# Vercel Deployment Standards

## Goal

Deploy safely, predictably and with clear rollback options.

## Environments

Use separate environments for:

- local development
- preview deployments
- production

## Environment variables

Document every environment variable:

- name
- purpose
- required environment
- example value if safe
- source system

Never commit secrets.

## Deployment flow

Recommended flow:

1. Work on feature branch
2. Open pull request
3. Review preview deployment
4. Check forms, SEO and responsiveness
5. Merge to main
6. Deploy production
7. Verify production URLs

## Pre-launch checklist

- production environment variables set
- domain configured
- redirects configured
- sitemap available
- robots rules checked
- metadata verified
- forms tested
- analytics checked if used
- Sanity dataset configured

## Rollback

Know how to revert to the last working deployment before launch.
