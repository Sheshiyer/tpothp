# TPoTHP — AI Anime Storytelling Workflow Plan

Created: 2026-06-15 22:02 IST
Skill: `ai-anime-storytelling-workflow`
Project root: `/Volumes/madara/2026/twc-vault/01-Projects/tryambakam-noesis/tpothp`

## Objective

Use the AI Anime Storytelling Workflow skill to plan, prompt, generate, and organize cinematic anime storytelling assets for TPoTHP.

## Workspace Setup

- [x] Create project output root.
- [x] Create task tracking folder.
- [x] Create prompt/reference/assets/generation/edit/deliverable folders.
- [x] Copy skill reference prompt library and extracted media into project-local references.
- [x] Add current-state tooling and canon orientation.
- [x] Confirm RunComfy auth before any RunComfy video generation.
- [x] Confirm first target Selemene engine anchor.
- [x] Build project-local Pichet asset manifest.
- [x] Prepare Taste Cortex / NVIDIA embedding ingestion records.
- [x] Rewrite first target concept/story brief against current canon.

## Phase 1 — Creative Brief

- [x] Define story title / working title.
- [x] Define core premise and emotional object.
- [x] Define target format: short, episode, trailer, explainer, or asset pack.
- [x] Define aspect ratio and runtime.
- [x] Define output channel: X, YouTube Shorts, YouTube long-form, Patreon, pitch deck, internal prototype.
- [x] Reconcile older 8-episode mythology with current 16-engine Selemene map.
- [x] Decide whether `The Arterial Nightmare` survives as the first proof clip.
- [x] Rewrite `series-brief.md` after the current canon decision.

## Phase 2 — Image Generation Prompts

- [x] Draft GPT Image 2 character/IP sheet prompt.
- [x] Draft storyboard/keyframe board prompt.
- [x] Validate prompt for originality and IP safety.
- [x] Update prompts to use `pichet.glb`, `pichet.png`, and `anime-charc.png` as reference source.
- [ ] Run live Taste Cortex retrieval before prompt lock.
- [ ] Choose final episode title grammar from `00-brief/episode-name-lab.md`.
- [x] Create first moodboard shot prompt from workflow scaffold.
- [x] Add prompt-quality rules for hand/background control.
- [x] Generate first image via local Codex GPT Image by default.
- [x] Store generated images under `04-generations/images/`.
- [x] Generate stricter v2 moodboard image with cleaner hands/background.
- [x] Create reference-style flowboard prompt from workflow thumbnails.
- [x] Generate reference-style vertical flowboard from workflow thumbnails.
- [x] Create Pichet character sheet prompt in Kaia format.
- [x] Generate Pichet character sheet in Kaia format.
- [x] Review final Tryambakam Noesis brand docs for Pichet design polish.
- [x] Create brand-polished Pichet character sheet v2 prompt.
- [x] Generate brand-polished Pichet character sheet v2.
- [x] Build deterministic v3 board for exact typography and grid.
- [x] Render deterministic v3 board to PNG.
- [x] Create design-system v3 image-generation prompt.
- [x] Generate design-system v3 clean art layer.
- [x] Create v4 exact-typography overlay board.
- [x] Render v4 hybrid board with exact typography overlay.
- [x] Create Maya character sheet prompt in Kaia format.
- [x] Generate Maya character sheet in Kaia format.
- [x] Create Maya reference manifest.
- [x] Create first no-typography Pichet + Maya Seedance keyframe prompt.
- [x] Generate first no-typography Pichet + Maya Seedance keyframe still.
- [x] Choose final Episode 01 title grammar.

## Phase 3 — Video Generation Prompts

- [x] Draft Seedance 2.0 / image-to-video prompt.
- [x] Attach generated character/storyboard image as strict visual reference.
- [x] Check RunComfy auth with `runcomfy whoami`.
- [x] Create dry-run Seedance input template.
- [x] Create public GitHub repo for Seedance keyframe hosting.
- [x] Verify public raw GitHub keyframe URL.
- [x] Generate first 4–15s clip via RunComfy Seedance 2.0 Pro.
- [x] Store generated videos under `04-generations/video/`.

## Phase 4 — Audio / Voice / Music

