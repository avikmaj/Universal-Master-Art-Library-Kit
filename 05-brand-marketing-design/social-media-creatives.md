---
id: social-media-creatives
title: Social Media Creatives
sector: brand-marketing-design
tags:
  - social-media
  - marketing
  - campaign
  - instagram
  - linkedin
  - youtube
  - tiktok
  - brand
supported_workflows:
  - text-to-image
  - reference-guided
  - image-editing
  - campaign-variation
best_for:
  - ChatGPT
  - Grok
  - Claude
status: stable
---

# Social Media Creatives

## Purpose

Create campaign-driven social visuals for organic content, announcements, launches, educational carousels, creator branding, events, recruitment, product promotion, and short-form cover images.

Start with audience, campaign objective, and one memorable message—not aesthetics alone.

## Campaign-first principle

Define these before prompting:

1. Target audience
2. Campaign objective
3. Single message
4. Visual proof
5. Platform format
6. Brand rules
7. Safe areas for manual typography and CTA overlays

## Ask before prompting

- Which platform and format are required?
- Is the objective awareness, engagement, education, click-through, lead generation, conversion, community, recruiting, or launch visibility?
- Who is the target audience?
- What one message should they remember?
- What product, person, character, event, offer, data point, or story moment must be central?
- What brand colors, typography, logo treatment, and visual rules are mandatory?
- Will final copy be added manually?
- What safe zones and aspect ratio are required?
- Which references control product, identity, character, or brand accuracy?

## Visual hierarchy

| Priority | Requirement |
|---|---|
| 1 | One dominant focal point or message |
| 2 | Clear subject-background contrast |
| 3 | Visual proof: product, person, result, setting, or data concept |
| 4 | Short supporting element only when necessary |
| 5 | Brand treatment that supports clarity rather than overwhelming it |

## Context variables

- `{{platform}}`
- `{{format}}`
- `{{aspect_ratio}}`
- `{{campaign_name}}`
- `{{campaign_objective}}`
- `{{target_audience}}`
- `{{single_message}}`
- `{{call_to_action}}`
- `{{primary_subject}}`
- `{{visual_proof}}`
- `{{composition}}`
- `{{background}}`
- `{{lighting}}`
- `{{palette}}`
- `{{brand_invariants}}`
- `{{copy_strategy}}`
- `{{safe_areas}}`
- `{{reference_invariants}}`
- `{{must_avoid}}`

## Master social visual prompt

Create a `{{format}}` social-media visual for `{{platform}}`.

Campaign: `{{campaign_name}}`.
Objective: `{{campaign_objective}}`.
Audience: `{{target_audience}}`.
Single message: `{{single_message}}`.
Call to action: `{{call_to_action}}`.

Primary subject: `{{primary_subject}}`.
Visual proof: `{{visual_proof}}`.
Composition: `{{composition}}`.
Background: `{{background}}`.
Lighting: `{{lighting}}`.
Palette: `{{palette}}`.

Apply brand invariants: `{{brand_invariants}}`.
Copy strategy: `{{copy_strategy}}`.
Keep `{{safe_areas}}` clear for platform UI, final typography, logo, or CTA.

Deliver in `{{aspect_ratio}}`.
Preserve: `{{reference_invariants}}`.
Avoid: `{{must_avoid}}`, clutter, tiny text, pseudo-text, generic stock imagery, off-brand colors, unsupported claims, distorted anatomy, and accidental logos.

## Platform formats

| Platform use | Recommended format | Direction |
|---|---|---|
| Instagram feed | 4:5 or 1:1 | Strong first impression; large subject; avoid tiny details |
| Instagram carousel | 4:5 | Maintain visual continuity; every slide must still stand alone |
| Story or Reel cover | 9:16 | Keep essential elements centered; account for platform UI |
| TikTok cover | 9:16 | Central subject, bold hook, editable overlay text |
| YouTube community post | 1:1 or 16:9 | One announcement or discussion hook |
| LinkedIn post | 1.91:1 or 4:5 | Clear, credible, restrained professional hierarchy |
| X post | 16:9 | Immediate news or discussion value |
| Pinterest pin | 2:3 | Vertical composition with instructional or aspirational proof |

## Brand announcement template

Create a `{{format}}` announcement visual for `{{brand_or_channel}}`.

Communicate `{{single_message}}` to `{{target_audience}}`.
Feature `{{primary_subject}}` as the visual proof.
Use `{{composition}}`, `{{lighting}}`, and `{{palette}}`.
Keep `{{safe_areas}}` clear for final headline, date, and CTA added manually.
Maintain `{{brand_invariants}}`.
Deliver in `{{aspect_ratio}}`.
Avoid fake logos, unreadable text, clutter, and unverified claims.

## Educational carousel template

Create an educational carousel-cover image for `{{topic}}`.

Audience: `{{target_audience}}`.
Core benefit: `{{single_message}}`.
Use one understandable visual metaphor: `{{visual_proof}}`.
Feature `{{primary_subject}}` with high contrast and simple composition.
Reserve `{{safe_areas}}` for a manual headline.
Use `{{palette}}` and `{{brand_invariants}}`.
Avoid dense text, small labels, complex diagrams, and vague abstractions.

## Product campaign template

Create a social campaign visual for `{{product_name}}`.

Objective: `{{campaign_objective}}`.
Main benefit: `{{single_message}}`.
Show `{{primary_subject}}` and demonstrate `{{visual_proof}}`.
Use `{{composition}}`, `{{lighting}}`, and `{{palette}}`.
Preserve product and brand reference rules: `{{reference_invariants}}`.
Keep `{{safe_areas}}` clear for manual headline and CTA.
Avoid invented specifications, misleading effects, distorted product geometry, and accidental text.

## Text and copy rules

Generate the visual foundation first. Add exact titles, dates, legal copy, prices, CTAs, and fine typography manually in a design editor whenever accuracy matters.

If text must appear in-image:

- Use exact approved wording.
- Keep it short.
- Specify placement, contrast, and hierarchy.
- Verify spelling before publication.
- Do not create factual claims the user has not supplied.

## Brand and rights safeguards

- Preserve approved brand assets; do not invent logos.
- Do not imply endorsements, awards, certifications, partnerships, statistics, or results that were not supplied.
- Use authorized references for people, products, marks, and characters.
- Distinguish concept imagery from literal photography when context requires it.

## Quality-control checklist

- A viewer understands the core message quickly.
- One dominant focal point exists.
- The layout fits the target platform.
- Safe areas are clear.
- The creative is recognizably on-brand.
- References are accurate.
- No pseudo-text, tiny labels, distorted anatomy, or unsupported claims appear.
- The image remains readable at mobile size.

## Final output format

1. Campaign objective
2. Single-message takeaway
3. Visual concept
4. Final image prompt
5. Recommended manual overlay copy
6. Format and safe areas
7. Preserve exactly
8. Avoid
9. Platform adaptation notes
10. Quality-control review
