# Working Protocol — Self-Contained Reconstruction

## 1. The repository is the creative source of truth
- **ChatGPT conversation:** collaborative development, decisions, prompt reviews and iteration.
- **GitHub repository:** durable, tool-independent instructions sufficient for a new AI or filmmaker to recreate the visual film without this conversation.
- **Current-production media archive:** optional convenience for our present work only. It is not part of the future reconstruction contract.

A future creator must not need our chat history, current AI platform, current generated images, external character references, or an existing media archive to understand and rebuild the film.

## 2. Required input and optional inputs
- **Required external input:** the exact song audio master. The user will add the audio file or an accessible download link later.
- **Repository-provided material:** lyrics, manually authored section/lyric markers, story, characters, environments, props, visual style, shot design, prompts, continuity rules and editing blueprint.
- **Optional only:** any images or clips created during this current production. They may be used as convenience references, but every prompt and design must remain usable without them.

If the audio is not yet supplied, continue visual development using the repository timing markers. Do not claim to have verified musical phrasing, final duration or exact cut points beyond the information recorded here.

## 3. Absolute GitHub media exclusion
Do not commit or upload images, videos, audio, thumbnails, rendered frames, project binaries or other media assets. Store text specifications, prompts, decisions, timing, metadata and instructions only.

## 4. Self-contained visual specification rule
Every recurring visual element must be described in text with enough specificity to regenerate it:
- Character age range, facial structure, skin tone, hair, build, clothing, posture, emotional behavior and timeline variations.
- Locations, architecture, layout, furniture, materials, practical details, lighting and atmosphere.
- Props, dimensions/style/materials, wear, placement and narrative purpose.
- Cinematography, composition, lens/look, camera position, movement, focus, palette and texture.
- Each shot's narrative purpose, exact action, start/end state, image prompt, animation prompt, duration and transition.

Never write “use the attached reference image” as a required instruction. If a current-production reference exists, label it **optional current-production reference** and include the complete text specification in the prompt itself.

## 5. Character and visual bootstrap workflow for any future AI
A future AI receiving only this repository and the song must:
1. Read `RECREATE_THIS_VIDEO.md` and all linked canonical documents.
2. Extract the character and visual specifications.
3. Generate its own protagonist and mother character sheets from the written character bibles.
4. Select internally consistent character appearances and reuse those AI-generated sheets within that recreation session wherever the tool supports image references.
5. Generate location and key prop reference sheets from the written environment/prop bible.
6. Create shot stills and animate them using the shot prompts.
7. If its platform cannot preserve image references, repeat the full character and wardrobe descriptions in each prompt and use a consistent seed/model/settings where supported.
8. Compare every output against the text continuity checklist; do not treat the generated references as new canon unless they satisfy the written design.

The future AI's internally generated sheets are working aids, not external prerequisites.

## 6. Prompt write-through rule
Whenever a production-ready prompt is written:
1. Save the complete prompt as text in the relevant repository file during the same working session.
2. Preserve exact prompt wording.
3. Assign prompt ID, version, purpose, status and any optional inputs.
4. Keep the model-agnostic master separate from tool-specific adaptations.
5. Retain used/superseded versions rather than silently erasing production history.
6. Tell the user which file was updated.

Casual brainstorming does not need archiving until it becomes an actionable production instruction.

## 7. Optional current-production asset tracking
The asset register may record current-production images, clips and audio for convenience. Mark these clearly as optional and never describe them as required inputs for future reconstruction. Do not add external archive paths as dependencies.

## 8. Status vocabulary
- `DRAFT`: being discussed.
- `READY`: complete and usable.
- `GENERATED`: output exists but has not been reviewed.
- `SELECTED`: preferred candidate, pending final approval.
- `APPROVED`: accepted as canonical design or production asset.
- `REJECTED`: not to be used.
- `SUPERSEDED`: replaced by a newer version; retain history.

## 9. Session handoff checklist
Update the decision log and relevant text bibles when a creative decision is approved. Save production-ready prompts in GitHub. Clearly distinguish confirmed decisions from provisional ones. Verify that no prompt requires an image or file outside the repository. Keep the music input requirement explicit until the user adds the audio file or link.