# Performance Principles

## Goal

Fast websites feel better, rank better and convert better.

Performance is a design and architecture concern, not just an optimization phase.

## Priorities

- minimize JavaScript
- optimize images
- optimize fonts
- reduce layout shift
- cache content intelligently
- avoid unnecessary client rendering
- lazy load non-critical content

## Core Web Vitals

Monitor:

- Largest Contentful Paint
- Interaction to Next Paint
- Cumulative Layout Shift

## Images

Use responsive image sizes.

Prefer modern formats.

Always define dimensions or reserve space.

## Fonts

Use few font families and weights.

Avoid blocking rendering where possible.

## JavaScript

Client-side JavaScript should be justified.

If content can render on the server, render it on the server.

## Review checklist

- Is the page server-first?
- Are images optimized?
- Are fonts optimized?
- Is animation lightweight?
- Is third-party JavaScript necessary?
- Is there layout shift?
