# Generation Log — Episode 01 Reference-Style Flowboard 01

## Asset

- File: `episode-01-flowboard-reference-style-01.png`
- Date/time: 2026-06-15
- Backend: local Codex GPT Image skill via Codex OAuth
- Model: `gpt-image-2`
- Input prompt file: `01-prompts/episode-01-arterial-nightmare/flowboard-reference-style-01-prompt.md`
- Reference files:
  - `pichet.png`
  - `anime-charc.png`
  - `02-references/ai-anime-storytelling-workflow/media/abhishek-lost-wind-chime/2066129327750877653-main-result-thumbnail.jpg`
  - `02-references/ai-anime-storytelling-workflow/media/mayz-big-wave-surfing/2066419213292777835-main-surfing-thumbnail.jpg`
- Reference docs:
  - `02-references/ai-anime-storytelling-workflow/02-ai-animation-factory.md`
  - `02-references/ai-anime-storytelling-workflow/03-gpt-image-seedance-big-wave-surfing.md`
- Output path: `04-generations/images/episode-01-flowboard-reference-style-01.png`
- Seed: not exposed by backend
- Size / aspect ratio / duration: 1024x1536 / vertical flowboard still image
- SHA-256: `d5098f1e804342e47b24e97bd7e0bd2650abd4363b6cd90f1e89748d16085f46`

## Result Notes

- What worked: strongest moodboard structure so far; follows the workflow reference style with top cinematic hero panel, character views, prop panels, storyboard beats, and palette swatches.
- What improved from v1/v2: cleaner tactical layout, much less random background clutter, better production-board utility, fewer hand/tool hallucinations, stronger animation workflow readiness.
- Remaining caveat: still has stylized symbolic marks on Pichet's forehead because that feature is present in prior image outputs/reference drift; decide whether to keep it as Pichet canon or explicitly remove it next pass.
- Next iteration: if refining, keep this layout and only adjust identity/canon details; do not return to single close-up mood shots.

## Prompt-Control Lesson

For this project, reference-style flowboard generation beats standalone keyframe generation. The flowboard format naturally constrains the model into clean panels, fewer arbitrary props, and clearer production-useful structure.
