# Asset Register — Metadata Only

This register indexes every supplied, generated, selected or final media asset. **It must never contain the media files themselves.** All images, videos, audio and project binaries remain in the external media archive. This file records metadata and recovery locations only.

| Asset ID | Exact filename | Type / description | Status | Used in shot(s) | Prompt ID | External archive path | Backup status | Notes |
|---|---|---|---|---|---|---|---|---|
| CHAR-PROTAG-CH3 | TBD | Original user-supplied protagonist face reference | Approved reference; archive location pending | All visible-face shots | N/A | TBD | Unknown | Identity-critical; preserve original resolution |
| CHAR-MOTHER-REF | TBD | Mother identity reference | Pending | Mother scenes | TBD | TBD | TBD | Maintain identity across timelines |
| WARDROBE-HOODIE-01 | N/A — text specification | Plain charcoal pullover hoodie specification | Approved specification | Present-day protagonist scenes | N/A | GitHub continuity bible | N/A | Hood position varies by story state |
| IMG-REF-A-001 | TBD | Bathroom water-splash still, protagonist face visible, hood up | Not generated | Intro / bathroom sequence | PROMPT-REF-A-001 v01 | TBD | TBD | Attach CHAR-PROTAG-CH3 when generating |

## Asset ID convention
CHAR- = character references; LOC- = location/set references; PROP- = props; IMG- = generated stills; VID- = generated video; AUD- = audio; EDIT- = edit/project/export; GFX- = graphics/titles. Use stable IDs and a version suffix for each distinct generation.

## Required metadata
Record stable ID, exact filename, type, format, dimensions/resolution, frame rate/duration where applicable, file size and SHA-256 checksum when practical, generation/capture date, tool/model/version/settings, prompt ID and reference IDs/input order, approval state, reviewer notes, parent/derived relationships, exact external archive path and backup status.

## Rules
- Never overwrite the only approved original; save new versions separately.
- Keep rejected generations only if useful for learning or as alternatives.
- Keep original user-supplied references separate from AI-generated derivatives.
- Asset register must agree with the final shot list and edit decision list.
- Save generated originals immediately outside the AI platform.
- **Never upload media files to this GitHub repository.** GitHub is only the text-based index and reconstruction blueprint.
