# AI Prompt Architecture — Self-Contained by Design

Every prompt in this repository must work without attaching an existing image. A future AI starts with repository text, generates its own internal references and then creates the shots. The repository text—not a generated image or prior chat—is the source of truth.

## 1. Canonical written sources

- Decision log: approval status of creative choices.
- Character bibles: identity, appearance, wardrobe and performance.
- Hoodie continuity: approved garment and hood states.
- Visual style bible: cinematography, lighting, palette and realism.
- Locations/props bible: sets and recurring objects.
- Master story structure: sequence order and emotional meaning.
- Audio timing document: manually authored music anchors.
- Shot tracker and individual shot sheets: production execution.

When two documents discuss the same topic, the specialist bible defines the detailed specification; the decision log defines whether the choice is approved, provisional or undecided.

## 2. Required reference bootstrap

Before generating story shots, create the following from repository text:

1. Protagonist character sheet — `CHARACTER_SHEETS/PROTAGONIST_CHARACTER_SHEET.md`.
2. Mother character sheet — `CHARACTER_SHEETS/MOTHER_CHARACTER_SHEET.md`.
3. Environment references — `REFERENCE_SHEETS/ENVIRONMENT_REFERENCE_SHEETS.md` (bathroom, bedroom/study, selected transit station and mother-lap room).
4. Separate recurring prop references as needed.

Select one coherent design for each. These references are created inside the future AI's own session. They are optional internal aids, not external prerequisites. Do not ask the user for an existing portrait, moodboard, location photo or prop photograph.

## 3. Timeline and wardrobe variations

Generate and preserve:
- Adult protagonist, hood up: bathroom, faceless and present-day station scenes.
- Same adult protagonist and same hoodie, hood down: mother-lap ending.
- Mother in present-day saree styling and a plausibly younger newborn-memory styling.
- Newborn son held by the mother.

The newborn must read as a real past event. The adult and newborn are not the same generated face; preserve the emotional and compositional relationship rather than attempting impossible literal facial identity.

## 4. Still-image prompt requirements

Every shot prompt must specify:
- Complete relevant character identity and exact wardrobe state.
- Location, time and physical environment.
- Character position, pose, expression and captured action.
- Props and their placement.
- Shot size, camera angle/height, composition, lens/perspective and focus.
- Lighting direction, quality and source.
- Palette, atmosphere, texture and realism.
- Narrative emotion and continuity links.
- Negative constraints for common generation failures.

A prompt must remain understandable if all optional reference images are absent. If an internally generated reference is used, the written identity/environment description must still be present.

## 5. Animation prompt requirements

Write a separate animation prompt for every animated still. Specify:
- Clip duration and one primary action.
- Camera movement or explicitly locked camera.
- Subject movement, small and physically plausible.
- Environmental motion (water, fabric, crowd, curtain, etc.).
- What must remain unchanged: identity, clothing, composition, geometry, lighting and set layout.
- What must not happen: morphing, facial drift, extra limbs, camera warping, wardrobe changes, sudden cuts unless requested.

Prefer one primary movement per short clip. Use editing for major story-state changes rather than asking a video model to transform a face, person or location.

## 6. First-frame / last-frame workflow

When a transition requires two generated states, describe both endpoints fully in text. Match camera, lens feel, framing, subject scale and lighting; change only the intended story state. Explain the transition path. Do not rely on an attached image to define either endpoint.

## 7. Optional current-production references

CH3 and images generated during current production may be used as optional aids by the current team only. Every prompt remains complete without them. Never write “exact same person as attached image” as the only identity instruction. Never ask a future user for these images.

## 8. Model independence and generation record

Keep a model-agnostic master prompt as the source of truth. Put model-specific adaptations in separate files; never overwrite the master. Record tool, model, version, settings, aspect ratio, seed (if available), optional internal reference and local output filename. No generated media or project binaries belong in GitHub.

## 9. Prompt write-through

Every production-ready prompt developed for this project must be saved in the relevant repository file during the same working session. Preserve exact wording, assign a prompt ID/version and report the updated path. Casual brainstorming need not be archived until it becomes an actionable production instruction.

## Production order

1. Generate and select the protagonist character sheet.
2. Generate and select the mother character sheet.
3. Generate and lock the bathroom and bedroom/study references.
4. Decide the exact transit-station type, then generate its reference.
5. Generate the mother-lap room and only the props needed for the first shots.
6. Review the existing bathroom water-splash prompt and create its matching shot sheet.
7. Generate the first key stills, review continuity, then animate approved stills.
8. Continue through the shot tracker in story order.

Do not generate all scenes at once. Maintain one consistent visual universe and review each milestone before moving on.
