# Asset Register

This is the canonical index of every generated, supplied, selected or final asset. Use one row per file or logical asset. Do not rely on filenames alone; record what the asset depicts and which shots use it.

| Asset ID | Filename / path | Type | Description | Status | Used in shot(s) | Source / tool | Recovery location | Notes |
|---|---|---|---|---|---|---|---|---|
| CHAR-PROTAG-CH3 | TBD | Character reference | Approved protagonist face reference (CH3) | Approved reference; file to be archived | All visible-face shots | User supplied | To be recorded | Preserve original resolution; identity-critical source |
| CHAR-MOTHER-REF | TBD | Character reference | Approved mother identity reference | Pending | Mother scenes | To be generated/selected | To be recorded | Maintain identity across timelines |
| WARDROBE-HOODIE-01 | TBD | Wardrobe reference | Plain charcoal pullover hoodie | Approved specification | Present-day protagonist scenes | Written specification | This repository | Hood position varies by story state |
| IMG-REF-A-001 | TBD | Generated still | Bathroom water-splash, protagonist face visible, hood up | Not generated | Intro / bathroom sequence | Pending | To be recorded | Prompt: PROMPT-REF-A-001 v01; attach CHAR-PROTAG-CH3 |

## Asset ID convention
- CHAR- = character references
- LOC- = location/set references
- PROP- = prop references
- IMG- = generated still images
- VID- = generated video clips
- AUD- = audio sources/exports
- EDIT- = edit/project/export files
- GFX- = graphics/titles/composites

Use stable IDs even if an asset is regenerated. Add a version suffix to each distinct generation (for example IMG-INTRO-001-v01).

## Required metadata
For every important asset, record:
- Stable asset ID and exact filename including extension.
- File type, format, dimensions/resolution, frame rate and duration where applicable.
- File size and checksum (SHA-256 recommended) for archival verification.
- Generation or capture date.
- Tool, model, model version and settings.
- Prompt ID, exact prompt text and reference inputs.
- Approval state and reviewer notes.
- Parent/derived asset relationships.
- Backup/archive location and whether the file is stored in this repository.

## Rules
- Never overwrite the only approved version with a new generation.
- Keep rejected generations only if they teach us something or are useful alternatives.
- Keep original user-supplied references separate from AI-generated derivatives.
- The asset register must agree with the final shot list and edit decision list.
- Save generated originals immediately outside the AI platform; platform galleries and temporary chat attachments are not reliable backups.
- Store large media in a separately backed-up archive. GitHub should primarily hold prompts, metadata and small essential references; record exact media filenames and recovery paths here.
