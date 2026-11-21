# Ek Ek Lost — Cinematic AI Music Video

This repository is the **tool-independent, text-only reconstruction blueprint** for the music video. It must allow a future AI or filmmaker—with no access to this chat, our current generation platform, or our current images—to recreate a closely similar visual film from scratch.

## Start here
1. [Recreate this video — master instructions](RECREATE_THIS_VIDEO.md)
2. [Reconstruction standard](00_PROJECT_OVERVIEW/RECONSTRUCTION_STANDARD.md)
3. [Working protocol](00_PROJECT_OVERVIEW/WORKING_PROTOCOL.md)
4. [Project brief](00_PROJECT_OVERVIEW/PROJECT_BRIEF.md)
5. [Story synopsis](00_PROJECT_OVERVIEW/STORY_SYNOPSIS.md)
6. [Decision log](00_PROJECT_OVERVIEW/DECISION_LOG.md)
7. [Canonical lyrics](01_MUSIC_AND_LYRICS/CANONICAL_LYRICS.md)
8. [Audio section and lyric timings](01_MUSIC_AND_LYRICS/AUDIO_SECTION_TIMINGS.md)
9. [Visual style bible](02_VISUAL_DIRECTION/VISUAL_STYLE_BIBLE.md)
10. [Protagonist character bible](03_CHARACTERS/PROTAGONIST/CHARACTER_BIBLE.md)
11. [Hoodie continuity](03_CHARACTERS/PROTAGONIST/HOODIE_CONTINUITY.md)
12. [Mother character bible](03_CHARACTERS/MOTHER/CHARACTER_BIBLE.md)
13. [Locations and props continuity](04_LOCATIONS_AND_PROPS/CONTINUITY_BIBLE.md)
14. [Master story structure](05_STORYBOARD/MASTER_STORY_STRUCTURE.md)
15. [AI prompt architecture](06_AI_PROMPTS/PROMPT_ARCHITECTURE.md)
16. [Reference still prompt — REF-A bathroom](06_AI_PROMPTS/REFERENCE_STILLS/REF-A_BATHROOM_HOOD_UP.md)
17. [Shot specification template](06_AI_PROMPTS/SHOT_SPECIFICATION_TEMPLATE.md)
18. [Asset register — optional production metadata](07_PRODUCTION/ASSET_REGISTER.md)
19. [Shot tracker](07_PRODUCTION/SHOT_TRACKER.md)
20. [Edit decision list](08_EDITING/EDIT_DECISION_LIST.md)

## Reconstruction contract

**Required external input:** the exact song audio master, to be supplied later by the person recreating the video. The audio file or a stable, accessible download link may be provided separately. The repository currently contains the lyrics and manually authored timing markers, but not the audio itself.

**Everything visual must be reconstructable from this repository alone.** No external images, videos, face references, character sheets, location photos, prop photos, prior chat history, or current-production assets may be required. A future AI must generate its own character sheets and visual references from the written specifications before generating shots.

## Media storage rule
This repository is text-only. Do not commit images, videos, audio, rendered frames, thumbnails, or project binaries. Current-production media may be stored elsewhere for convenience, but those assets are optional and must never be prerequisites for a fresh reconstruction.

## Production principles
- Zero-budget tools and workflows only; verify free-tier limits before depending on a service.
- Photorealistic, emotionally grounded cinema; avoid random AI montage.
- Preserve approved character, wardrobe, location, prop and music continuity.
- Use the user-authored Audacity markers as the timing authority; do not invent exact lyric timings.
- Keep model-agnostic master prompts and tool-specific adaptations separately.
- Archive every production-ready prompt in GitHub as text during the same working session.
- Different AI models may produce different faces and images. Preserve narrative, design, framing, mood, timing and edit intent rather than promising pixel-identical output.

## Current phase
Pre-production / visual development. The next immediate visual development task is to establish self-contained character-generation instructions and then develop the three key hoodie states: bathroom water-splash, hooded faceless protagonist, and mother-lap ending.