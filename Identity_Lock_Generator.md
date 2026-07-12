Using this for identity lock, to ensure the character's identity is preserved.

```
# Identity Lock Generator

You are analyzing the three attached Character Reference Sheets:
1. Full-Body Turnaround (five standing views)
2. Head Portraits (four angles)
3. Expression Range (six expressions)

Together these constitute the "Identity Model" for one individual. Your task
is to produce an **Identity Fidelity Requirements** document that will be
attached to future image-generation prompts to lock this character's
identity. Write it so that any image model reading it, alongside the three
sheets, can reproduce this exact individual.

## Analysis Instructions

Study all three sheets before writing. Base every statement on what is
visually observable — never invent, assume, or generalize features you
cannot see. Describe features in concrete visual language (shapes, colors,
gradients, silhouettes), not subjective terms ("handsome", "striking").

Identify the subject's **Primary Identity Anchor**: the one or two most
distinctive, recognizable features of this specific person — the features a
stranger would use to describe them (e.g., a distinctive beard, unusual
hair, prominent glasses, a strong nose, freckle pattern, distinctive eyes).
This anchor gets its own expanded section with the most detailed treatment.

Note any asymmetries, marks, moles, scars, or irregularities and their
locations — these are identity evidence, not flaws.

## Output Format

Produce ONLY the document below, in markdown, with no commentary before or
after. Follow this structure exactly, filling in observations from the
sheets:

# Identity Fidelity Requirements

## Core Principle
The subject must always be recognizable as the same individual shown in
the Identity Model. A human familiar with the Identity Model should
immediately recognize the subject in every generated image.

## Facial Structure (Non-Negotiable)
"Preserve:" list covering skull shape and cranial silhouette, forehead
structure, eye spacing and alignment, eyebrow shape and placement, nose
bridge and nose shape, cheekbone structure, jawline and chin proportions,
mouth shape and lip proportions, ear size/placement/attachment — each item
annotated with the specific observed characteristics of THIS subject, not
generic anatomy.
"Do not:" list forbidding stylizing proportions, beautifying or idealizing,
averaging facial structure, or altering natural asymmetry.

## Eyes
Observed color (be precise), structural depth, shape, symmetry, and any
distinctive qualities. Note eyewear here if the subject wears any, treating
it as part of identity.

## [Primary Identity Anchor] (Primary Identity Anchor)
Title this section after the actual feature (e.g., "Beard", "Hair",
"Glasses", "Freckle Pattern"). Provide the most detailed treatment in the
document: silhouette, texture, density, color including any gradients or
patterns, and how it appears across angles. Include a "Do not:" list of
the specific ways image models tend to simplify or restyle this feature.
If two features are equally distinctive, give each its own section.

## Hair
Color (precise, including any variation), length, texture, part placement
and direction, silhouette from front / profile / back as shown in the
sheets, and any styling that must remain consistent. If hair was already
the Primary Anchor, omit this section.

## Skin & Distinguishing Marks
Skin tone in plain descriptive terms. Location and character of all visible
moles, freckles, scars, or marks, described positionally ("left cheek,
below the outer corner of the eye"). If none are visible, state that the
skin is clear and must not gain invented marks.

## Body Structure
From the Turnaround sheet: shoulder width relative to hips, torso and limb
proportions, posture tendency, overall build and mass distribution. Include
the instruction: "Do not rely on numeric height/weight values over visual
reference consistency."

## Expression Behavior
From the Expression sheet: briefly describe how this face changes under
emotion — what the smile does, how the brow moves, any expression-specific
landmarks (dimples, crow's feet, forehead lines) — so expressive images
deform the face the way THIS face deforms, not generically.

## Usage Note
End with: "These requirements apply to every generated image of this
subject, in every style, setting, attire, and expression. When any prompt
instruction conflicts with identity fidelity, identity fidelity wins."
```
