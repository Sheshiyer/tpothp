# Episode 01 - Pichet Character Sheet Design System 03 Prompt

Purpose: generate a cleaner art layer for the v3 manually typeset board. This prompt should use the deterministic HTML board as the layout reference, but it should not rely on the image model for final typography.

Use with local Codex GPT Image and these references:

- `pichet.png` as Pichet identity anchor.
- `anime-charc.png` as anime stylization reference.
- `04-generations/images/episode-01-pichet-character-sheet-brand-polish-02.png` as current Pichet content reference.
- `05-edits/episode-01-pichet-board-v3.png` as strict layout, spacing, grid, and hierarchy reference.
- `brand-docs-final/tryambakam-noesis-aleph/06-visual-identity.md` as visual-system authority.

Output target:

- `04-generations/images/episode-01-pichet-character-sheet-design-system-03.png`

## Prompt

```text
Create one horizontal 16:9 Pichet production board for Tryambakam Noesis using the provided v3 board image as strict layout reference.

The priority is layout quality, not more detail. Preserve the v3 board's design system: exact dark master canvas, generous outer margin, three-column top structure, full-width bottom repair-kit structure, right rhythm-plaque module, sharp rectangular modules, consistent gutters, Sacred Gold borders, Deep Surface panels, and disciplined negative space.

IMPORTANT TYPOGRAPHY RULE
Do not invent dense typography. Keep all text zones clean and minimal. Use only short clean heading placeholders where shown in the v3 reference. Do not add pseudo-writing, fake paragraphs, fake UI labels, or random annotation text. The final typography will be manually typeset outside the image model.

BRAND SYSTEM
Canvas: Void Black #070B1D.
Panel surface: Deep Surface #0E1428.
Primary text zones: Parchment #F0EDE3.
Secondary marks: Muted Silver #8A9BA8.
Accent borders and sacred geometry: Sacred Gold #C5A017.
Small internal glow only: Coherence Emerald #10B5A7.
Use Flow Indigo #0B50FB only as tiny data-flow accent.

GRID AND SPACING
Use the v3 reference board's modular grid exactly:
- large hero panel on the left
- identity stack in the center
- turnaround and expression modules on the right
- repair-kit strip across the lower left and center
- rhythm-plaque module on the lower right
Maintain consistent gutters, consistent border weight, and generous padding inside every module. No cramped content. No loose scrapbook layout.

PICHET IDENTITY
Pichet is a mature South Asian working adult in his late 30s to early 40s. He is grounded, weathered, practical, and humble. Work cap, tied-back dark hair, light stubble, calm eyes, rolled sleeves, dark utility overalls, tool belt, worn trousers, practical boots. He must not look like a child, teen protagonist, guru, monk, superhero, mascot, or cyberpunk fighter.

PANEL CONTENT
Left hero: Pichet in a living arterial corridor, one open palm listening to the wall, one brass pressure gauge held low and clear. The scene is dark-field, internally lit by Sacred Gold vascular geometry and tiny Coherence Emerald rhythm nodes. Clean and architectural, not cluttered.

Center identity: one clean Pichet standing study plus brand palette swatches. Keep this area clean and spacious. No duplicate side figures. No cropped body parts. No extra props.

Right top: four clean full-body turnarounds on a dark Deep Surface field: front, side, back, three-quarter. Consistent scale and baseline.

Right middle: four expression portraits in equal crop boxes: listening, concerned, gentle half-smile, focused repair mode. Mature face, restrained anime realism, no oversized childish eyes.

Bottom strip: exactly six repair-kit cells, each isolated and centered: brass pressure gauge, copper wrench, folded cloth, repair chalk, sealing thread spool, utility pouch. No hands, no extra tools, no overlap.

Lower right rhythm plaque: black-violet oval plaque with sparse Sacred Gold biorhythm rings and a small Coherence Emerald core glow. Sacred geometry as data visualization, not decoration.

AESTHETIC TARGET
This should feel like a premium brand bible board, not a generic character sheet. Dark-field. Architectural. Precise. Quietly mythic. Tryambakam Noesis first, Pichet second, anime production third.

NEGATIVE CONSTRAINTS
No cream dominant background. No generic anime whiteboard. No pseudo-writing. No dense labels. No fake UI. No logos. No rounded cards. No wellness aesthetic. No chakra rainbow. No third-eye cliche. No lotus cliche. No excessive neon. No cyberpunk. No busy micro-architecture. No extra hands. No fused fingers. No tool bundle in hand. No weaponized tools. No copied unrelated reference content.
```
