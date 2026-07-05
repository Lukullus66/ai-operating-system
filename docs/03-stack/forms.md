# Forms Workflow

## Purpose

Forms must be reliable, accessible and easy to maintain.

A form is not complete when it submits. It is complete when the user clearly understands what happened.

## Recommended approaches

Use one of:

- Formspark for simple marketing forms
- Next.js server actions for framework-native handling
- route handlers for custom backend logic
- external CRM or automation tools when required

## Required states

Every form must include:

- default state
- validation state
- loading state
- success state
- error state
- spam protection strategy

## Accessibility

Forms must have:

- visible labels or accessible labels
- useful error messages
- keyboard support
- correct input types
- focus states
- logical tab order

## Validation

Validate:

- required fields
- email fields
- phone fields if used
- consent fields if required
- hidden contextual fields

Prefer server-side validation even when client-side validation exists.

## Hidden fields

Useful hidden fields:

- page URL
- page title
- form name
- campaign source
- selected product or service

## AI prompt

```txt
Analyze this form and propose a reliable implementation plan. Include validation, loading state, success state, error state, spam protection and accessibility. Wait for approval before editing files.
```
