# B Studio Workflow — YOUNES STICKS STUDIO

## Purpose
B Studio is the user's chosen editing and review destination. YOUNES STICKS STUDIO remains the independent episode-production skill: story, character continuity, storyboard, prompts, voiceover, asset organization, and delivery notes.

Official B Studio repository: https://github.com/bassam-pt95/edit-studio

## License and separation (mandatory)
- Install and use B Studio only from its official repository and under its own license.
- Do not copy, vendor, redistribute, patch, reverse-engineer, or reproduce B Studio files, code, UI, internal project formats, scripts, or bundled skills in this repository.
- Do not build a replacement editor or a software extension on top of B Studio.
- Do not remove or hide B Studio branding, attribution, guide, or icon.
- Keep this repository's workflow as a documented handoff to the separately installed official B Studio tools.
- If the user requests a change to B Studio itself, direct them to the official repository Issues page; do not implement the change here.

## What B Studio can safely do in this workflow
Use its official installed `edit-studio` skill to open/review a rendered MP4, make supported timeline refinements, add or adjust captions, images and audio where the official workflow supports them, collect review notes, and export the result.

The official `video-edit` skill is designed around Arabic talking-head montage and its own source/work structure. A Younes stickman animation is not automatically a talking-head project. Do not feed an arbitrary animation folder into that workflow or pretend it can convert it into a fully editable project.

## Handoff decision
1. **A rendered episode MP4 exists:** ask the official `edit-studio` skill to open it as a final-only project using its documented workflow. Explain that elements already rendered into the MP4 are baked in; supported overlays, trims, captions, and audio additions may still be editable.
2. **Only separate shot clips, stills, voiceover, and sound assets exist:** keep them organized in the episode folder and finish/assemble them with a separately approved toolchain. Do not claim B Studio can ingest the folder as a native multitrack project unless its official documentation explicitly adds that capability.
3. **The user asks for the full B Studio-native editable project:** inspect the current official documentation first. If the documented workflow does not support the Younes asset structure, explain the limitation and offer the final-MP4 handoff instead.

## Episode handoff package
Every completed episode should contain:
- `exports/younes-episode-XX-review.mp4` — review/export candidate (when actually rendered).
- `audio/voiceover.wav` or the actual recorded voice file.
- `assets/` — approved shot renders, backgrounds, and sound effects.
- `EDIT_NOTES.md` — timecoded requests for B Studio refinements.
- `DELIVERY_STATUS.md` — what was rendered, what was opened in B Studio, what was edited, and what was actually exported.

Only list files that really exist. Never claim B Studio was opened, an edit was applied, or a final export was made unless the action completed and the output was checked.

## First-time setup
If B Studio is not installed, direct the user to its official README and let the official installer/skill handle installation. Do not manually copy its private files into this repository. Ask permission before installing tools, downloading large models, using paid credits, or making any external publication.

## Quality gate
Before handing off:
- Verify the MP4 exists, duration and dimensions are known, audio is present when expected, and playback is checked.
- Check that Younes matches the approved reference image in every generated shot.
- Check scene order, timing, transitions, voiceover sync, captions, and sound levels.
- Record unresolved issues in `EDIT_NOTES.md`.
- After B Studio work, verify the exported file exists and is playable before marking delivery complete.
