# Consistent Character Image Generation

Prompts for keeping a consistent character identity across image generations, plus reusable scene prompts that plug into that identity.

## Use
So often, something in the prompt or the atatched image that causes the output to miss the mark. This repo is an attempt at causing a repeatable system for consistency and accuracy in your Image Prompts by creating an animation style Character Board or Model Sheet, and geenrating rules for how those images are used. While there is some setup required for this, this is a one time activity.

Once this has been done, you can use the translator to strip out non-essential componnents of a prompt, and structure into a repeatable manner for you to use.

## Layout

The repo is organized around:
- **`Setup/`** (below) — a one-time, multi-session pipeline that locks in
  one person's appearance so it can be reproduced in any scene.
- **`Prompt_Treanslator.md`** (root) — an everyday-use utility, run per
  scene rather than as part of the one-time setup, so it lives outside
  `Setup/`.
- **`Prompts/`** (planned) — individual scene prompts, each its own markdown
  file paired with an example output image.

## Files in this repo

| File | Role |
|---|---|
| `Setup/Character_Board.md` | Three prompts that turn uploaded reference photos into three Character Reference Sheets (Full-Body Turnaround, Head Portraits, Expression Range) — together these form the "Identity Model". |
| `Setup/Identity_Lock_Generator.md` | Analyzes the three Character Reference Sheets and writes an "Identity Fidelity Requirements" document describing the person's locked, non-negotiable features. |
| `Setup/Identity_Injection_Engine.md` | The reusable prompt. Takes the Identity Fidelity Requirements + the three reference sheets + a normalized scene description, and merges them into one final image-generation prompt. |
| `Prompt_Treanslator.md` | Strips a raw scene idea down to a normalized, structured prompt with the main character replaced by the `{{LOCKED_IDENTITY}}` placeholder, ready to feed into the Identity Injection Engine. |

## Character Identity Setup

Run once per character, across three separate sessions (keeping each stage
in its own session keeps the model focused on just that task):

1. **Session 1 — Build the Identity Model** (`Setup/Character_Board.md`)
   Upload as many reference photos of the person as your image orchestrator
   allows. In that same session, run all three prompts in order:
   Full-Body Turnaround → Head Portraits → Expression Range.
   Output: three Character Reference Sheets.

2. **Session 2 — Generate the Identity Fidelity Requirements** (`Setup/Identity_Lock_Generator.md`)
   Start a new session, attach the three Character Reference Sheets from
   Session 1, and run this prompt.
   Output: an Identity Fidelity Requirements document.

3. **Session 3 — Assemble the reusable Identity Injection Engine** (`Setup/Identity_Injection_Engine.md`)
   Paste the full output from Session 2 into the
   `# Identity Fidelity Requirements` placeholder section of this prompt.
   The result is a complete, character-specific Identity Injection Engine.

   Recommended: save this as a reusable prompt in your image tool, with the
   three Character Reference Sheet images attached in its knowledge/reference
   section alongside the prompt text, so it's self-contained (images + text)
   for everyday use.

## Everyday Usage

Once the reusable Identity Injection Engine exists (Session 3 above):

1. Take any ad-hoc scene idea and run it through `Prompt_Treanslator.md`
   first. It normalizes the prompt into structured plain text with the
   main character replaced by `{{LOCKED_IDENTITY}}`.
2. Copy that normalized output into the reusable Identity Injection Engine
   prompt as the normalized scene description.
3. The Identity Injection Engine merges the locked identity into the scene
   and outputs one final image-generation prompt — send that, along with
   the attached reference images, to your image model.
