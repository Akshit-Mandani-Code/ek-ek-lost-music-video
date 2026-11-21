# AI Prompt Architecture — Self-Contained by Design

Every prompt in this repository must work without attaching an existing image. A future AI starts with repository text, generates its own internal references, and then creates the shots.

## 1. Canonical written sources
The character bibles, visual style bible, environment/prop bible, story structure and decision log are the creative source of truth. A generated image is never the only record of a design decision. Prompts must repeat the relevant identity, wardrobe and environment details rather than relying on undocumented visual memory.

## 2. Character bootstrap
Before creating story shots, generate:
- A protagonist character sheet using the complete written protagonist bible.
- A mother character sheet using the complete written mother bible.
- Required timeline variations (adult son; newborn son; mother in present and earlier memory).
- Consistent wardrobe views and neutral expression/pose variations where useful.

Select one coherent design per character for that recreation. Reuse the generated sheet as an internal image reference when the platform supports it. If it does not, repeat the full written identity description in every prompt and use stable model/settings/seeds where available. These sheets are generated during that session and are not external prerequisites.

## 3. Environment and prop bootstrap
Generate internal reference views for recurring locations and important props using the written continuity bible. Keep architecture, room layout, materials, furniture, object design, scale and wear consistent across shots. These references are generated from text; they are not required inputs.

## 4. Still-image prompt
Every shot prompt must specify:
- Complete relevant character description and exact wardrobe state.
- Scene/location, time and physical environment.
- Character position, pose, expression and captured action.
- Camera framing, angle, composition, lens/look and focus.
- Lighting, color palette, atmosphere and texture.
- Props and their placement.
- Narrative emotion and continuity constraints.
- Negative constraints preventing common generation failures.

## 5. Animation prompt
Specify separately:
- Camera movement or explicitly locked camera.
- Subject movement, small and physically plausible.
- Environmental motion (water, fabric, background extras, etc.).
- Duration and motion pacing.
- What must remain unchanged: identity, clothing, composition, geometry, lighting and scene layout.
- What must not happen: morphing, facial drift, extra limbs, camera warping, sudden cuts unless requested.

## 6. First-frame / last-frame workflow
Design both stills with matching camera, lens feel, framing, subject scale and lighting. Change only the intended story state. Describe the transition path between endpoints. Both endpoints must be fully described in text; do not rely on external images to define them.

## 7. Optional current-production references
CH3 and any images generated during the current production may be used as optional aids by the current team only. Every prompt must remain fully understandable and usable if those images are absent. Never write “exact same person as attached image” as the only identity instruction. Do not ask a future user for these images.

## 8. Model independence and generation record
Keep a model-agnostic master prompt as the source of truth. Store model-specific adaptations separately; never overwrite the master. For current production, record tool, model, version, settings, aspect ratio, seed (if available), optional internal reference used and output filename outside GitHub as appropriate. No generated media or project binaries belong in this repository.

## 9. Prompt write-through
Every production-ready prompt developed for this project must be saved as text in the relevant repository file during the same working session. Preserve exact wording, assign a prompt ID/version, and tell the user which file was updated. Casual brainstorming need not be archived until it becomes an actionable production instruction.

## Production order
Complete the written character and environment specifications first. Then create character sheets and key stills: hooded bathroom water-splash, hooded faceless protagonist, and mother-lap ending with hood down. Review stills for continuity before animation.