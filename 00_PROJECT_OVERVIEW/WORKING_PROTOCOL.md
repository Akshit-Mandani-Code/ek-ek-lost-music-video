# Working Protocol — Chat, Prompts and Reference Assets

## 1. Two connected workspaces
- **ChatGPT conversation:** creative discussion, decisions, reviews and iteration.
- **GitHub repository:** durable source of truth. Approved decisions, production prompts, shot specifications, asset records and reconstruction instructions must be committed here.
- Chat history is not the only place where a production-critical prompt or decision may exist.

## 2. Prompt write-through rule
Whenever a production prompt is written in the conversation:
1. Save the complete prompt in the relevant folder/file in this repository during the same working session.
2. Preserve the exact prompt text; do not silently shorten it in GitHub.
3. Give it a prompt ID, version, purpose, status and intended reference inputs.
4. If the prompt is revised, preserve the previous version or record the change clearly; do not erase the history of a prompt that produced an asset.
5. Store the model-agnostic master separately from any tool-specific adaptation and record the exact submitted version.
6. Tell the user which repository file was updated and link it.

This applies to image prompts, image-to-video prompts, text-to-video prompts, editing/compositing instructions and other production-critical prompts. Casual brainstorming fragments do not need archiving unless they become a usable production instruction.

## 3. Reference-image availability protocol
Never assume a previous image output will be available in a later session or on another platform.

Before writing a prompt that depends on an earlier image, identify the reference inputs by asset ID and check whether the actual image is available to attach/upload in the current tool.

Use this priority order:
1. **Original reference available:** attach the exact approved image and identify it by asset ID in the prompt.
2. **Approved derivative available:** use it only if its asset record says it is an approved reference for that purpose; record the parent asset.
3. **Image unavailable, written specification exists:** use the character/location/wardrobe bible and describe the continuity details explicitly. Mark the prompt as specification-only, not image-reference-guided.
4. **Critical identity cannot be reliably described:** pause and ask the user to retrieve or re-upload the original reference before generating. Do not pretend a text description can preserve an exact face.

## 4. Asset preservation routine
When an image or video is generated:
- Save the original output immediately to the user's local project archive.
- Keep the original unedited; create derivatives as separate files.
- Use stable filenames based on asset ID and version.
- Record the exact filename, dimensions, format, generation tool/model, date, prompt ID, reference inputs, approval status and backup location in `07_PRODUCTION/ASSET_REGISTER.md`.
- Maintain at least one backup outside the generation platform. A platform gallery or temporary chat attachment is not a reliable archive.
- GitHub is primarily for text, prompts, metadata and small essential references. Do not commit large video files or fill the repository with every rejected variation. Store media in a separately backed-up folder/cloud location and record its exact path.
- For essential small reference images, committing a copy to the repository may be considered, provided repository size and rights allow it.

## 5. Standard local archive layout
Use a matching folder structure on the user's computer or chosen cloud drive:
```text
Ek-Ek-Lost-Assets/
  00_Original_References/
  01_Character_References/
  02_Location_And_Prop_References/
  03_Generated_Stills/
  04_Generated_Video/
  05_Approved_Exports/
  06_DaVinci_Project_And_Proxies/
```
This is a recommended archive layout, not a claim that these folders already exist.

## 6. When a reference is missing
Do not block all production automatically. Decide whether the missing reference is:
- **Identity-critical:** protagonist face, mother face, or another recurring identifiable person. Prefer retrieving the original.
- **Continuity-important:** hoodie, room, key prop or recurring set. Use a saved image if possible; otherwise use the written continuity bible and label the result as a recreation.
- **Mood-only:** lighting inspiration, atmosphere or generic composition. A written description may be sufficient.

Never label a newly generated approximation as the original approved reference.

## 7. Prompt and asset status vocabulary
- `DRAFT`: being discussed; not ready to generate.
- `READY`: prompt is complete and can be used.
- `GENERATED`: output exists but has not been reviewed.
- `SELECTED`: preferred candidate, pending final continuity approval.
- `APPROVED`: accepted as a canonical reference or production asset.
- `REJECTED`: not to be used, with reason recorded when useful.
- `SUPERSEDED`: replaced by a newer approved version; retain its history.

## 8. Session handoff checklist
At the end of a meaningful production session:
- Commit new prompts and approved decisions.
- Update asset and shot trackers.
- Identify which source images must be attached for the next generation.
- State which required references are currently unavailable.
- Do not ask the user to regenerate an image if a recoverable original should exist; first check the documented archive location.
