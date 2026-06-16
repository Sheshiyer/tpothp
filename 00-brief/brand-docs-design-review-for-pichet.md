# Brand Docs Design Review for Pichet Sheet

Reviewed: 2026-06-16
Source folder: `/Volumes/madara/2026/twc-vault/01-Projects/tryambakam-noesis/brand-docs-final/`

## Diagnosis

The current Pichet Kaia-format sheet is useful as an identity and prop-lock asset, but it is only about 40 percent aligned as a Tryambakam Noesis brand artifact.

It works as illustration reference because Pichet reads mature, grounded, and practical. It fails as design because the page still reads like a generic anime concept sheet: cream board, loose panel sizing, pseudo-text, weak hierarchy, and insufficient relationship to the Tryambakam Noesis visual system.

## Brand System Extracted

Primary brand doctrine from `brand-docs-final/tryambakam-noesis-aleph/06-visual-identity.md`:

- Visual philosophy: bioluminescent, not fluorescent.
- Structural rule: architectural, not decorative.
- Data rule: sacred geometry is information visualization, not ornament.
- Canvas: Void Black `#070B1D`.
- Surface: Deep Surface `#0E1428`.
- Text: Parchment `#F0EDE3`.
- Secondary text: Muted Silver `#8A9BA8`.
- Accent: Sacred Gold `#C5A017`.
- Signal: Coherence Emerald `#10B5A7`.
- Flow state: Flow Indigo `#0B50FB`, accent only unless paired with Parchment.
- Display type: Panchang, wide industrial-panoramic.
- Body type: Satoshi, geometric modernist.
- Data type: SF Mono, for technical metrics and engine data.
- Type scale: 10, 12, 16, 26, 42, 68, 110px.
- Wordmark rule: all caps, Panchang, wide tracking.
- Geometry rule: 0.5px to 1px Sacred Gold lines at low opacity.
- Social/card rule: Void Black background, Panchang headers, Satoshi body, Sacred Gold accents only.

## What To Fix Next

### Typography

- Replace pseudo-label noise with a small number of exact, readable labels.
- Use Panchang-style all-caps only for `PICHET`, `DAILY PRACTICE`, and major module titles.
- Use Satoshi-style small labels for short descriptive lines only.
- Use SF Mono-style data labels for engine tags, coordinates, metric strips, and prop callouts.
- Add letterspacing to all-caps labels.
- Do not ask the image model for paragraphs or dense UI copy.

### Layout

- Stop using the cream open concept-sheet canvas as the dominant surface.
- Use a Void Black master board with Deep Surface modules.
- Use a strict 12-column modular grid with consistent gutters.
- Use sharp rectangular modules, not rounded panels.
- Use generous outer margins and consistent internal padding.
- Use fewer, larger modules rather than many tiny tiles.

### Spacing

- Outer margin target: 48px equivalent.
- Primary gutter target: 24px equivalent.
- Module padding target: 24px to 32px equivalent.
- Bottom equipment strip should breathe: six objects maximum, isolated in equal cells.
- Portrait/expression modules need equal crop boxes and consistent baseline alignment.

### Grid

- Board should resolve into a clear hierarchy:
- Left 5 columns: hero panel.
- Center 3 columns: identity, title, palette, engine tags.
- Right 4 columns: turnarounds and expressions.
- Bottom full width: equipment strip and rhythm-plaque detail.

### Aesthetic Direction

- Dark field, not white studio board.
- Sacred Gold linework as grid and module frame.
- Coherence Emerald glow only from symbolic objects, not everywhere.
- Workwear colors remain Pichet-specific but should be subordinated to brand tokens.
- No fake text blocks, fake logos, UI scribbles, or tiny unreadable paragraphs.

## Next Prompt Strategy

Do not simply regenerate the Kaia sheet with more detail. Generate a branded production board that uses the existing Pichet sheet as identity source and the brand docs as art-direction source.

The next prompt should request:

- exact 16:9 dark brand board
- strict modular grid
- controlled label set
- Pichet identity consistency from existing references
- limited symbolic geometry
- brand palette and type hierarchy
- fewer panels and more whitespace

If the image model still produces weak text, the next production approach should be a two-stage workflow: generate a label-free dark board, then overlay exact typography manually in SVG/HTML or a design tool.
