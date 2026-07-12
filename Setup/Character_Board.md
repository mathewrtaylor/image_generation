Character Board sheet

Step 1 of the Character Identity Setup (see repo README). Upload as many
reference photos of the person as your image orchestrator allows, then run
all three prompts below in the same session. Each prompt reuses those
uploaded photos, not the sheet a previous prompt produced. The three
resulting sheets together form the "Identity Model" — attach all three to
Identity_Lock_Generator.md in the next (new) session.

The neutral grey attire, flat studio lighting, and plain background are
intentional across all three sheets: they remove clothing, lighting, and
setting as variables so the only thing downstream prompts have to lock
onto is the person's actual face and body.

Run in this order — turnaround first establishes build and proportions,
portraits add facial detail, expressions round out how the face moves:

Full Body Turnaround
```
CHARACTER REFERENCE — SHEET 1 OF 3: FULL-BODY TURNAROUND

Using the uploaded images as reference, create a full-body character
turnaround sheet: ONE horizontal row of five standing views of the same
person, left to right: Front, 3/4 Left, Left Profile, Back, Right Profile.

POSE: Relaxed A-pose, arms slightly away from the body, palms facing
forward so hands are visible. Barefoot. Neutral, relaxed facial expression,
mouth closed. Identical height, build, and limb proportions in all five
views, with a consistent eyeline across the row.

IDENTITY: Strict 1:1 identity match to the reference images. Preserve all
distinguishing features — facial hair shape, moles, freckles, scars, and
natural asymmetries — in the same locations in every view. Do not beautify,
smooth, or idealize the subject.

TECHNICAL:
- Photorealistic, sharp focus throughout, no motion blur, no film grain,
  no stylization.
- 85mm-equivalent lens at the subject's eye level; no wide-angle distortion.
- Attire: form-fitting medium-grey t-shirt, dark fitted trousers.
- Lighting: flat, diffuse, high-key studio lighting; even illumination,
  no harsh shadows; preserve skin texture.
- Background: solid, flat light-grey.

LAYOUT: Single high-resolution landscape image. Generous empty background
margin on all four edges; the bottom-right corner must remain completely
empty background. No text, labels, logos, or watermarks within the panel
area.
```

Head Portraits — close-up detail on the face itself (ears, jawline,
hairline) that the turnaround sheet is too far back to capture.
```
CHARACTER REFERENCE — SHEET 2 OF 3: HEAD PORTRAITS

Using the uploaded images as reference, create a portrait reference sheet:
ONE horizontal row of four high-detail head-and-shoulder portraits of the
same person, left to right: Front, 3/4 Left, Left Profile, Right Profile.

POSE: Neutral, relaxed expression, mouth closed, eyes open and level. Hair
styled or tucked behind the ears so that ears, jawline, and hairline are
clearly visible, especially in the profile views. Identical head size and
eyeline across all four portraits.

IDENTITY: Strict 1:1 identity match to the reference images. Preserve all
distinguishing features — facial hair shape, moles, freckles, scars, and
natural asymmetries — in the same locations in every view. Do not beautify,
smooth, or idealize the subject.

TECHNICAL:
- Photorealistic, sharp focus, no motion blur, no film grain, no
  stylization. Fine skin texture and facial detail preserved.
- 85mm-equivalent lens at the subject's eye level; no wide-angle distortion.
- Attire: form-fitting medium-grey t-shirt.
- Lighting: flat, diffuse, high-key studio lighting; even illumination,
  no harsh shadows.
- Background: solid, flat light-grey.

LAYOUT: Single high-resolution landscape image. Generous empty background
margin on all four edges; the bottom-right corner must remain completely
empty background. No text, labels, logos, or watermarks within the panel
area.
```

Expression Range — shows how this specific face deforms under emotion, so
later prompts can render feeling without drifting into a generic face.
```
CHARACTER REFERENCE — SHEET 3 OF 3: EXPRESSION RANGE

Using the uploaded images as reference, create an expression reference
sheet: a 3x2 grid (three columns, two rows) of six head-and-shoulder
portraits of the same person, one distinct expression per panel:

Top row, left to right: Neutral, Joy (open smile), Anger.
Bottom row, left to right: Sadness, Surprise, Fear.

POSE: All six portraits face the camera directly (front view), identical
head size and framing in every panel. Each expression must be clearly
distinct and readable, showing how the face changes while the identity
stays constant.

IDENTITY: Strict 1:1 identity match to the reference images. Preserve all
distinguishing features — facial hair shape, moles, freckles, scars, and
natural asymmetries — in the same locations in every panel. Do not
beautify, smooth, or idealize the subject.

TECHNICAL:
- Photorealistic, sharp focus, no motion blur, no film grain, no
  stylization. Fine skin texture preserved.
- 85mm-equivalent lens at the subject's eye level; no wide-angle distortion.
- Attire: form-fitting medium-grey t-shirt.
- Lighting: flat, diffuse, high-key studio lighting; even illumination,
  no harsh shadows.
- Background: solid, flat light-grey.

LAYOUT: Single high-resolution landscape image. Generous empty background
margin on all four edges; the bottom-right corner must remain completely
empty background. No text, labels, logos, or watermarks within the panel
area.
```
