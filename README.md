# Universal Master Art Library Kit

A Markdown-first, model-neutral image-context and prompt-engineering library.

This repository is designed for use with ChatGPT, Grok, Claude, Midjourney, Flux, SDXL, ComfyUI, and other image-generation workflows.

## Design principles

- One Markdown file per reusable visual context, not one file per isolated prompt.
- Separate image sector knowledge from model-specific prompt syntax.
- Use GitHub as the read-only source of truth.
- Preserve reusable context: purpose, audience, composition, lighting, style, constraints, reference-image rules, and quality checks.
- Add model adapters only at the final prompt-conversion stage.

## Start here

1. Read `INDEX.md`.
2. Select the appropriate sector file.
3. Read the relevant files in `00-core/`.
4. Apply a model adapter from `12-model-adapters/`.
5. Use `13-quality-safety/` to review the final prompt and image.

## Project layout

- `00-core/` — universal image-prompt foundations
- `01-people-portraits/` through `10-art-styles-media/` — sector context libraries
- `11-editing-reference/` — image editing and reference-image workflows
- `12-model-adapters/` — ChatGPT, Grok, Claude, and other platform adaptations
- `13-quality-safety/` — quality, safety, rights, and accessibility checks
- `_templates/` — repeatable Markdown authoring templates
- `examples/` — end-to-end production examples
