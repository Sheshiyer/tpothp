# Episode 01 — Final Delivery Log

**Date:** 2026-06-16  
**Episode:** 01 — The Dream in the Artery  
**Status:** Proof-of-world complete

---

## Deliverable

| Field | Value |
|-------|-------|
| File | `07-deliverables/episode-01-the-dream-in-the-artery-v1.mp4` |
| Resolution | 1280x720 |
| Duration | 15.04s |
| Size | 7,246,919 bytes (7.1 MB) |
| Video codec | H.264 (copy from source) |
| Audio codec | AAC 192kbps stereo |
| SHA-256 | `69cecb800df23d6a8ced969211c096d0d515a6ce17fa9eaabaea6cc3c1dea5cd` |

---

## Source Assets

### Video
- `04-generations/video/episode-01/e5ef985b222de7858d80763a7873b4a3_1781627474_siay9jex.mp4`
- Generated via RunComfy Seedance 2.0 Pro
- Request ID: `6f21c6f0-4a25-49ee-b720-ac33b9323f5d`

### Score
- `04-generations/audio/episode-01/episode-01-score-01.mp3`
- Generated via RunComfy ElevenLabs Music
- Request ID: `f4bc9b6a-dda7-4340-afd0-c0cdb8989f8b`
- Duration: 15.05s

### Pichet Voice
- `04-generations/audio/episode-01/episode-01-pichet-line-01.mp3`
- Generated via Composio ElevenLabs TTS
- Voice: Chris (`iP95p4xoKVk53GoZ742B`)
- Line: "Nightmares are not attacks, Maya. Sometimes they are pipes carrying a truth that has nowhere else to go."
- Duration: 5.80s

### Maya Voice
- `04-generations/audio/episode-01/episode-01-maya-line-01.mp3`
- Generated via Composio ElevenLabs TTS
- Voice: Jessica (`cgSgspJ2msm6clMCkdW9`)
- Line: "If it was scary... why is it shining?"
- Duration: 2.88s

---

## Mix Timeline

```
0s                    5s                    10s                   15s
|---------------------|---------------------|---------------------|
[VIDEO: Arterial tunnel, Pichet + Maya, plaque clearing]
[SCORE: -6dB ambient bed full length]
         [PICHET: 2.0s-7.8s]
                                      [MAYA: 10.5s-13.4s]
```

---

## Tools Used

| Phase | Tool | Endpoint/Method |
|-------|------|-----------------|
| Video | RunComfy CLI | `bytedance/seedance-2.0/pro` |
| Score | RunComfy CLI | `elevenlabs/elevenlabs/music-generation` |
| Voice | Composio CLI | `ELEVENLABS_TEXT_TO_SPEECH` |
| Mix | FFmpeg 8.1.1 | `amix`, `adelay`, `volume` filters |

---

## Verification Checklist

- [x] Character identity consistent (Pichet grounded repair-oriented, Maya six-year-old curious)
- [x] Negative constraints present in prompts (no guru, no superhero, no anime protagonist)
- [x] Runtime matches target (15s proof-of-world clip)
- [x] Aspect ratio matches target (16:9 landscape)
- [x] Files saved with predictable naming
- [x] Final output reproducible from stored prompts and references

---

## Known Caveats

1. **Pichet visual age drift** — Seedance renders Pichet slightly younger/cleaner than intended mature 40s. Acceptable for proof-of-world.
2. **Wall markings** — Some arterial wall patterns read like pseudo-UI rather than organic plaque. Acceptable for proof-of-world.
3. **Maya voice age** — Jessica voice sounds young but not fully six-year-old. May need iteration for final.

---

## Next Steps (Future Episodes)

- Iterate on Pichet visual age with stronger negative prompts
- Explore alternative child voices for Maya
- Add lip-sync pass if dialogue timing requires tighter sync
- Scale to full episode runtime (target: 3-5 minutes)