- [x] Draft ElevenLabs voice direction.
- [x] Draft Suno-style score prompt.
- [x] Generate or import audio assets.
- [x] Store generated/imported audio under `04-generations/audio/`.

## Phase 5 — Edit + Delivery

- [ ] Assemble clip/audio references.
- [ ] Create final edit or edit plan.
- [ ] Export deliverable(s) into `07-deliverables/`.
- [ ] Document final prompts, seeds, tools, and file paths.

## Verification Checklist

- [ ] Character identity is consistent across image and video prompts.
- [ ] Negative constraints are present.
- [ ] Runtime and aspect ratio match target platform.
- [ ] Generated files are saved and named predictably.
- [ ] Final output can be reproduced from stored prompts and references.

## Review / Results

Processed existing source docs into project setup, series brief, episode production map, pilot GPT Image prompt, pilot Seedance prompt, voice/music prompts, and automation blueprint. Pending first image generation run.

2026-06-15 continuation pass: added Pichet manifest, Taste Cortex ingestion records, Codex GPT Image dry-run command template, Seedance input template, and Selemene-aligned Episode 01 framing. `runcomfy whoami` initially failed with not-signed-in status.

2026-06-15 naming/auth pass: `runcomfy whoami` now succeeds. Added `00-brief/episode-name-lab.md` with candidate title systems. Canonical episode titles are not replaced yet; next step is choosing the title grammar.

2026-06-15 first image pass: generated `04-generations/images/episode-01-moodboard-shot-01.png` from `pichet.png` and `anime-charc.png` using `01-prompts/episode-01-arterial-nightmare/moodboard-shot-01-prompt.md`. Logged result at `logs/2026-06-15-episode-01-moodboard-shot-01.md`. Main issue: Pichet reads too young; next image iteration should strengthen mature grounded identity.

2026-06-15 v2 image pass: generated `04-generations/images/episode-01-moodboard-shot-01-v2.png` from stricter prompt `01-prompts/episode-01-arterial-nightmare/moodboard-shot-01-v2-prompt.md`. Logged result at `logs/2026-06-15-episode-01-moodboard-shot-01-v2.md`. Prompt-quality rule added at `01-prompts/prompt-quality-rules.md` to reduce hand/tool/background hallucinations.

2026-06-15 reference-style flowboard pass: generated `04-generations/images/episode-01-flowboard-reference-style-01.png` using Pichet references plus the Lost Wind Chime and Big Wave Surfing workflow thumbnails. Logged result at `logs/2026-06-15-episode-01-flowboard-reference-style-01.md`. This is the strongest moodboard direction so far because it matches the source workflow's clean production-board structure.

2026-06-15 Kaia-format character sheet pass: generated `04-generations/images/episode-01-pichet-character-sheet-kaia-format-01.png` using Pichet references plus `2066419938857001187-kaia-character-sheet.jpg`. Logged result at `logs/2026-06-15-episode-01-pichet-character-sheet-kaia-format-01.md`. This is the strongest character identity/prop-lock asset so far.

2026-06-16 brand-polish review: reviewed `brand-docs-final/` and extracted concrete rules for typography, layout, spacing, grid, and visual-system alignment. Added `00-brief/brand-docs-design-review-for-pichet.md`, updated `01-prompts/prompt-quality-rules.md`, and created `01-prompts/episode-01-arterial-nightmare/pichet-character-sheet-brand-polish-02-prompt.md`. Next step is generating `04-generations/images/episode-01-pichet-character-sheet-brand-polish-02.png`.

2026-06-16 brand-polish generation: generated `04-generations/images/episode-01-pichet-character-sheet-brand-polish-02.png` using Pichet references, the Kaia-format Pichet sheet, and selected Tryambakam Noesis dark brand artifacts. Logged result at `logs/2026-06-16-episode-01-pichet-character-sheet-brand-polish-02.md`. This is now the strongest overall design-board asset because it fixes the dark brand system, grid, borders, hierarchy, spacing, and readable label discipline.

2026-06-16 v3 deterministic layout pass: created `05-edits/episode-01-pichet-board-v3.html` and rendered `05-edits/episode-01-pichet-board-v3.png` with Playwright at 1536x1024. Added `01-prompts/episode-01-arterial-nightmare/pichet-character-sheet-design-system-03-prompt.md` for the next art-layer generation. Logged result at `logs/2026-06-16-episode-01-pichet-board-v3-deterministic-layout.md`. This is the strongest typography/layout/grid artifact so far, but it still uses crops from the v2 generated art.

