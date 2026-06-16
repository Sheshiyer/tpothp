# Episode 01 — Codex GPT Image Command Template

Status: dry-run template only. Do not execute until canon and reference gates are approved.

## Inputs

- Primary identity reference: `pichet.png`
- Anime/stylization reference: `anime-charc.png`
- Optional GLB-derived stills: create from `pichet.glb` if needed before generation.
- Prompt file: `01-prompts/episode-01-arterial-nightmare/gpt-image-character-storyboard-prompt.md`
- Output file: `04-generations/images/episode-01-daily-practice-character-storyboard-board.png`

## Command

```bash
python3 /Users/sheshnarayaniyer/.agents/skills/codex-gpt-image/scripts/codex_gpt_image.py generate \
  --image "/Volumes/madara/2026/twc-vault/01-Projects/tryambakam-noesis/tpothp/pichet.png" \
  --image "/Volumes/madara/2026/twc-vault/01-Projects/tryambakam-noesis/tpothp/anime-charc.png" \
  --prompt "$(cat /Volumes/madara/2026/twc-vault/01-Projects/tryambakam-noesis/tpothp/01-prompts/episode-01-arterial-nightmare/gpt-image-character-storyboard-prompt.md)" \
  --size 1536x1024 \
  --out "/Volumes/madara/2026/twc-vault/01-Projects/tryambakam-noesis/tpothp/04-generations/images/episode-01-daily-practice-character-storyboard-board.png"
```

## Preflight

- Prompt includes Pichet strict identity binding.
- Prompt includes `Not prediction. Reflection. Inquiry. Witness.`
- Prompt maps Episode 01 to the Selemene `daily-practice` workflow.
- No model call has been made yet in this planning pass.
