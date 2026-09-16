---
id: electronics-product-photography
title: Electronics Product Photography
sector: product-commerce
tags:
  - electronics
  - product-photography
  - ecommerce
  - product-launch
  - gadget
  - advertising
supported_workflows:
  - text-to-image
  - reference-guided
  - image-to-image
  - product-editing
best_for:
  - ChatGPT
  - Grok
  - Claude
status: stable
---

# Electronics Product Photography

## Purpose

Create accurate, commercially useful images for phones, laptops, storage devices, headphones, cameras, wearables, smart-home products, electronics accessories, and technology campaigns.

When a product reference image is supplied, treat its geometry, ports, buttons, camera layout, materials, finish, color, branding, accessories, and proportions as non-negotiable unless the user explicitly permits a change.

## Production modes

| Mode | Goal | Typical use |
|---|---|---|
| Catalog packshot | Clear product recognition | Marketplace listing, product catalog |
| Premium hero | Desire and innovation | Landing page, launch campaign, keynote |
| Lifestyle scene | Context and buyer benefit | Social ad, ecommerce carousel |
| Feature callout | Explain one capability | Listing slide, product ad |
| Comparison visual | Clarify a difference | Buying guide, review, thumbnail |
| Exploded concept | Explain product architecture conceptually | Deck, education, concept campaign |
| Workspace visual | Show ownership context | Review, creator content, lifestyle campaign |

## Ask before prompting

- What is the exact product or product category?
- Is it a shipping product, prototype, or pure concept?
- Which reference image controls product accuracy?
- Which physical traits must not change: shape, dimensions, ports, buttons, camera layout, colors, finish, logo, screen, packaging, or accessories?
- Is this a packshot, hero, lifestyle image, comparison, callout, or concept?
- What output channel and aspect ratio are required?
- What one feature or buyer benefit must be visually obvious?
- Is the background white, transparent, colored, or environmental?
- Will final text be applied manually?

## Product-fidelity rules

- Use the supplied product reference as the source of truth.
- Do not invent or duplicate cameras, ports, buttons, LEDs, cables, controls, labels, or accessories.
- Do not change color, material, dimensions, screen ratio, keyboard layout, packaging, or branding without explicit direction.
- Do not produce fake specifications, false labels, or unreadable micro-text.
- Label prototype or concept imagery as concept artwork if it could be mistaken for a shipping product.

## Context variables

- `{{product_name}}`
- `{{product_type}}`
- `{{product_status}}`
- `{{primary_feature}}`
- `{{target_customer}}`
- `{{campaign_goal}}`
- `{{reference_invariants}}`
- `{{view_angle}}`
- `{{composition}}`
- `{{background_environment}}`
- `{{lighting}}`
- `{{palette}}`
- `{{materials_finish}}`
- `{{supporting_props}}`
- `{{brand_requirements}}`
- `{{text_safe_area}}`
- `{{aspect_ratio}}`
- `{{must_avoid}}`

## Master product prompt

Create a `{{image_type}}` for `{{product_name}}`, a `{{product_type}}`.

Campaign goal: `{{campaign_goal}}`.
Target customer: `{{target_customer}}`.
Primary feature: `{{primary_feature}}`.

Use the supplied product reference as source of truth.
Preserve exactly: `{{reference_invariants}}`.

View angle: `{{view_angle}}`.
Composition: `{{composition}}`.
Background or environment: `{{background_environment}}`.
Lighting: `{{lighting}}`.
Palette: `{{palette}}`.
Materials and finish: `{{materials_finish}}`.
Supporting props: `{{supporting_props}}`.
Brand requirements: `{{brand_requirements}}`.

Reserve `{{text_safe_area}}` for manually added copy or feature callouts.
Deliver in `{{aspect_ratio}}`.

Avoid `{{must_avoid}}`, incorrect product geometry, extra ports, distorted screens, malformed controls, duplicate products, pseudo-text, fake labels, inaccurate reflections, unintended logos, and physically impossible shadows.

## Catalog packshot template

Create a clean ecommerce catalog packshot of `{{product_name}}`.

Place the product on `{{background_color_surface}}`.
Use `{{view_angle}}` and `{{lighting}}` to show true form, finish, and `{{primary_feature}}`.

Preserve `{{reference_invariants}}` exactly.
Do not include extra accessories unless explicitly specified.

Deliver in `{{aspect_ratio}}` with safe margins for marketplace cropping.
Avoid floating geometry, incorrect ports, strong shadows hiding details, accidental text, and duplicate products.

## Premium launch hero template

Create a premium product-launch hero image for `{{product_name}}`.

Show the product at `{{view_angle}}` in `{{background_environment}}`.
Use `{{composition}}` to emphasize `{{primary_feature}}`.
Use dramatic but physically plausible `{{lighting}}`, realistic `{{materials_finish}}`, controlled reflections, and `{{palette}}`.

Keep `{{text_safe_area}}` clear for the manually added headline.
Preserve `{{reference_invariants}}`.
Deliver in `{{aspect_ratio}}`.
Avoid fake specifications, wrong product geometry, clutter, unreadable UI, excessive effects, and incompatible accessories.

## Lifestyle template

Create a realistic lifestyle image for `{{product_name}}`.

Show `{{target_user}}` using the product in `{{environment}}` for `{{use_case}}`.
Keep the product visible and accurate, especially `{{primary_feature}}`.
Use `{{composition}}`, `{{lighting}}`, and `{{palette}}` to provide believable context.

Preserve `{{reference_invariants}}`.
Avoid incorrect handling, implausible ergonomics, invented UI claims, brand conflicts, distorted hands, and generic stock-image staging.

## Quality-control checklist

- Product silhouette and proportion are accurate.
- Product count is correct.
- Cameras, ports, buttons, keys, controls, cables, and accessories are accurate.
- Materials, reflections, shadows, and screens are physically plausible.
- The product is readable at target display size.
- Text-safe areas remain clear.
- No pseudo-text, fake claims, malformed geometry, impossible reflections, or unwanted brand marks appear.
- Human hands and interactions are plausible in lifestyle scenes.

## Final output format

1. Product visual objective
2. Reference-fidelity statement
3. Final image prompt
4. Preserve exactly
5. Avoid
6. Suggested aspect ratio and crop
7. Manual post-production notes
8. Quality-control review
