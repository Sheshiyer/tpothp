# TPoTHP — AI Anime Workflow Automation Blueprint

## Goal

Create a reproducible local-to-cloud workflow for generating TPoTHP symbolic narrative assets.

## Manual First, Automate Later

### Step 1 — Brief

- Write/update `00-brief/series-brief.md`.
- Choose episode and target output.
- Confirm Selemene anchor in `00-brief/current-state-tooling-and-canon.md`.
- Confirm Pichet identity anchors in `02-references/pichet-reference-manifest.md`.

### Step 1.5 — Taste Cortex Retrieval Gate

- Prepare or update `02-references/taste-cortex-ingestion-records.json`.
- Ingest Pichet references, anime workflow references, Noesis visual-system references, and Selemene engine anchors.
- Retrieve nearest style/canon records before final prompt lock.
- Store the retrieval query and selected records in the generation log.

### Step 2 — Prompt Drafting

- Create prompts under `01-prompts/<episode-slug>/`.
- Store:
  - image prompt
  - video prompt
  - voice prompt
  - music prompt

### Step 3 — Still Image Generation

Default backend: local Codex GPT Image.

Dry-run command template:

- `01-prompts/episode-01-arterial-nightmare/codex-gpt-image-command.template.md`

```bash
python3 /Users/sheshnarayaniyer/.agents/skills/codex-gpt-image/scripts/codex_gpt_image.py generate \
  --image "/Volumes/madara/2026/twc-vault/01-Projects/tryambakam-noesis/tpothp/pichet.png" \
  --image "/Volumes/madara/2026/twc-vault/01-Projects/tryambakam-noesis/tpothp/anime-charc.png" \
  --prompt "$(cat 01-prompts/episode-01-arterial-nightmare/gpt-image-character-storyboard-prompt.md)" \
  --size 1536x1024 \
  --out 04-generations/images/episode-01-daily-practice-character-storyboard-board.png
```

### Step 4 — Video Generation

Backend: RunComfy Seedance 2.0 Pro.

Prerequisite:

```bash
runcomfy login
runcomfy whoami
```

Run pattern:

```bash
runcomfy run bytedance/seedance-v2/pro \
  --input-file 01-prompts/episode-01-arterial-nightmare/seedance-input.json \
  --output-dir 04-generations/video/episode-01
```

Use `01-prompts/episode-01-arterial-nightmare/seedance-input.template.json` as the non-secret starting file. Replace the placeholder `image_url` only after the still image exists at a public URL accepted by RunComfy.

### Step 5 — Logs

For every generation, copy `logs/generation-log-template.md` into a dated log file and fill:

- backend
- model
- prompt path
- input references
- output file
- seed / size / duration
- result notes

### Step 6 — Delivery

Copy final clips/images to `07-deliverables/` with clean names.

## Future Make/n8n Pipeline

1. Watch `01-prompts/` for approved prompt files.
2. Generate image via Codex or RunComfy GPT Image 2.
3. Upload generated image to public/reference storage if needed by RunComfy.
4. Generate Seedance video via RunComfy.
5. Download outputs into `04-generations/video/`.
6. Trigger review notification.
7. On approval, copy to `07-deliverables/` and publish/schedule.
