# Maya Reference Manifest

Created: 2026-06-16
Purpose: lock Maya's first usable identity reference before Episode 01 two-character keyframe and Seedance generation.

## Use Rule

All Maya still-image and video prompts must treat the generated Maya sheet as the current identity anchor. The model may adapt lighting, camera, and environment, but should preserve Maya's child-safe age read, face logic, sleepwear, comfort blanket, tired-but-curious emotional arc, and personal object set.

## Primary Asset

| Asset ID | Path | Role | Format | Dimensions | Bytes | SHA-256 |
|---|---|---|---|---:|---:|---|
| `maya-kaia-format-sheet-01` | `04-generations/images/episode-01-maya-character-sheet-kaia-format-01.png` | primary Maya identity, turnarounds, expressions, objects | PNG | 1672x941 | 2187501 | `32c6db015087a7810a4b52d5cb66eb790f65fbd3bcf6570d8b4b7deb80eec298` |

## Identity Lock

- Maya is a six-year-old South Asian child.
- She wears modest blue sleepwear with loose pale trousers.
- She carries a cream comfort blanket.
- Her hair is dark, slightly messy, and bedtime-real.
- Her emotional range is frightened, listening, confused curiosity, and relieved wonder.
- Her personal objects include comfort blanket, biorhythm drawing, bedside cup, night lamp, stitched moon patch, and brass bell.

## Prompt Binding Language

Use this language when invoking image or video models:

```text
Use the provided Maya character sheet as a strict identity anchor. Preserve Maya's six-year-old child proportions, soft dark eyes, messy bedtime hair, modest blue sleepwear, comfort blanket, cautious-to-curious expression range, and gentle non-magical presence. Do not redesign her into an older character, magical hero, mascot, fashion model, or anime idol.
```

## Negative Identity Constraints

- Do not make Maya older than a small child.
- Do not change her sleepwear into costume, uniform, or fashion styling.
- Do not remove the comfort blanket unless a shot explicitly calls for it nearby.
- Do not give her weapons, magic tools, or heroic action poses.
- Do not make the nightmare into an external monster.
- Do not turn the rhythm witness arc into prophecy or chosen-one power.

## Generation Note

The first Codex GPT Image attempt returned no image payload, likely because the uploaded Kaia reference plus stronger child-safety wording triggered filtering. The prompt was sanitized to avoid risky wording while keeping the child-safe intent, and the second attempt succeeded.
