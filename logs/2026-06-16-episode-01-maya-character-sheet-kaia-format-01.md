# Generation Log - Episode 01 Maya Character Sheet Kaia Format 01

## Asset

- File: `episode-01-maya-character-sheet-kaia-format-01.png`
- Date/time: 2026-06-16
- Backend: local Codex GPT Image skill via Codex OAuth
- Model: `gpt-image-2`
- Input prompt file: `01-prompts/episode-01-arterial-nightmare/maya-character-sheet-kaia-format-01-prompt.md`
- Reference files:
  - `02-references/ai-anime-storytelling-workflow/media/mayz-big-wave-surfing/2066419938857001187-kaia-character-sheet.jpg`
- Output path: `04-generations/images/episode-01-maya-character-sheet-kaia-format-01.png`
- Seed: not exposed by backend
- Size / aspect ratio: 1672x941 / approximately 16:9
- File size: `2187501` bytes
- SHA-256: `32c6db015087a7810a4b52d5cb66eb790f65fbd3bcf6570d8b4b7deb80eec298`

## Result Notes

- What worked: Maya reads as a child, not an older anime protagonist. The sleepwear, blanket, messy bedtime hair, turnarounds, expression portraits, and personal-object strip are all present.
- What worked: the Kaia sheet's production-board structure translated well while avoiding the beach/sport identity.
- What worked: the rhythm-plaque / biorhythm-ring motif is visually clear and gentle enough for Episode 01.
- What improved the pipeline: Maya now has a reference anchor for the two-character Seedance emotional scene.
- Remaining caveat: output dimensions are `1672x941`, not the requested `1536x1024`; this is acceptable for a 16:9 video reference and better aligned with Seedance framing.

## Generation Issue

- First attempt failed with `Error: No image payload found in Codex response.`
- Likely cause: child-character generation plus uploaded Kaia beach/sport reference and overly explicit negative safety wording.
- Fix: sanitized prompt language while preserving child-safe constraints.
- Second attempt succeeded.

## Prompt-Control Lesson

When a layout reference contains adult/teen beach styling but the target character is a child, avoid explicit high-risk negative wording. State the target age, modest wardrobe, and layout-only use positively and keep the negative list focused on broad category drift.
