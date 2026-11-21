# Working Protocol — Chat, Prompts and External Media

## 1. Two connected workspaces
- **ChatGPT conversation:** creative discussion, decisions, reviews and iteration.
- **GitHub repository:** text-only production blueprint and source of truth for decisions, prompts, shot specifications, metadata, continuity and editing instructions.
- **External media archive:** the only storage location for image, video, audio and other binary production assets. It may be local, cloud-backed or both.
- Chat history and AI-platform galleries are not reliable long-term archives.

## 2. Absolute GitHub media exclusion
**Do not commit, upload, attach through Git, or otherwise store any image, video, audio file, thumbnail, rendered frame, project binary or other media asset in this GitHub repository.**
This applies to original references, generated outputs, rejected variations, approved stills, video clips, song files, exports and DaVinci project files.
GitHub may contain text-only records about those assets: asset IDs, filenames, formats, dimensions, checksums, generation metadata, prompt IDs, approval status and external archive paths.
Prompts and documentation are text and should be committed normally.
If an image is needed as a reference in a future document, use a text asset ID and external path; do not embed or commit the media.

## 3. Prompt write-through rule
Whenever a production-ready prompt is written in the conversation:
1. Save the complete prompt as text in the relevant repository folder/file during the same working session.
2. Preserve exact prompt wording; do not silently shorten it.
3. Give it a prompt ID, version, purpose, status and intended reference inputs.
4. When revising, retain prior versions that have been used or generated outputs; mark superseded versions rather than erasing production history.
5. Store the model-agnostic master separately from tool-specific adaptations and record the exact submitted version.
6. Tell the user which text file was updated and link it.
Casual brainstorming fragments do not need archiving until they become actionable production instructions.

## 4. Reference-image availability protocol
Never assume a previous image output will be available in a later session or on another platform.
Before writing a prompt that depends on an earlier image, identify the reference inputs by asset ID and check whether the actual image can be attached in the current tool.
1. **Original reference available:** attach the exact approved image from the external archive and identify its asset ID in the prompt.
2. **Approved derivative available:** use only if its asset record approves it for that purpose; record its parent asset.
3. **Image unavailable, written specification exists:** use the relevant character/location/wardrobe bible and mark the prompt as specification-only.
4. **Critical identity cannot be reliably described:** pause and ask the user to retrieve or re-upload the original reference. Do not imply that text can preserve an exact face.

## 5. External media archive
- Save each original generated/supplied media file immediately to the external archive, not only to the generation platform or chat.
- Keep originals unchanged; create derivatives as separate files.
- Use stable asset IDs and filenames.
- Maintain a second copy/backup outside the generation platform.
- Record the exact external path or cloud folder reference in `07_PRODUCTION/ASSET_REGISTER.md`.
- GitHub is not a media backup and must never be treated as one.

### Recommended local archive layout
```text
Ek-Ek-Lost-Assets/
  00_Original_References/
  01_Character_References/
  02_Location_And_Prop_References/
  03_Generated_Stills/
  04_Generated_Video/
  05_Approved_Exports/
  06_DaVinci_Project_And_Proxies/
  07_Audio_And_Timing_Exports/
```
This is a proposed structure only; it is not claimed to exist until the user creates it.

## 6. Asset metadata recorded in GitHub
For each important media asset, record stable ID, exact filename, media type, format, dimensions/resolution, frame rate/duration where applicable, file size and SHA-256 checksum when practical, generation date, tool/model/settings, prompt ID, reference asset IDs/input order, approval state, reviewer notes, parent/derived relationships, exact external archive path and backup status.
Do not store the media bytes in this repository.

## 7. Missing-reference categories
- **Identity-critical:** protagonist face, mother face or another recurring identifiable person. Recover the original wherever possible.
- **Continuity-important:** hoodie, room, key prop or recurring set. Use saved reference media if possible; otherwise use the written bible and label the output as a recreation.
- **Mood-only:** lighting, atmosphere or generic composition. A written description may be sufficient.
Never label a newly generated approximation as the original approved reference.

## 8. Prompt and asset status vocabulary
- `DRAFT`: being discussed; not ready to generate.
- `READY`: prompt is complete and can be used.
- `GENERATED`: output exists but has not been reviewed.
- `SELECTED`: preferred candidate, pending final continuity approval.
- `APPROVED`: accepted as a canonical reference or production asset.
- `REJECTED`: not to be used, with reason recorded when useful.
- `SUPERSEDED`: replaced by a newer version; retain history.

## 9. Session handoff checklist
At the end of a meaningful production session, commit new prompts and approved decisions as text, update asset and shot trackers with external media paths, identify which source images must be attached next, state which required references are unavailable, and check documented archive locations before asking the user to regenerate anything.
