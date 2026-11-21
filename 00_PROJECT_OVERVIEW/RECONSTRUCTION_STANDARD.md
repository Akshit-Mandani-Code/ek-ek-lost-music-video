# Reconstruction Standard — The Repository Must Outlive the Video

## Purpose
This repository is the durable **text-only reconstruction blueprint** for the music video. It must remain useful if the finished export, editing project, generated media or original AI services are lost.

A future creator or AI assistant should be able to use this repository together with any recoverable external media assets to rebuild a version as close as reasonably possible to the approved video. The repository itself intentionally contains no media files.

## Strict repository boundary
This GitHub repository stores text documentation and metadata only. Never commit or upload images, video, audio, rendered frames, thumbnails, DaVinci project binaries, archives or other media assets. Store all media in the separately backed-up external asset archive. GitHub records asset IDs, exact filenames, metadata, checksums and external recovery paths only.

## What “reconstructable” means
The documentation must preserve enough information to reproduce the song version, duration and exact edit range; complete narrative and scene order; every shot's duration, timeline position and music relationship; character identity and wardrobe; locations, props, lighting and cinematography; exact prompts and negative constraints; first/last frames; motion and timing; editing decisions; generation tools/settings; and asset recovery paths.

## Reproducibility tiers
1. **Exact recovery** — original file exists in the external archive or backup; reuse it.
2. **Reference-guided recreation** — original output is unavailable, but approved external reference images, prompts and settings are preserved.
3. **Specification-only recreation** — no original media remains; recreate from detailed written specifications.
4. **Approximation** — a tool cannot reproduce a detail; preserve story function, framing and emotional intent.

AI outputs are stochastic. Different tools, models and versions will not produce pixel-identical results. The goal is the closest practical match, not a promise of identical output.

## Required record for every final shot
Each final shot must have a unique ID and a shot document or complete shot entry containing:
- Shot ID and status (planned / generated / selected / approved / used in final edit).
- Timeline in/out, duration and source music/lyric marker.
- Narrative purpose and emotion.
- Location, time, characters, wardrobe and props.
- Framing, camera angle, lens/look, composition and focus.
- Lighting, palette, atmosphere and visual effects.
- Exact master image prompt and model-specific prompt actually used.
- Exact animation prompt and negative prompt actually used.
- First-frame, last-frame and approved output asset IDs plus external paths.
- Tool, model, version/date, settings, aspect ratio, seed if available, reference inputs.
- Clip trim, speed, transition and grading notes.
- Known defects, fixes and fallback approach.

## External media preservation policy
Store all media outside GitHub in a separately backed-up archive. Keep original files unchanged and use stable asset IDs and filenames. Record exact filenames, archive paths, checksums where practical, dimensions, duration, format and backup status in the text asset register. Never rely on an AI platform gallery, temporary URL or chat attachment as the only copy.

## Tool independence
For every prompt, preserve the model-agnostic creative master prompt, exact prompt submitted to the tool, tool/model/version/settings, reference asset identifiers and input order, and notes describing model deviations or failures.

## Completion gate
The project is not reconstruction-ready until every final timeline shot is documented, all used media assets are recoverable externally or have recreation instructions, the edit timeline can be rebuilt from the EDL, audio source and final range are identified, continuity references are available externally, and a new person can rebuild the video without undocumented chat history.