2026-06-16 v4 hybrid typography pass: generated clean art layer `04-generations/images/episode-01-pichet-character-sheet-design-system-03.png`, then created and rendered `05-edits/episode-01-pichet-board-v4.html` to `05-edits/episode-01-pichet-board-v4.png`. Logged result at `logs/2026-06-16-episode-01-pichet-board-v4-hybrid-typography.md`. This is now the strongest version because it combines clean generated art with deterministic typography, labels, spacing, and composition.

2026-06-16 Maya identity pass: created `01-prompts/episode-01-arterial-nightmare/maya-character-sheet-kaia-format-01-prompt.md` using the Kaia sheet as layout-only reference. First Codex image attempt returned no image payload, then a sanitized prompt succeeded. Generated `04-generations/images/episode-01-maya-character-sheet-kaia-format-01.png` at 1672x941. Added `02-references/maya-reference-manifest.md` and logged result at `logs/2026-06-16-episode-01-maya-character-sheet-kaia-format-01.md`. Maya is now sufficiently identity-locked for two-character Episode 01 keyframe ideation.

2026-06-16 Seedance keyframe prep: live Taste Cortex retrieval remains unresolved because this project only has prepared ingestion records and no runnable retrieval command in the vault. The local `.agents` index exposes NVIDIA NIM probe/client scripts, but not a completed project-local search pipeline for these records. Proceeded with the recorded retrieval queries as documented prompt-lock basis and added `01-prompts/episode-01-arterial-nightmare/seedance-keyframe-01-prompt.md` for one no-typography Pichet + Maya cinematic still.

2026-06-16 Seedance keyframe generation: first Codex request failed with server overload, one retry succeeded. Generated `04-generations/images/episode-01-seedance-keyframe-01.png` at 1672x941, 2637233 bytes, SHA-256 `6eb7361fae1df09a72aae6b0cf890c608048645ad44d7bf1b3816663e9be857f`. Logged result at `logs/2026-06-16-episode-01-seedance-keyframe-01.md`. This is now the best local image reference for the first Seedance run after hosting/uploading to a public URL.

2026-06-16 GitHub public repo pass: initialized a nested repo for the TPoTHP workspace, curated the public surface with `.gitignore`, created `Sheshiyer/tpothp` as a public GitHub repository, pushed `main`, and verified the raw keyframe URL returns `200 image/png`. Public Seedance keyframe URL: `https://raw.githubusercontent.com/Sheshiyer/tpothp/main/04-generations/images/episode-01-seedance-keyframe-01.png`. Logged result at `logs/2026-06-16-github-public-repo.md`.

2026-06-16 Seedance run 01: created `01-prompts/episode-01-arterial-nightmare/seedance-input.json` using the public GitHub keyframe URL. First RunComfy attempt with `bytedance/seedance-v2/pro` failed with 404; live RunComfy docs show the API model id is `bytedance/seedance-2.0/pro`. Reran successfully with request ID `6f21c6f0-4a25-49ee-b720-ac33b9323f5d`. Downloaded `04-generations/video/episode-01/e5ef985b222de7858d80763a7873b4a3_1781627474_siay9jex.mp4`, 1280x720, 24 fps, 15.092971s, AAC audio, SHA-256 `bbbda4f8f77107f12597f56f07c064435e5326fdab07cfeeb5af007e2e0856e3`. Logged result at `logs/2026-06-16-episode-01-seedance-run-01.md`.

2026-06-16 Audio generation pass: generated Episode 01 score via ElevenLabs Music on RunComfy (`elevenlabs/elevenlabs/music-generation`, request ID `f4bc9b6a-dda7-4340-afd0-c0cdb8989f8b`). Generated Pichet voice line via Composio ElevenLabs TTS using Chris voice (charming, down-to-earth). Generated Maya voice line using Jessica voice (playful, bright, warm). All three audio files stored under `04-generations/audio/episode-01/`: score (15.05s), Pichet line (5.80s), Maya line (2.88s). Logged result at `logs/2026-06-16-episode-01-audio-generation.md`.
