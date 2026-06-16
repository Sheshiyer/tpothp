# Creative Brief — TPoTHP

Use `current-state-tooling-and-canon.md` as the current orientation document. `series-brief.md` is older mythology and should be rewritten against current Selemene/Noesis canon before generation.

## Current Production Target

Planning target: rebuild the first proof-of-world clip around a current Selemene engine theme before generating assets.

## Current Prompt Set

- `01-prompts/episode-01-arterial-nightmare/gpt-image-character-storyboard-prompt.md`
- `01-prompts/episode-01-arterial-nightmare/seedance-video-prompt.md`
- `01-prompts/episode-01-arterial-nightmare/voice-and-music-prompts.md`

## Backend Routing

- Still images: local Codex GPT Image by default.
- Video: RunComfy Seedance 2.0 Pro after `runcomfy login`.

## Current Tooling Gate

- Catalog `pichet.glb`, `pichet.png`, and `anime-charc.png` as Pichet reference inputs.
- Use the custom Taste Cortex / NVIDIA embedding design-memory layer before final prompt lock.
- Use the local `ai-anime-storytelling-workflow` skill references for prompt structure.
- Use RunComfy downstream skills only after prompt, reference, and payload gates are ready.
