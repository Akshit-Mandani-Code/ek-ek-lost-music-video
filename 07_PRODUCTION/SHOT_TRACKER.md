# Shot Tracker

This is the master index of planned story shots. It tracks shot identity and production status; the individual shot specification is the place for complete prompts and edit instructions. A shot is not production-ready until its still and animation instructions are complete and approved.

## Planned shot index

| Shot ID | Sequence | Story purpose | Music anchor | Status | Shot specification |
|---|---|---|---|---|---|
| INT-001 | Bathroom / opening | Establish protagonist alone at mirror | 00:00 instrumental | Planned | To be authored |
| INT-002 | Bathroom / mirror | Show exhausted self-recognition | INTRO_L1 00:09.497 | Planned | To be authored |
| INT-003 | Bathroom / confusion | Confusion registers | INTRO_L2 00:12.608 | Planned | To be authored |
| INT-004 | Bathroom / water | Water splash as attempted reset | INTRO_L3 00:14.998 | Prompt exists; shot sheet pending | [REF-A prompt](../06_AI_PROMPTS/REFERENCE_STILLS/REF-A_BATHROOM_HOOD_UP.md) |
| INT-005 | Bathroom / disappearance | Reflection becomes faceless | INTRO_L4 00:18.676 | Planned | To be authored |
| BED-001 | Bedroom / diary | Establish diary and present isolation | Verse 1 | Planned | To be authored |
| STA-001 | Station / wide | Still protagonist against moving crowd | Verse 1 / Bridge 1 | Planned | To be authored |
| MEM-001 | Hackathon memory | Reveal solo achievement | Verse 1 memory | Planned | To be authored |
| MEM-002 | Interview memory | Show repeated rejection through concise fragment | Verse 1 memory | Planned | To be authored |
| MEM-003 | Job / family | Offer letter beside medical papers | Verse 1 memory | Planned | To be authored |
| MEM-004 | University | Admission and loan rejection | Verse 2 memory | Planned | To be authored |
| MEM-005 | Relationship / job | Breakup and departure from settled job | Bridge 1 / Verse 2 | Planned | To be authored |
| BED-002 | Bedroom / dreams | Diary and old ambitions | Verse 2 | Planned | To be authored |
| STA-002 | Station / closer | Intensify isolation with altered framing | Verse 2 / first chorus | Planned | To be authored |
| CHR1-001 | First chorus | Emotional collapse | Chorus 1 | Planned | To be authored |
| CHR1-002 | First chorus / bedroom | Isolation after accumulated fragments | Chorus 1 | Planned | To be authored |
| BRG-001 | Bridge / protagonist | Attempts to hold himself together | Bridge | Planned | To be authored |
| BRG-002 | Bridge / mother | Mother quietly notices | Bridge | Planned | To be authored |
| END-001 | Mother-lap / present | Adult son rests in mother's lap | Final chorus | Planned | To be authored |
| END-002 | Newborn memory | Mother holds newborn in same lap | Final chorus | Planned | To be authored |
| END-003 | Return / tear | Return to present; tear falls naturally | Final chorus | Planned | To be authored |
| END-004 | Return / renewal | Face returns; son opens eyes peacefully | Final chorus / remaining audio | Planned | To be authored |
| END-005 | Final pullback | Quiet ending, no victory pose | Remaining audio / outro | Planned | To be authored |

## Existing prompt inventory

| Prompt ID | Purpose | File | Status |
|---|---|---|---|
| PROMPT-REF-A-001 | Bathroom water splash, hood up, face visible | [REF-A bathroom prompt](../06_AI_PROMPTS/REFERENCE_STILLS/REF-A_BATHROOM_HOOD_UP.md) | Ready for still generation; not generated or approved |

## Status definitions

- Planned: creative intent exists; no prompt or asset generation completed.
- Prompt ready: complete still and/or animation prompt exists and is approved for generation.
- Generated: one or more candidate assets exist.
- Selected: candidate chosen for refinement or edit.
- Approved: visual and continuity review passed.
- Used in final: confirmed present in the final rendered timeline.

## Timing rules

- The music markers in `AUDIO_SECTION_TIMINGS.md` are anchors, not exact vocal end times.
- Do not invent exact in/out points for shots that have not been edited against the full audio.
- Record final timeline in/out and duration only after the audio and edit are verified.
- Once frame rate is selected, use consistent frame-accurate timecode.
- The song continues beyond the labelled final chorus marker at 109.121698 seconds; review the complete audio before final out-point.

## Asset policy

Generated images and videos are stored outside GitHub. Record local filenames or asset IDs only when useful; never upload media or project binaries to this repository.
