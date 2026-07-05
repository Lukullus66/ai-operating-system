# Component Rules

## Purpose

Components are the foundation of maintainable frontend work.

A good component is reusable enough to be useful, but not so abstract that it becomes hard to understand.

## Component principles

Components should be:

- focused
- composable
- accessible
- responsive
- typed
- content-flexible
- visually consistent

## Naming

Use names that describe purpose, not appearance.

Good:

- `ProjectCard`
- `ServiceOverview`
- `TestimonialList`
- `ContactForm`

Weak:

- `BlueBox`
- `Section3`
- `BigCard`
- `LeftThing`

## Props

Props should be explicit and typed.

Avoid passing large unstructured objects unless the object is a clear domain model.

## Composition

Prefer composition over too many variants.

If a component has too many boolean props, split it.

## Accessibility

Components must preserve:

- semantic HTML
- keyboard support
- focus states
- heading structure
- alt text where relevant

## AI prompt

```txt
Analyze these sections and propose a reusable component model. Identify shared patterns, props, accessibility concerns and where content should come from Sanity. Wait for approval before implementation.
```
