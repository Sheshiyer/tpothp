# Episode 01 Teaser Storyboard

## Episode: 01 — The Dream in the Artery
## Selemene Engine: Chronos (Time, Cycles, Rhythms)
## Duration: ~20 seconds

---

## Beat-by-Beat Storyboard

### FRAME 1: Brand Open (0-2s)
**Visual:** Tryambakam Noesis logomark centered on void black
**Audio:** Low drone fade-in
**Text:** Subtle "TRYAMBAKAM NOESIS" below mark
**Generation:** GPT Image 2 (text precision)

```
Prompt: Minimalist logo card on pure black background (#070B1D). 
Centered geometric symbol suggesting three eyes or trinity, rendered in 
sacred gold (#C5A017) with subtle emerald (#10B5A7) inner glow. 
Below the symbol, small caps text "TRYAMBAKAM NOESIS" in elegant 
serif typography, gold on black. No other elements. 
Cinematic 16:9 aspect ratio. Dark, sacred, minimal.
```

---

### FRAME 2: Episode Title Card (2-4s)
**Visual:** Episode number and title on parchment-toned background
**Audio:** Score swells subtly
**Text:** "EPISODE 01" above, "THE DREAM IN THE ARTERY" below
**Generation:** GPT Image 2 (text precision)

```
Prompt: Elegant title card with warm parchment texture background (#F0EDE3). 
Centered text layout: "EPISODE 01" in small caps above, elegant serif font.
Below it, larger title "THE DREAM IN THE ARTERY" in sophisticated serif typography.
Sacred gold (#C5A017) text with subtle deep surface (#0E1428) shadow.
Minimal decorative line or flourish separating number from title.
Cinematic 16:9 aspect ratio. Clean, typographic, editorial.
```

---

### FRAME 3: Atmospheric A — Arterial Tunnel (4-9s)
**Visual:** Existing Seedance clip segment — arterial tunnel environment
**Audio:** Score continues, Pichet voiceover begins
**Voiceover:** "Nightmares are not attacks..."
**Source:** Trim from `e5ef985b...mp4` (0:00-0:05)

---

### FRAME 4: Atmospheric B — Clearing Light (9-14s)
**Visual:** Seedance clip segment — plaque clearing, golden light emerging
**Audio:** Voiceover continues
**Voiceover:** "...Sometimes they are pipes, carrying a truth that has nowhere else to go."
**Source:** Trim from `e5ef985b...mp4` (0:05-0:10)

---

### FRAME 5: Thematic Echo — Maya's Question (14-18s)
**Visual:** Seedance clip climax or generated frame — luminous moment
**Audio:** Maya's line as punctuation
**Voiceover:** "If it was scary... why is it shining?"
**Source:** Trim from `e5ef985b...mp4` (0:10-0:14) OR generated frame

**Optional generated frame prompt:**
```
Prompt: A six-year-old South Asian girl in modest sleepwear, seen from behind, 
looking up at a luminous golden light emerging from organic arterial walls. 
Her small hand reaches toward the light. Warm parchment and sacred gold tones 
against deep organic reds and blacks. Cinematic, painterly, Studio Ghibli meets 
Moebius. 16:9 aspect ratio. Sense of wonder, not fear.
```

---

### FRAME 6: Series Close (18-22s)
**Visual:** Fade to void black, series title centered
**Audio:** Score resolves to silence
**Text:** "THE PULSE OF THE HIDDEN PATH" + "tryambakam.noesis"
**Generation:** GPT Image 2 (text precision)

```
Prompt: Minimalist end card on pure black background (#070B1D).
Centered text: "THE PULSE OF THE HIDDEN PATH" in elegant small caps,
sacred gold (#C5A017) serif typography. Below it, smaller text 
"tryambakam.noesis" in clean sans-serif. Subtle coherence emerald (#10B5A7) 
underline or accent. No other elements. Cinematic 16:9 aspect ratio.
Dark, sophisticated, final.
```

---

## Audio Timeline (Retimed)

```
0s        2s        4s        9s        14s       18s       22s
|---------|---------|---------|---------|---------|---------|
[DRONE FADE IN  ][SCORE SWELL                              ]
                          [PICHET VO: "Nightmares...truth"]
                                            [MAYA: "If it was scary..."]
                                                          [RESOLVE]
```

### Voiceover Timing
- **Pichet line:** Start at 4.5s, end at ~11s (slower, contemplative)
- **Maya line:** Start at 14.5s, end at ~17s (questioning, wonder)
- **Total VO:** ~9 seconds over 22 second teaser

---

## Generation Queue

| Frame | Model | Priority |
|-------|-------|----------|
| Frame 1: Brand Open | GPT Image 2 | High |
| Frame 2: Episode Card | GPT Image 2 | High |
| Frame 6: Series Close | GPT Image 2 | High |
| Frame 5: Maya Wonder (optional) | Nano Banana 2 | Medium |

---

## Assembly Notes

1. Generate title card frames first (Frames 1, 2, 6)
2. Extract Seedance clip segments for Frames 3, 4, 5
3. Re-record or retime Pichet voiceover (slower, more pauses)
4. Assemble with FFmpeg:
   - Frame 1 (2s) → Frame 2 (2s) → Clip A (5s) → Clip B (5s) → Clip C (4s) → Frame 6 (4s)
5. Mix audio: score full-length, voiceover at marked timecodes
6. Export to `07-deliverables/teaser-episode-01-v1.mp4`
