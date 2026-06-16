# Generation Log — Episode 01 Moodboard Shot 01 v2

## Asset

- File: `episode-01-moodboard-shot-01-v2.png`
- Date/time: 2026-06-15
- Backend: local Codex GPT Image skill via Codex OAuth
- Model: `gpt-image-2`
- Input prompt file: `01-prompts/episode-01-arterial-nightmare/moodboard-shot-01-v2-prompt.md`
- Reference files:
  - `pichet.png`
  - `anime-charc.png`
- Output path: `04-generations/images/episode-01-moodboard-shot-01-v2.png`
- Seed: not exposed by backend
- Size / aspect ratio / duration: 1536x1024 / 3:2 image output / still image
- SHA-256: `d3ffc01e965865660486d99e7144195c24e093d38a6f1e30df0ef10c72aa17c6`

## Result Notes

- What worked: Pichet now reads as a mature adult worker; the hand/tool design is much cleaner; the bundled-tool hallucination is gone; the background is less chaotic and more readable; the rhythm plaque is clear.
- What improved from v1: stricter hand instructions, one-prop rule, adult identity language, and three-layer background rule all improved output control.
- Remaining caveat: output is 1536x1024 because the current Codex GPT Image route uses that size; treat this as a moodboard/keyframe source, not final 16:9 delivery framing.
- Next iteration: if needed, crop/outpaint to 16:9 after selecting the strongest keyframe; keep the v2 prompt-quality rules for all future Pichet generations.

## Prompt-Control Lesson

Do not ask image models to place multiple tiny tools in Pichet's hands until a locked character sheet exists. Use one visible prop per moodboard shot and keep both hands separated from dense symbolic linework.
