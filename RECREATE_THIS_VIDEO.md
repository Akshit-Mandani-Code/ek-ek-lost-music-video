# RECREATE THIS VIDEO — Master Instructions for Any AI

## Your assignment
Recreate the cinematic music video described in this repository. You have not participated in the original conversation and must assume you have no access to any previous images, videos, character references, platform history or external production archive.

Your only required inputs are:
1. This complete GitHub repository.
2. The exact song audio master, supplied separately by the user as a file or an accessible download link.

**Do not ask the user to provide visual reference images.** All characters, locations, props and visual references must be generated from the written specifications in this repository.

## Non-negotiable reconstruction rules
- Treat repository text as the creative source of truth.
- Do not depend on the original ChatGPT conversation or any undocumented decisions.
- Do not depend on CH3 or any other existing face image. Those are optional aids from a different production session, not required inputs.
- Do not depend on existing location photographs, prop photographs, moodboards, generated stills, video clips or exports.
- Do not upload media binaries to this repository.
- Do not promise pixel-identical AI results. Different models produce different images. Preserve the character design, wardrobe, story, composition, cinematography, emotional intent, music timing and editing logic as closely as possible.
- Do not invent exact lyric timings or musical events. Use the supplied timing documents and verify against the actual audio.

## Required reading order
Read these documents before generating anything:
1. `00_PROJECT_OVERVIEW/RECONSTRUCTION_STANDARD.md`
2. `00_PROJECT_OVERVIEW/PROJECT_BRIEF.md`
3. `00_PROJECT_OVERVIEW/STORY_SYNOPSIS.md`
4. `00_PROJECT_OVERVIEW/DECISION_LOG.md`
5. `01_MUSIC_AND_LYRICS/CANONICAL_LYRICS.md`
6. `01_MUSIC_AND_LYRICS/AUDIO_SECTION_TIMINGS.md`
7. `02_VISUAL_DIRECTION/VISUAL_STYLE_BIBLE.md`
8. `03_CHARACTERS/PROTAGONIST/CHARACTER_BIBLE.md`
9. `03_CHARACTERS/PROTAGONIST/HOODIE_CONTINUITY.md`
10. `03_CHARACTERS/MOTHER/CHARACTER_BIBLE.md`
11. `04_LOCATIONS_AND_PROPS/CONTINUITY_BIBLE.md`
12. `05_STORYBOARD/MASTER_STORY_STRUCTURE.md`
13. `06_AI_PROMPTS/PROMPT_ARCHITECTURE.md`
14. All shot specifications and prompt files linked from the storyboard/shot tracker.
15. `08_EDITING/EDIT_DECISION_LIST.md`

If a linked file is missing, do not invent its approved contents. Identify the gap and use only confirmed decisions from the files that exist.

## Phase 1 — Understand the song
1. Obtain the exact song audio file from the user or accessible link.
2. Confirm that it is the same song/version described by the lyrics and timing map.
3. Read all lyric and section markers from the repository.
4. Listen to the audio and verify the emotional arc, instrumental passages, vocal phrasing, transitions and final ending.
5. Treat the manually authored markers as timing anchors, not necessarily exact vocal boundaries.
6. If a timing conflict exists, report it and ask before changing canonical markers.

If the audio has not been supplied yet, you may prepare the visual plan, but must not claim audio-verified synchronization or finalize the cut.

## Phase 2 — Generate the visual universe from text
Do not jump directly into shot generation.

### A. Protagonist
Generate a protagonist character sheet from the full written protagonist bible. Establish a consistent face, age, skin tone, facial structure, hair, stubble, build and natural expression range. The approved current-production CH3 image is not required and must not be requested.

### B. Mother
Generate a mother character sheet from the full written mother bible. Preserve the same recognizable identity across present-day and remembered past, allowing only plausible age and styling differences described in the bible.

### C. Timeline and wardrobe states
Generate any needed variations from text:
- Adult protagonist with hood up for bathroom, faceless and present-day station scenes.
- Same adult protagonist with hood down for the mother-lap ending.
- Mother in present-day saree styling and the earlier newborn-memory styling.
- Newborn son in the mother's arms, based on the story and period-appropriate simple clothing.

### D. Locations and props
Generate internal reference sheets for the apartment bathroom, bedroom/study, station environment and all recurring props using the written environment and prop bible. Keep architecture, furniture, materials and object designs consistent.

### E. Internal continuity
Choose the strongest coherent generated designs and reuse them as internal references throughout the session wherever the platform permits. If image references are not supported, repeat the complete relevant text description in every prompt and use consistent model/settings/seeds where available.

These generated references are working aids created by you. They are not external prerequisites.

## Phase 3 — Build the shots
Follow the approved story structure and shot list. For every shot:
1. State its narrative purpose and emotional beat.
2. Identify the lyric/section or instrumental passage it supports.
3. Use the complete character, wardrobe, location and prop descriptions.
4. Generate a still image using the model-agnostic prompt.
5. Check it against the written continuity rules.
6. Revise until it meets the intended composition and emotional function.
7. Animate the selected still with a separate motion prompt.
8. Keep motion physically plausible and restrained; avoid unnecessary complexity.
9. Check for face drift, wardrobe changes, geometry changes, hand defects and unwanted camera movement.
10. Record the chosen tool/model/settings and any deviations.

Do not generate random filler shots. Each shot must advance the story, establish an emotional beat, or create a deliberate visual transition.

## Phase 4 — Edit and synchronize
Use the actual supplied song as the master timeline. Follow the repository's edit decision list, shot durations, transitions and color progression. Verify all cuts by listening to the music. Do not infer an ending time solely from a lyric marker if the audio continues afterward.

If using DaVinci Resolve, work at the documented project resolution/frame rate and use proxies or optimized media when necessary. Preserve the full audio unless the approved edit plan specifies a verified cut.

## Phase 5 — Quality control
Before calling the recreation complete, verify:
- Story and emotional arc match the repository.
- Protagonist and mother remain visually coherent.
- Hoodie design and hood-up/hood-down progression are correct.
- Locations and props remain consistent.
- First chorus and final chorus have intentionally different emotional meanings.
- Mother's newborn memory is clearly a real remembered past, not a supernatural vision.
- The tear is physically realistic, with no glowing or magical effect.
- The son's face returns quietly; no triumphant pose or exaggerated smile.
- All edits follow the supplied audio and timing blueprint.
- No external visual asset was required at any stage.

## If the repository leaves something undecided
Do not silently turn a provisional idea into canon. Preserve the confirmed decisions, make the smallest practical assumption only when necessary, label it provisional, and ask the user about major creative choices.

## Final deliverables
Produce the finished music video and, if requested, a concise generation/edit report listing tools, model versions, prompts, settings, limitations and any deviations from the repository. The finished media does not belong in this GitHub repository.