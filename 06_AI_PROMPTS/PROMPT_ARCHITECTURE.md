# AI Prompt Architecture

Use this layered structure so prompts remain reusable across image and video models.

## 1. Character Bible
Identity, age, appearance, body type, approved face reference, wardrobe and continuity locks. Do not rewrite identity details differently in each shot.

## 2. Visual Style Bible
Photorealism, cinematic language, color, lighting, lens/depth-of-field intent, aspect ratio and realism constraints.

## 3. Shot Prompt (still image)
Specify:
- Scene/location and time of day
- Character position, pose and exact action at the captured instant
- Camera framing, angle and composition
- Lighting, atmosphere and background details
- Character/wardrobe/prop continuity
- Negative constraints that prevent common failures

## 4. Animation Prompt (image-to-video)
Specify separately:
- Camera movement (or explicitly locked camera)
- Subject movement, small and physically plausible
- Environmental movement (water, fabric, background extras)
- Duration and motion pacing
- What must remain unchanged: identity, clothing, composition, geometry and lighting continuity
- What must not happen: morphing, extra limbs, facial drift, camera warping, sudden cuts unless requested

## 5. First-frame / last-frame workflow
Design both stills with matching camera, lens feel, framing, subject scale and lighting. Change only the intended story state. Use a transition prompt that describes the path between those states, not just the endpoints.

## 6. Reference inputs and fallback
A prompt must not silently depend on an image that may be unavailable later.
- Give each important reference a stable asset ID.
- State which reference images must be attached to the generation tool.
- If the original image is available, attach it; a filename or asset ID in text is not a substitute for the actual image input.
- If unavailable, use the relevant written bible and label the generation as specification-only.
- For identity-critical faces, retrieve/re-upload the approved source image whenever possible. Text descriptions alone cannot guarantee the same face.
- Record parent/derived relationships when a generated image becomes a reference for another image or video.

## Master prompt policy
Keep a model-agnostic master prompt as the source of truth. Store model-specific adaptations in MODEL_SPECIFIC_ADAPTATIONS; never overwrite the master. Record tool, model, settings, aspect ratio, seed (if available), reference assets and output filename for each generation.

## Prompt write-through policy
Every production-ready prompt written in chat must also be saved in the relevant repository folder during the same working session. Preserve the exact text and assign a prompt ID and version. When revising, retain the history of any prompt already used to generate an asset. Casual brainstorming does not need to be archived until it becomes an actionable production prompt.

## Production priority
Generate and approve the three key hoodie reference stills first: bathroom water-splash, hooded faceless protagonist, and mother-lap ending. Do not animate before the stills pass continuity review.
