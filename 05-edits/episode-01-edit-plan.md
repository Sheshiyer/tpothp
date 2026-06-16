# Episode 01 - Edit Plan

## Source Assets

### Video
- File: `04-generations/video/episode-01/e5ef985b222de7858d80763a7873b4a3_1781627474_siay9jex.mp4`
- Duration: 15.09s
- Resolution: 1280x720
- Codec: H.264, 24fps
- Built-in audio: AAC (to be replaced)

### Audio - Score
- File: `04-generations/audio/episode-01/episode-01-score-01.mp3`
- Duration: 15.05s
- Volume: -6dB (background level)

### Audio - Pichet Voice
- File: `04-generations/audio/episode-01/episode-01-pichet-line-01.mp3`
- Duration: 5.80s
- Line: "Nightmares are not attacks, Maya. Sometimes they are pipes carrying a truth that has nowhere else to go."
- Start time: 2.0s (enters after establishing shot)
- Volume: 0dB (foreground)

### Audio - Maya Voice  
- File: `04-generations/audio/episode-01/episode-01-maya-line-01.mp3`
- Duration: 2.88s
- Line: "If it was scary... why is it shining?"
- Start time: 10.5s (responds near end as plaque clears)
- Volume: 0dB (foreground)

## Timeline

```
0s                    5s                    10s                   15s
|---------------------|---------------------|---------------------|
[VIDEO: Seedance clip - arterial tunnel, Pichet + Maya, plaque clearing]
[SCORE: Full 15s ambient bed at -6dB----------------------------------------]
         [PICHET: 2.0s-7.8s "Nightmares are not attacks..."]
                                      [MAYA: 10.5s-13.4s "If it was scary..."]
```

## FFmpeg Mix Command

```bash
ffmpeg -y \
  -i "04-generations/video/episode-01/e5ef985b222de7858d80763a7873b4a3_1781627474_siay9jex.mp4" \
  -i "04-generations/audio/episode-01/episode-01-score-01.mp3" \
  -i "04-generations/audio/episode-01/episode-01-pichet-line-01.mp3" \
  -i "04-generations/audio/episode-01/episode-01-maya-line-01.mp3" \
  -filter_complex "
    [1:a]volume=-6dB[score];
    [2:a]adelay=2000|2000[pichet];
    [3:a]adelay=10500|10500[maya];
    [score][pichet][maya]amix=inputs=3:duration=longest:normalize=0[aout]
  " \
  -map 0:v -map "[aout]" \
  -c:v copy \
  -c:a aac -b:a 192k \
  -shortest \
  "07-deliverables/episode-01-the-dream-in-the-artery-v1.mp4"
```

## Output

- File: `07-deliverables/episode-01-the-dream-in-the-artery-v1.mp4`
- Format: MP4 (H.264 video, AAC audio)
- Target: Proof-of-world deliverable for internal review

## Notes

- Pichet's line starts at 2s to allow the establishing arterial tunnel shot.
- Maya's line starts at 10.5s, timed to coincide with the plaque-clearing arc.
- Score runs full length as ambient bed at -6dB.
- Video codec is copied (no re-encode) to preserve quality.
- Audio mixed to AAC 192kbps stereo.
