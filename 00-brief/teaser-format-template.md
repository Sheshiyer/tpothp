# TPoTHP Teaser Format Template

## Series: The Pulse of the Hidden Path
**Style:** Love Death + Robots anthology aesthetic  
**Format:** 15-30s cinematic teasers per episode  
**Mode:** Meta-narrative voiceover, not lip-synced dialogue

---

## Teaser Structure (6-Beat Format)

### Beat 1: Brand Open (0-2s)
- **Visual:** Tryambakam logo from `/Branding/logo/2x/Asset 8@2x.png` centered on void black (`#070B1D`)
- **Audio:** Low drone fade-in from score
- **Text:** Logo only (no additional text)

### Beat 2: Episode Card (2-4s)
- **Visual:** Episode number + title on parchment texture (`#F0EDE3`)
- **Audio:** Score continues, subtle swell
- **Text:** 
  ```
  EPISODE [XX]
  [TITLE IN CAPS]
  ```
- **Typography:** Serif, sacred gold accents (`#C5A017`)

### Beat 3: Atmospheric Visual A (4-9s)
- **Visual:** First Seedance clip segment OR generated storyboard frame
- **Audio:** Score builds, first voiceover line begins
- **Text:** None (let visuals breathe)

### Beat 4: Atmospheric Visual B (9-14s)
- **Visual:** Second clip segment OR transition frame
- **Audio:** Voiceover continues or pauses for score
- **Text:** None

### Beat 5: Thematic Echo (14-18s)
- **Visual:** Key symbolic image or clip climax
- **Audio:** Second voice (Maya or thematic line) as punctuation
- **Text:** Optional pull quote overlay

### Beat 6: Series Close (18-22s)
- **Visual:** Fade to void black, series title card
- **Audio:** Score resolves, silence
- **Text:**
  ```
  THE PULSE OF THE HIDDEN PATH
  tryambakam.space
  ```

---

## Visual Language

### Color Palette
| Name | Hex | Use |
|------|-----|-----|
| Void Black | `#070B1D` | Backgrounds, negative space |
| Deep Surface | `#0E1428` | Secondary backgrounds |
| Parchment | `#F0EDE3` | Title cards, text backgrounds |
| Sacred Gold | `#C5A017` | Accents, highlights, type |
| Coherence Emerald | `#10B5A7` | Subtle highlights, Noesis mark |

### Typography
- **Titles:** Serif (Cormorant Garamond, Playfair Display)
- **Body/Credits:** Sans-serif (Inter, DM Sans)
- **Sacred text:** Handwritten or calligraphic flourishes

### Aspect Ratio
- **Primary:** 16:9 (1920x1080 or 1280x720)
- **Vertical variant:** 9:16 for social (1080x1920)

---

## Audio Architecture

### Score Layer
- Full-length ambient bed at -6dB to -9dB
- Genre: Dark ambient, cinematic, organic textures
- No lyrics, no prominent melody — texture and atmosphere

### Voiceover Layer
- Contemplative, unhurried pacing
- Not explaining — evoking
- Pichet as philosophical guide OR neutral narrator
- 2-3 sentences maximum per teaser

### Sound Design Layer (Optional)
- Subtle foley: heartbeats, breath, water, organic sounds
- No sharp transients or jarring cuts

---

## Voiceover Reframing

### Before (Dialogue)
> "Nightmares are not attacks, Maya. Sometimes they are pipes carrying a truth that has nowhere else to go."

### After (Narration)
> "Nightmares are not attacks. Sometimes they are pipes... carrying a truth that has nowhere else to go."

- Remove character address ("Maya")
- Add pauses (ellipsis = breath)
- Shift from speaking-to to speaking-about

### Maya's Line (Thematic Echo)
> "If it was scary... why is it shining?"

- Works as-is — question floats over visuals as hook
- No change needed

---

## Episode Teaser Checklist

- [ ] Brand open frame generated (Noesis mark)
- [ ] Episode title card generated
- [ ] 2-3 atmospheric frames or clips selected
- [ ] Series close frame generated
- [ ] Score selected/generated (15-25s)
- [ ] Voiceover recorded and retimed
- [ ] FFmpeg assembly with proper timing
- [ ] Export to `07-deliverables/teaser-episode-XX.mp4`

---

## Storyboard Frame Requirements

For each episode teaser, generate:

1. **Title Card Frame** — Episode number + title on brand palette
2. **Atmospheric Frame A** — Key visual from episode's Selemene engine theme
3. **Atmospheric Frame B** — Secondary visual or symbolic element
4. **Close Frame** — Series title on void black

Generation approach:
- Title cards: GPT Image 2 (typography precision)
- Atmospheric frames: Nano Banana 2 or Flux 2 Klein (fast, cheap)
- All at 1280x720 for consistency with Seedance output
