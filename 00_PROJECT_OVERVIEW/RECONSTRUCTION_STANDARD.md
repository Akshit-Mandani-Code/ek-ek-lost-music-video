# Reconstruction Standard — The Repository Must Outlive the Video

## Purpose
This repository is the durable source of truth for reconstructing the music video if the finished export, original project files, generated assets, or original AI services are lost.

A future creator or AI assistant should be able to use this repository alone, plus any explicitly listed external assets that remain available, to rebuild a version that is as close as reasonably possible to the approved video.

## What “reconstructable” means
The repository must preserve enough information to reproduce:
- The song version, duration, audio properties and exact edit range.
- The complete narrative, scene order and emotional intent.
- Every shot's duration, timeline position, lyric/music relationship and transition.
- Character identity, wardrobe, age, performance and reference-image provenance.
- Locations, props, set dressing, lighting, color and cinematography.
- The exact generation prompt used for each approved image/video, plus negative constraints.
- The intended first and last frame of animated shots, where relevant.
- Camera motion, subject motion, environmental motion and timing.
- Editing decisions: clip order, trims, speed changes, overlays, compositing, transitions, grading, titles and sound treatment.
- Tool/model/version/settings used at the time, without making those tools mandatory.
- Which assets are essential, optional, replaceable or merely illustrative.

## Reproducibility tiers
Every important asset and decision should be classified:
1. **Exact recovery** — original file is stored or safely backed up; reuse it.
2. **Reference-guided recreation** — original is unavailable, but approved reference images, prompts and settings are preserved.
3. **Specification-only recreation** — no original asset remains; recreate from detailed written specifications.
4. **Approximation** — a tool cannot reproduce a particular detail; preserve story function, framing and emotional intent.

AI outputs are stochastic. Different tools, models and versions will not produce pixel-identical results. The goal is to preserve the creative specification and achieve the closest practical match, not promise identical outputs.

## Required record for every final shot
Each final shot must have a unique ID and a shot document or complete shot entry containing:
- Shot ID and final status (planned / generated / selected / approved / used in final edit).
- Timeline in/out, duration and source music/lyric marker.
- Narrative purpose and emotion.
- Location, time, characters, wardrobe and props.
- Framing, camera angle, lens/look, composition and focus.
- Lighting, palette, atmosphere and visual effects.
- Exact master image prompt and model-specific prompt actually used.
- Exact animation prompt and negative prompt actually used.
- First-frame, last-frame and approved output asset paths/IDs.
- Tool, model, version/date, settings, aspect ratio, seed if available, reference inputs.
- Clip trim, speed, transition and grading notes.
- Known defects, fixes and fallback approach.

## Asset preservation policy
Do not assume GitHub is a good home for every large video. Store small, important text and metadata in Git. Store large media in a separately backed-up asset archive or cloud drive, and record stable filenames, checksums where possible, dimensions, duration, format and location in the asset register. If an asset is essential and can reasonably be committed without repository bloat, it may be stored in the repository.

Never leave a final shot dependent on an unnamed file, temporary browser URL or undocumented AI-generation history.

## Tool independence
For every prompt, preserve:
- A model-agnostic creative master prompt.
- The exact prompt submitted to the tool.
- Tool/model/version and generation settings.
- Reference asset identifiers and input order.
- A short note describing what the model changed or failed to follow.

A future tool adapter may translate the master prompt, but must not silently change the creative intent.

## Completion gate
The project is not “reconstruction ready” until:
- Every final timeline shot is documented.
- All used assets are listed and recoverable or have recreation instructions.
- The edit timeline can be rebuilt from the edit decision list.
- Audio source and exact final range are identified.
- Character/location/prop continuity references are available.
- A new person can follow the README and rebuild the video without relying on undocumented chat history.
