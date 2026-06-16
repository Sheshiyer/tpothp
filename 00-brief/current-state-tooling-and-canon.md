# Current State Tooling And Canon

Created: 2026-06-15
Project root: `/Volumes/madara/2026/twc-vault/01-Projects/tryambakam-noesis/tpothp`

## Status

This workspace is still in planning, processing, and tooling setup. Do not generate final images or video until the canon, reference pack, retrieval layer, and payload files are aligned.

## Current Goal

TPoTHP is not a standalone anime experiment. It is the symbolic narrative layer for current Tryambakam Noesis and Selemene Engine.

The goal is to create a proof-of-world workflow where Pichet makes Selemene's mirrors felt through story: not prediction, not guru instruction, but reflection, inquiry, witness, and self-authorship.

## Current Canon

- Selemene Engine is the live computational core: 16 engines, 6 workflows, API, SDK, TUI, and web surfaces.
- Tryambakam Noesis is the larger field: computation, somatic content, symbolic narratives, physical anchors, and initiation.
- The older 8-episode body/chakra arc is raw mythology, not final production canon.
- The updated Plumber direction should map episodes or clips to Selemene engine themes and Noesis initiation states.
- Pichet should remain practical, humble, and repair-oriented. He is not a guru, superhero, or chosen savior.
- Every generated artifact must preserve the Noesis distinction: engine outputs orient; the user authors.

## Tooling Stack

### 1. Local Workflow Skill

Primary planning skill:

`/Users/sheshnarayaniyer/.craft-agent/workspaces/my-workspace/skills/ai-anime-storytelling-workflow/`

Use its reference library for structure:

- `references/01-gpt-image-seedance-lost-wind-chime.md`
- `references/02-ai-animation-factory.md`
- `references/03-gpt-image-seedance-big-wave-surfing.md`
- `references/04-universal-templates.md`
- `references/05-media-manifest.md`
- `references/media/`

### 2. Taste Cortex / NVIDIA Embedding Layer

Use the custom design-memory retrieval layer before locking prompts.

Observed implementation lineage:

- `brandmint-design-memory` style asset ingestion and search.
- NVIDIA embeddings through `/embeddings`.
- Model candidate lineage includes `nvidia/nv-embed-v1` and related NVIDIA embedding families.
- Asset records should include project, brand, source, asset id, aspect, caption, prompt, tags, flows, colors, and SHA-256.
- Search should rank retrieved assets by cosine similarity against the current prompt/design query.

For this project, Taste Cortex should ingest and retrieve:

- Pichet references.
- Anime workflow reference stills and thumbnails.
- Noesis visual-system references.
- Selemene engine-symbol references.
- Prompt drafts and prompt deltas.

### 3. Pichet Reference Pack

Existing root assets:

- `pichet.glb` — GLB model, 44.8 MB.
- `pichet.png` — 1024x1024 PNG.
- `anime-charc.png` — 1024x1024 PNG with alpha.

These are the base reference starting points for Pichet. They should be cataloged before prompt generation and used to stabilize character identity.

### 4. Image Generation

Default still-image route during planning:

- Local Codex GPT Image via `/Users/sheshnarayaniyer/.agents/skills/codex-gpt-image/`.

Use when generating:

```bash
python3 /Users/sheshnarayaniyer/.agents/skills/codex-gpt-image/scripts/codex_gpt_image.py generate \
  --image /absolute/path/to/pichet.png \
  --image /absolute/path/to/anime-charc.png \
  --prompt "<approved prompt>" \
  --size 1536x1024 \
  --out 04-generations/images/<asset-name>.png
```

RunComfy GPT Image 2 remains available, but only when explicitly selected.

### 5. Video Generation

Default video route for strict multimodal reference consistency:

- RunComfy Seedance 2.0 Pro: `bytedance/seedance-v2/pro`.

Prerequisites before any Seedance run:

- `runcomfy whoami` passes.
- The still/reference image is generated and accessible as a URL accepted by RunComfy.
- A `seedance-input.json` exists and contains no secrets.
- Output directory is under `04-generations/video/`.

Use `image-to-video` router only when Seedance is not specifically required.

## Planning Gates

Before generating anything:

1. Rewrite the current brief against current Selemene/Noesis canon.
2. Build a project-local asset manifest for Pichet and references.
3. Run Taste Cortex retrieval or prepare the exact records needed for ingestion.
4. Decide the first proof clip's engine theme.
5. Rewrite image and video prompts using Pichet references and retrieved style references.
6. Create dry-run payload files for still image and Seedance video.
7. Confirm auth/tool readiness without exposing tokens.

## Recommended Next Decision

Current first proof clip anchor:

- Use `The Dream in the Artery` as the active Episode 01 title.
- Keep `The Arterial Nightmare` only as the legacy raw-concept title.
- Reframe it through Selemene's `daily-practice` workflow: Panchanga + Vedic Clock + Biorhythm.
- Visual emphasis: Biorhythm and Vedic Clock, with Panchanga as background timing atmosphere.
- Story premise: a recurring nightmare is not an omen to decode; it is a rhythm interruption Pichet helps Maya witness safely.
- Noesis guardrail: `Not prediction. Reflection. Inquiry. Witness.`

Alternative anchors if this direction is rejected:

- `Temporal Grammar`: show time as qualitative and cyclic.
- `Three-Wave Cycle`: show body rhythm as the first text.
- `Bioelectric Field`: show prana as measurable signal.
- `Synthesis`: show Pichet holding multiple mirrors until the witness emerges.

The old `The Arterial Nightmare` scene survives as source mythology only because it has been reframed around the current `daily-practice` anchor.
