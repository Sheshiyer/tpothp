# TPoTHP — The Plumber of the Human Psyche

This repository contains the public production workspace for the first TPoTHP proof-of-world clip in the Tryambakam Noesis ecosystem.

Active Episode 01 title: **The Dream in the Artery**.

Legacy working title: `The Arterial Nightmare`.

## Public Seedance Reference

Current keyframe image for RunComfy Seedance:

`https://raw.githubusercontent.com/Sheshiyer/tpothp/main/04-generations/images/episode-01-seedance-keyframe-01.png`

Local source path:

`04-generations/images/episode-01-seedance-keyframe-01.png`

Use this URL in `image_url` for `bytedance/seedance-v2/pro`.

## Folder Map

- `tasks/` — plan, checklist, review notes, lessons.
- `00-brief/` — creative briefs, concepts, target format decisions.
- `01-prompts/` — generated prompt drafts and final prompts.
- `02-references/` — copied skill references, examples, extracted X media.
- `03-assets/source-media/` — user-provided or imported source media.
- `04-generations/images/` — generated stills, character sheets, storyboard boards.
- `04-generations/video/` — generated video clips.
- `04-generations/audio/` — voice, SFX, score, and music assets.
- `05-edits/` — edit projects, assembly notes, intermediates.
- `06-automation/` — Make/n8n/Zapier workflow plans and payload schemas.
- `07-deliverables/` — final exported outputs.
- `logs/` — generation logs and backend metadata.

## Default Backend Routing

- Still images: local Codex GPT Image skill.
- Explicit RunComfy GPT Image 2: `runcomfy run openai/gpt-image-2/text-to-image`.
- Image-to-video / Seedance: RunComfy Seedance 2.0 Pro after auth.

## Next Step

Host the keyframe through this public repository, then run the Seedance 2.0 Pro payload using the raw GitHub image URL.

Private source documents, copied workflow example media, local credentials, and raw source media are intentionally excluded from this public repo.
