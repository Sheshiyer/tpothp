# Pichet Reference Manifest

Created: 2026-06-15
Purpose: lock the current Pichet identity references before any image or video generation.

## Use Rule

All Pichet still-image and video prompts must treat these files as identity anchors, not loose inspiration. The model may adapt rendering style, lighting, camera, and production-board layout, but should preserve Pichet's face logic, silhouette, grounded repair-worker bearing, clothing vocabulary, and tool-world.

## Primary Assets

| Asset ID | Path | Role | Format | Dimensions | Bytes | SHA-256 |
|---|---|---|---|---:|---:|---|
| `pichet-model-glb` | `pichet.glb` | 3D body/silhouette/pose reference | GLB | n/a | 44816716 | `bcba6740b458e65b1f3166ecdd0f0d721ebdb574f5d9080e3c80059d90216c8c` |
| `pichet-primary-portrait` | `pichet.png` | primary face/color/identity reference | PNG | 1024x1024 | 2082252 | `757cb8ebabc0eec3282901d561224f54758e0228ea773b714e2ab33aca75efbb` |
| `pichet-anime-style-reference` | `anime-charc.png` | anime stylization / alpha reference | PNG | 1024x1024 | 1878895 | `18528586bbdf85e6d80498d61d2ac8f7c3c53b6644104c2fa0be90cb1e62f036` |

## Reference Priority

1. `pichet.png` controls face, emotional bearing, and primary identity.
2. `pichet.glb` controls silhouette, grounded physicality, and pose plausibility.
3. `anime-charc.png` controls stylization compatibility and transparent character treatment.

## Prompt Binding Language

Use this language when invoking image or video models:

```text
Use the provided Pichet reference images as strict identity anchors. Preserve Pichet's face logic, calm practical expression, grounded repair-worker posture, outfit vocabulary, tool-belt silhouette, and humble non-guru presence. Do not redesign him into a superhero, monk, mascot, cyberpunk warrior, fantasy wizard, or generic anime protagonist.
```

## Negative Identity Constraints

- Do not make Pichet look younger than a mature working adult.
- Do not replace repair tools with weapons or magic staffs.
- Do not turn sacred-geometry tools into combat gear.
- Do not make him a guru, chosen savior, priest, or action hero.
- Do not drift from practical clothing into ornate fantasy costume.
- Do not remove the grounded plumber/repair-worker read.

## Generation Gate

Before first generation, confirm:

- `pichet.png` and `anime-charc.png` are attached or passed as image references.
- `pichet.glb` has been visually inspected or converted to still references if the target model cannot consume GLB directly.
- Prompt includes the binding language above.
- Prompt includes the Noesis guardrail: `Not prediction. Reflection. Inquiry. Witness.`
- Output path is under `04-generations/images/` or `04-generations/video/`.
