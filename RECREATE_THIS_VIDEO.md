# RECREATE THIS VIDEO — Master Instructions for Any AI

## Assignment and required inputs
Recreate the cinematic music video described by this repository. Assume you have no access to the original conversation, prior AI history, current-production images, current generation platform or external media archive.

The only required inputs are:
1. The complete text contents of this repository.
2. The exact song audio master, supplied separately by the user as an audio file or an accessible download link.

**Never ask the user for visual reference images.** Generate every character sheet, location reference and prop reference from the written specifications in this repository.

## Non-negotiable rules
- Treat repository text as the creative source of truth.
- No external visual references, previous chat, platform galleries, generated stills, clips or archive folders may be required.
- CH3 is a current-production-only optional aid. It is not a required input and must not be requested.
- Do not commit images, video, audio or project binaries to this repository.
- Do not promise pixel-identical AI outputs. Preserve the story, character design, wardrobe, locations, shot composition, cinematography, emotional intent, timing and edit logic as closely as possible.
- Do not invent exact lyric timings or musical events. Use the supplied timing markers and verify against the actual audio.
- Preserve the distinction between approved, provisional and undecided creative choices in the decision log.

## Read these documents first
1. `00_PROJECT_OVERVIEW/PROJECT_BRIEF.md`
2. `00_PROJECT_OVERVIEW/DECISION_LOG.md`
3. `00_PROJECT_OVERVIEW/STORY_SYNOPSIS.md`
4. `01_MUSIC_AND_LYRICS/CANONICAL_LYRICS.md`
5. `01_MUSIC_AND_LYRICS/AUDIO_SECTION_TIMINGS.md`
6. `02_VISUAL_DIRECTION/VISUAL_STYLE_BIBLE.md`
7. `03_CHARACTERS/PROTAGONIST/CHARACTER_BIBLE.md`
8. `03_CHARACTERS/PROTAGONIST/HOODIE_CONTINUITY.md`
9. `03_CHARACTERS/MOTHER/CHARACTER_BIBLE.md`
10. `04_LOCATIONS_AND_PROPS/CONTINUITY_BIBLE.md`
11. `05_STORYBOARD/MASTER_STORY_STRUCTURE.md`
12. `06_AI_PROMPTS/PROMPT_ARCHITECTURE.md`
13. All shot prompt/specification files indexed in the shot tracker.
14. `08_EDITING/EDIT_DECISION_LIST.md`

If a referenced specification is missing or incomplete, identify the gap. Do not pretend an undecided detail is approved.

## Phase 1 — Understand the song
1. Obtain the exact song audio from the user or accessible link.
2. Confirm it matches the documented lyrics and timing map.
3. Listen to the complete track; verify its duration, instrumental passages, vocal phrasing, section transitions, emotional arc and ending.
4. Treat manually authored Audacity labels as timing anchors, not necessarily exact vocal boundaries.
5. If audio and labels conflict, report the discrepancy and ask before changing canonical timings.

Until the audio is supplied, visual development may proceed using the documented markers, but do not claim audio-verified synchronization or finalize the cut.

## Phase 2 — Build the visual universe from text
Do not jump directly into story-shot generation.

### A. Protagonist
Generate a consistent character sheet using the full written protagonist bible. Establish the same age, face shape, skin tone, eyes, hair, stubble, build and natural expression range across front, three-quarter and profile views.

### B. Mother
Generate a consistent mother character sheet from her written bible. Preserve recognizable facial identity across present-day and newborn-memory scenes, allowing only plausible age and styling changes.

### C. Timeline and wardrobe states
Generate the required variations from text:
- Adult protagonist, hood up, for bathroom, faceless and present-day station scenes.
- Same adult protagonist and same hoodie, hood down, for the mother-lap ending.
- Mother in present-day saree styling and earlier newborn-memory styling.
- Newborn son held in the mother's lap.

### D. Locations and props
Generate internal reference sheets for the apartment, bathroom, bedroom/study, transit station and recurring story props using the location/prop bible. Preserve layout, architecture, materials, furniture, object design and wear across shots.

### E. Continuity
Select internally consistent generated designs and reuse them within the session wherever the platform supports image references. If it does not, repeat the full relevant written descriptions in every prompt and use consistent model/settings/seeds where available.

These generated references are working aids created during your own session. They are not external prerequisites and do not become new canon unless they satisfy the written specifications.

## Phase 3 — Create the shots
Follow the approved story structure and shot tracker. Every final shot must have:
1. Unique shot ID and narrative purpose.
2. Emotional beat and lyric/section or instrumental relationship.
3. Timeline in/out and duration, verified against the audio.
4. Location, characters, wardrobe, props and continuity links.
5. Composition, framing, camera angle, lens/look, focus and camera movement.
6. Lighting, palette, atmosphere and realism constraints.
7. Complete still-image prompt and negative constraints.
8. Separate animation prompt describing camera, subject and environmental movement.
9. Start/end visual states and transition instructions where relevant.
10. Generation model/settings/seed where known, defects, selection and fallback notes.

Generate the still first, check it against continuity, then animate it. Keep movement physically plausible and restrained. Do not create random filler clips: every shot must advance the story, establish an emotional beat or create a deliberate transition.

## Phase 4 — Edit and synchronize
Use the supplied song as the master timeline. Follow the shot tracker and edit decision list, then verify every cut by listening to the actual audio. Never infer the final out-point from a lyric marker if the track continues afterward.

For DaVinci Resolve, use the documented project settings. Prefer 1080p, short clips and proxies/optimized media where necessary. Keep the source audio continuous unless an approved, verified edit says otherwise.

## Phase 5 — Quality control
Before completion, verify:
- Narrative and emotional progression match the synopsis and approved story structure.
- Protagonist and mother remain coherent across shots and timelines.
- The charcoal pullover hoodie remains the same garment; hood-up/hood-down progression is correct.
- Locations and recurring props remain consistent.
- The first chorus communicates collapse; the final chorus communicates remembrance and quiet renewal.
- The newborn sequence reads as an actual remembered past, not a supernatural vision.
- The tear is physically realistic, with no glow or magical effect.
- The son's face returns through a motivated cinematic edit; he opens his eyes peacefully.
- No triumphant pose, exaggerated smile or sudden victory montage is added.
- Timing and ending follow the supplied audio.
- No external visual asset was required at any stage.

## Handling undecided details
Do not silently convert provisional ideas into canon. Preserve confirmed decisions, make only minimal practical assumptions when necessary, label them provisional and ask the user about major creative choices.

## Deliverables
Create the finished music video outside GitHub. If requested, also provide a concise generation/edit report with tools, model versions, prompts, settings, limitations and deviations. Do not commit the finished media or project binaries to this repository.