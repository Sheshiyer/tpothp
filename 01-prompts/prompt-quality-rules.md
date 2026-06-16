# Prompt Quality Rules

## Anti-Hallucination Rule

When generating Pichet stills, avoid asking for many small objects in the hands. Small bundled tools, rods, charms, cables, gauges, and tuning forks increase the chance of fused fingers and invented mechanics.

Prefer:

- exactly two visible hands
- one hand open and relaxed
- one hand holding exactly one simple prop
- simple prop silhouette
- breathing room around hands
- no overlapping fingers and tools

## Background Readability Rule

Dense anatomical-city backgrounds should be layered, not cluttered.

Use three layers:

1. foreground subject and immediate problem
2. middle-distance symbolic/environmental shape
3. far background atmosphere

Avoid:

- tiny windows everywhere
- tangled pipes everywhere
- illegible pseudo-symbols
- random scaffolds
- noisy micro-architecture
- diagrams crossing faces or hands

## Pichet Identity Rule

Every prompt must explicitly say Pichet is a mature South Asian working adult in his late 30s to early 40s. Avoid broad anime language that lets the model drift into a young protagonist.

Use:

```text
Pichet must read as a mature South Asian working adult in his late 30s to early 40s, not a child, teenager, mascot, or generic young anime protagonist.
```

## Prop Rule

For moodboard shots, use only one foreground prop at a time:

- pressure gauge
- wrench
- tuning fork
- repair chalk

Do not combine multiple hand-held props until the character sheet has locked the design.

## Brand Layout Rule

When generating a Tryambakam Noesis production board, do not default to a cream anime concept-sheet canvas.

Use:

- Void Black `#070B1D` master canvas
- Deep Surface `#0E1428` modules
- Parchment `#F0EDE3` primary text
- Muted Silver `#8A9BA8` secondary text
- Sacred Gold `#C5A017` borders and geometry
- Coherence Emerald `#10B5A7` only as small internal glow
- sharp rectangular modules
- 12-column grid logic
- consistent gutters and generous margins

Avoid:

- loose whiteboard layouts
- rounded generic cards
- many tiny panels
- fake UI blocks
- decorative sacred geometry without structural purpose

## Typography Rule

For generated sheets, ask for only a small number of exact labels. Image models are weak at dense typography.

Use the brand hierarchy:

- Panchang-style wide all-caps for one or two major headings
- Satoshi-style for short body labels
- SF Mono-style for tiny data tags

Avoid:

- paragraphs of generated text
- pseudo-writing
- fake brand names
- dense annotation clusters
- random microcopy in small panels

## Child Character Rule

When generating Maya, explicitly prevent the model from inheriting teen, glamour, or body-emphasis cues from style references.

Use:

- six-year-old child
- modest sleepwear
- child-safe proportions
- frightened-to-curious emotional acting
- comfort blanket as the one main prop
- no swimsuit logic even if a layout reference contains beachwear

Avoid:

- exposed midriff
- teen styling
- idol / glamour facial language
- fashion-model stance
- makeup
- magical-girl costume
- adult body proportions
