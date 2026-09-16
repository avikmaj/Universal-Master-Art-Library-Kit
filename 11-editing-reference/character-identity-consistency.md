---
id: character-identity-consistency
title: Character Identity Consistency
sector: editing-reference
tags:
  - character-consistency
  - identity-preservation
  - reference-image
  - ai-film
  - editing
  - continuity
supported_workflows:
  - reference-guided
  - image-to-image
  - character-bible
  - multi-scene-continuity
best_for:
  - ChatGPT
  - Grok
  - Claude
  - Midjourney
  - Flux
  - ComfyUI
status: stable
---

# Character Identity Consistency

## Purpose

Preserve an original recurring fictional character's identity across AI-generated images, film frames, thumbnails, posters, social creatives, concept art, and scene variations.

Character consistency is a production-continuity system, not only a face-description problem. Stable results require documented identity invariants, controlled scene variables, reference hierarchy, wardrobe/prop continuity, and repeatable QC.

## Core rule

Before changing pose, expression, shot, lighting, setting, action, costume variation, or time period, explicitly lock what must remain unchanged.

Each prompt must distinguish:

- Identity invariants: defining traits that remain stable
- Scene variables: traits allowed to change
- Reference sources: images or documents controlling each category
- Prohibited drift: changes requiring explicit approval

## Character identity record

```md
# Character: {{character_name}}

## Narrative role
{{role_in_story}}

## Identity invariants
- Apparent age range: {{age_range}}
- Face shape: {{face_shape}}
- Skin tone and undertone: {{skin_tone}}
- Eye color and shape: {{eyes}}
- Nose, lips, jaw, and facial structure: {{facial_structure}}
- Hair color, texture, length, parting, and signature style: {{hair}}
- Body and silhouette: {{body_silhouette}}
- Distinguishing marks: {{marks}}
- Default physical presence: {{body_language}}
- Personality continuity: {{personality}}

## Signature wardrobe and accessories
- {{signature_item_1}}
- {{signature_item_2}}
- {{signature_item_3}}

## Approved variables
- Pose
- Expression
- Camera angle
- Lens character
- Lighting
- Location
- Time of day
- Weather
- Approved scene-appropriate wardrobe changes

## Prohibited drift
- {{prohibited_change_1}}
- {{prohibited_change_2}}
- {{prohibited_change_3}}

## Authoritative references
- Face: {{face_reference}}
- Full body: {{body_reference}}
- Wardrobe: {{wardrobe_reference}}
- Color: {{color_reference}}
- Props: {{prop_reference}}
```

## Ask before prompting

- Is this an original fictional character, an authorized person, or a real public figure?
- Which reference controls facial identity?
- Which reference controls body proportions, costume, accessories, and color?
- What traits are invariant?
- What may change in this scene?
- Is the character a one-off visual or part of a continuing series?
- Are there approved age states, disguises, transformations, injuries, or costume phases?
- What scene, emotion, action, shot type, and lighting are needed?
- Which previous or next frame must remain continuous?

## Reference hierarchy

Use this priority unless the user gives another order:

1. Approved character identity sheet
2. Face reference
3. Full-body reference
4. Wardrobe and accessory reference
5. Previously approved scene frame
6. New scene direction

When sources conflict, ask which reference controls. Never silently merge incompatible traits.

## Invariants and variables

| Category | Usually invariant | Usually allowed to change |
|---|---|---|
| Face | Bone structure, eye shape, nose, lips, skin tone, marks | Expression, gaze, minor scene makeup |
| Hair | Color, texture, length, signature style | Wind, wetness, approved styling |
| Body | Height impression, build, silhouette, posture pattern | Pose, perspective, scene clothing |
| Wardrobe | Signature palette, key accessory, uniform logic | Approved clothing appropriate to scene |
| Props | Iconic object geometry, color, placement logic | Whether held, carried, or visible |
| Personality | Baseline physical and emotional presence | Moment-specific reaction |
| World | Era, setting, production-design rules | New locations inside the established world |

## Master identity-preservation prompt

Use the supplied character references as the authoritative source of truth for `{{character_name}}`.

Preserve exactly:

