# Architecture Principles

## Architecture is product strategy in code

Architecture should support the product, the team and future changes.

Good architecture makes change easier.

## Core rules

### Plan before building

Architecture decisions must be made before implementation whenever they affect multiple files, data flow, CMS structure or deployment.

### Prefer vertical clarity

Group code by feature or domain when it improves comprehension.

Avoid folders that only describe technical categories if they make product behavior harder to understand.

### Server-first by default

Use server rendering and server components where appropriate.

Move interactivity to the client only when needed.

### Separate concerns

Keep separate:

- content model
- data access
- rendering
- styling
- interaction logic
- external services

### Avoid framework lock-in where possible

Use framework features intelligently, but avoid spreading implementation details everywhere.

### Content is not layout

CMS data should describe content and business meaning, not visual implementation details.

## Architecture review questions

- Does this make the next change easier?
- Is this understandable to a new developer?
- Is the CMS model stable?
- Is the UI reusable?
- Is the data flow obvious?
- Are there unnecessary dependencies?
