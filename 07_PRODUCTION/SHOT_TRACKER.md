# Shot Tracker

This is the master index of story shots. Every shot used in the final video must have a unique ID and a detailed specification based on [the shot specification template](../06_AI_PROMPTS/SHOT_SPECIFICATION_TEMPLATE.md). This index is not a substitute for the detailed shot sheets.

| Shot ID | Sequence | Timeline in | Timeline out | Duration | Status | Selected local asset | Shot specification |
|---|---|---:|---:|---:|---|---|---|
| INT-001 | Intro / bathroom opening | 00:00.000 | TBD | TBD | Planned | TBD | To be authored |
| INT-002 | Intro / mirror | 00:09.497 | TBD | TBD | Planned | TBD | To be authored |
| INT-003 | Intro / water splash | 00:14.998 | TBD | TBD | Planned | TBD | See reference still prompt below; full shot sheet pending |
| INT-004 | Intro / reflection disappearance | 00:18.676 | TBD | TBD | Planned | TBD | To be authored |

## Existing reference-still prompt

| Prompt ID | Purpose | Prompt file | Status |
|---|---|---|---|
| PROMPT-REF-A-001 | Protagonist in bathroom, water splash, hood up; face visible | [REF-A bathroom prompt](../06_AI_PROMPTS/REFERENCE_STILLS/REF-A_BATHROOM_HOOD_UP.md) | Ready; not generated or approved |

Reference stills are development aids, not automatically final shots. A future AI must be able to generate them from the prompt text without attaching an existing image.

## Status definitions
- Planned: creative intent exists; no asset generation completed.
- Prompt ready: still and/or animation prompt approved for generation.
- Generated: one or more candidate assets exist.
- Selected: candidate chosen for refinement or edit.
- Approved: asset and continuity approved.
- Used in final: confirmed present in the final rendered timeline.

## Timing rules
Use exact timeline in/out values from the final edit, not estimated lyric windows. Preserve source Audacity markers separately. Record frame rate and convert timecode consistently once the edit frame rate is approved. The audio markers are timing anchors, not guaranteed exact vocal boundaries.