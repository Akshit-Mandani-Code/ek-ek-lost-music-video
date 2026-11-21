# Reconstruction Standard — From Nothing but This Repository

## Purpose
This repository must allow a future AI assistant or filmmaker—with no access to this conversation, our current AI platform, our generated images, or any external visual archive—to recreate a closely similar music video from scratch.

The repository is intentionally text-only. It must contain the complete creative and technical blueprint, not links to required visual references.

## Required external input
The exact song audio master will be supplied separately later, either as an audio file or an accessible download link. Lyrics and manually authored timing markers are documented in the repository, but they do not replace the actual audio. Until the audio is supplied, do not claim that the final duration, musical phrasing or ending cut has been fully verified.

## No external visual dependencies
A fresh reconstruction must not require:
- Existing character photographs or face references.
- Generated character sheets, location images, prop photos or moodboards.
- Existing video clips, stills, thumbnails or exports.
- This ChatGPT conversation, prior AI history or platform galleries.
- Any external archive or private folder.

Current-production media can be useful to us now, but is optional. The written specification is the canonical source for a future from-scratch recreation.

## What “reconstructable” means
The documentation must preserve enough detail to recreate:
- The narrative, emotional progression and scene order.
- Character appearance, wardrobe, body language and continuity across timelines.
- Locations, room layouts, props, materials and practical details.
- Visual style, cinematography, framing, lighting, palette and atmosphere.
- Every shot's action, composition, duration, music relationship and transition.
- Model-agnostic image prompts, animation prompts, negative constraints and fallbacks.
- Editing timeline, cut logic, transitions, color treatment and audio synchronization.

It does not promise pixel-identical results. AI image/video outputs are stochastic and vary by model, version, seed and tool. The target is a close recreation of the story, design language, visual progression, framing, emotional intent, timing and edit.

## Required bootstrap process
A future AI must begin by generating its own visual references from text:
1. Read the project, character, environment, prop and style bibles.
2. Generate a protagonist character sheet using the full written description.
3. Generate a mother character sheet using the full written description.
4. Generate location and key prop sheets.
5. Establish consistent internal references for the session.
6. Generate the shot stills and animate them from the shot specifications.
7. If the platform cannot attach/reuse generated references, repeat full identity and continuity descriptions in every relevant prompt and use stable settings/seeds where available.

Do not ask the user for external images to proceed.

## Required record for every final shot
Each final shot must have:
- Unique shot ID and status.
- Timeline in/out, duration and source music/lyric marker.
- Narrative purpose and emotional beat.
- Location, time, characters, wardrobe and props.
- Framing, angle, lens/look, composition, camera movement and focus.
- Lighting, palette, atmosphere and realism constraints.
- Complete image-generation prompt and negative constraints.
- Complete image-to-video/text-to-video animation prompt.
- Start/end visual states and transition instructions.
- Clip trim, speed, transition and grading notes.
- Tool/model/settings/seed where known, plus known limitations and fallback.

## Tool independence
Keep a model-agnostic master prompt as the canonical creative instruction. Tool-specific adaptations may be added separately. Record model/version/settings and generation deviations when known, but do not make any single platform mandatory.

## Repository media policy
Never commit images, video, audio, rendered frames, thumbnails, project files or other binaries. Keep the actual music outside the repository until the user decides how to supply it. The repository may contain a future audio download link or filename as text, but must not depend on any visual media link.

## Completion gate
The repository is reconstruction-ready when a new AI can use only its text contents plus the separately supplied exact song audio to generate all required visual references and shots, then rebuild the intended edit without undocumented chat history or external visual assets.