- Facial identity: `{{facial_identity_invariants}}`
- Skin tone and marks: `{{skin_marks}}`
- Hair: `{{hair_invariants}}`
- Body and silhouette: `{{body_invariants}}`
- Signature wardrobe and accessories: `{{wardrobe_invariants}}`
- Character presence: `{{personality_posture}}`

Create a scene where `{{character_name}}` is `{{scene_action}}` in `{{location}}`.

Narrative context: `{{story_beat}}`.
Emotion: `{{emotional_state}}`.
Shot: `{{shot_type}}`, `{{camera_angle}}`, `{{lens_character}}`.
Composition: `{{composition}}`.
Lighting: `{{lighting}}`.
Palette: `{{palette}}`.
Output: `{{aspect_ratio}}`.

Allowed changes: `{{allowed_scene_changes}}`.

Do not alter apparent age, facial structure, hairstyle identity, skin tone, body silhouette, signature accessories, wardrobe logic, or any reference-defined traits. Avoid identity drift, face swapping, inconsistent eyes, distorted anatomy, extra limbs, duplicate characters, random jewelry, unwanted text, and unintended logos.

## Scene-to-scene continuity prompt

Create the next image in a continuous visual sequence.

Previous approved frame: `{{previous_frame_summary}}`.
New story beat: `{{new_story_beat}}`.

Maintain:

- Identity: `{{identity_invariants}}`
- Wardrobe state: `{{wardrobe_state}}`
- Prop state: `{{prop_state}}`
- Environment and time: `{{environmental_continuity}}`
- Lighting/palette progression: `{{color_lighting_continuity}}`
- Screen direction and blocking: `{{screen_direction}}`

Change only: `{{scene_change}}`.

Use `{{shot_type}}` and `{{composition}}`.
Deliver in `{{aspect_ratio}}`.
Avoid any unwanted continuity changes.

## Multi-character prompt

Create a scene with `{{character_a}}` and `{{character_b}}`.

Character A must preserve: `{{character_a_invariants}}`.
Character B must preserve: `{{character_b_invariants}}`.

Interaction: `{{interaction}}`.
Location: `{{location}}`.
Composition: `{{composition}}`.
Shot/lens: `{{shot_type}}`, `{{lens_character}}`.
Lighting and palette: `{{lighting}}`, `{{palette}}`.

Keep both identities distinct. Do not blend faces, swap wardrobes, merge limbs, duplicate people, or add unapproved extra characters.

## Identity-drift diagnosis

| Failure | Likely reason | Correction |
|---|---|---|
| Face changes across images | Identity description or reference priority is unclear | Lock facial structure, hair, skin, marks, and primary face reference |
| Wardrobe changes unexpectedly | Signature items are not locked | Specify garment, color, material, and accessories |
| Character looks older or younger | Age range is missing | Lock apparent age range and prohibit age drift |
| Body proportions shift | Full-body reference is absent | Add silhouette constraints and a full-body reference |
| Characters blend together | Separate identity blocks are missing | Define every character independently |
| Scene continuity fails | Prior-frame anchors are absent | State costume, props, lighting, screen direction, and location |
| Style overwhelms identity | Reference roles are not separated | Declare whether each reference controls identity, style, composition, or product fidelity |

## Quality-control checklist

- Face shape, eyes, nose, lips, skin tone, hair, and marks match the approved profile.
- Apparent age is within the approved range.
- Body silhouette, posture, costume, accessories, and props remain correct.
- The image logically follows prior-frame setting, weather, lighting, action, and screen direction.
- No extra limbs, duplicated people, merged faces, mismatched eyes, pseudo-text, fake logos, or random jewelry appear.
- No unrequested drift in identity, age, body size, cultural context, or signature styling occurs.

## Rights and ethical handling

- Use authorized source images for real people.
- Do not create deceptive impersonation or non-consensual intimate imagery.
- Maintain an approved origin and reference set for recurring fictional characters.
- Clearly distinguish fictional character art from real documentary or news imagery where confusion is possible.

## Final output format

1. Character identity lock
2. Allowed scene changes
3. Continuity anchors
4. Final image prompt
5. Preserve exactly
6. Avoid
7. Identity-drift revision instructions
8. Quality-control review
