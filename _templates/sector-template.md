# Markdown Context File Template

---
id: replace-with-kebab-case-id
title: Replace With Human-Readable Title
sector: replace-with-sector
tags:
  - image-generation
  - replace-with-tag
supported_workflows:
  - text-to-image
  - reference-guided
best_for:
  - ChatGPT
  - Grok
  - Claude
status: draft
---

# Replace With Human-Readable Title

## Purpose

State the production problem this context file solves.

## Best uses

- Use case one
- Use case two
- Use case three

## Ask before prompting

- What is the image meant to achieve?
- Who is the audience?
- What output format and aspect ratio are needed?
- Which elements must be accurate?
- Is a reference image required?
- What should not be included?

## Context variables

- `{{subject}}`
- `{{objective}}`
- `{{audience}}`
- `{{environment}}`
- `{{composition}}`
- `{{camera}}`
- `{{lighting}}`
- `{{palette}}`
- `{{style}}`
- `{{aspect_ratio}}`
- `{{constraints}}`

## Universal visual brief template

Create a {{image_type}} featuring {{subject}} for {{audience}}.

Objective: {{objective}}.
Composition: {{composition}}.
Camera: {{camera}}.
Environment: {{environment}}.
Lighting: {{lighting}}.
Palette: {{palette}}.
Style: {{style}}.
Output: {{aspect_ratio}}.

Preserve: {{non_negotiable_details}}.
Avoid: {{negative_constraints}}.

## Reference-image mode

State exactly which supplied visual traits are source-of-truth and which are permitted to change.

## Quality checklist

- The image fulfills the stated objective
- The focal point is unambiguous
- The composition fits the intended delivery channel
- Required details are present and correct
- Excluded elements do not appear
- Lighting, scale, perspective, and style are coherent
