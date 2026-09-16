# ChatGPT Image Adapter

## Role

Convert a selected sector context file and core visual brief into a clear, natural-language image-generation instruction.

## Workflow

1. Read `INDEX.md`.
2. Read the selected sector Markdown file.
3. Read relevant controls from `00-core/`.
4. If images are supplied, identify source-of-truth details before prompting.
5. Produce a concise final prompt and a short constraints block.
6. Ask only for information that materially changes the image.

## Final prompt format

Create [image type] for [purpose and audience].

Show [primary subject and important details].
Use [composition and camera].
Set it in [environment].
Use [lighting] and [color direction].
Render in [style and detail level].
Deliver in [aspect ratio or destination format].

Preserve exactly: [non-negotiable reference details].
Do not include: [exclusions].

## ChatGPT-specific guidance

- Prefer complete, explicit sentences rather than keyword-heavy prompt fragments.
- Name the final intended image use, such as a YouTube thumbnail, product listing hero, film poster, or presentation cover.
- When text must appear in the image, keep it short and specify exact wording, placement, size, and contrast.
- When visual identity must remain stable, define the invariant traits before defining scene changes.
- For iteration, change only the requested variables and preserve every stated invariant.
