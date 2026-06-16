# Generation Log - Episode 01 Audio Assets

## Overview

- Date/time: 2026-06-16
- Phase: 4 - Audio / Voice / Music
- Backends: ElevenLabs Music (RunComfy), ElevenLabs TTS (Composio)

## Music Generation

### Score

- Backend: RunComfy CLI
- Model: `elevenlabs/elevenlabs/music-generation`
- Request ID: `f4bc9b6a-dda7-4340-afd0-c0cdb8989f8b`
- Input file: `01-prompts/episode-01-arterial-nightmare/elevenlabs-music-input.json`
- Output file: `04-generations/audio/episode-01/episode-01-score-01.mp3`
- Duration: `15.0465` seconds
- Format: MP3, 44.1kHz stereo, 128kbps
- File size: `240789` bytes
- SHA-256: `ab9c68610dd1be0ea8ba4e26b7227feaf983c18f4a0da1c5c53d30d68c2fd697`

### Score Prompt

```
Original symbolic anime short score for a tender mystical repair scene inside a living arterial city. Soft low heartbeat percussion at 60 BPM, warm glass harmonics, distant lullaby motif, subtle tanpura-like drone, gentle strings entering after 0:09, aged-gold emotional glow. Begins eerie and constricted, then opens into calm circulation. Cinematic, healing, intimate, quietly cosmic. No bombast, no trailer drums, no vocals. Clean fade ending.
```

## Voice Generation

### Pichet Voice Line

- Backend: Composio ElevenLabs TTS
- Tool: `ELEVENLABS_TEXT_TO_SPEECH`
- Voice: Chris - Charming, Down-to-Earth (voice_id: `iP95p4xoKVk53GoZ742B`)
- Model: `eleven_multilingual_v2`
- Text: "Nightmares are not attacks, Maya. Sometimes they are pipes carrying a truth that has nowhere else to go."
- Voice settings: stability 0.45, similarity 0.85, style 0.25, speaker boost ON
- Output file: `04-generations/audio/episode-01/episode-01-pichet-line-01.mp3`
- Duration: `5.804989` seconds
- File size: `94084` bytes
- SHA-256: `ef912b5ee92ffb5f8d91c568ebcd3fd653e433086ecfea31a6b5f113fab78a98`

### Maya Voice Line

- Backend: Composio ElevenLabs TTS
- Tool: `ELEVENLABS_TEXT_TO_SPEECH`
- Voice: Jessica - Playful, Bright, Warm (voice_id: `cgSgspJ2msm6clMCkdW9`)
- Model: `eleven_multilingual_v2`
- Text: "If it was scary... why is it shining?"
- Voice settings: stability 0.55, similarity 0.75, style 0.15, speaker boost ON
- Output file: `04-generations/audio/episode-01/episode-01-maya-line-01.mp3`
- Duration: `2.879274` seconds
- File size: `47273` bytes
- SHA-256: `677856015b01abdad0bba8c7526160a70cf55b772d460a202655057c75290986`

## Voice Selection Rationale

- **Pichet**: Chris (iP95p4xoKVk53GoZ742B) selected for "charming, down-to-earth" quality matching the prompt's "warm, grounded, practical, slightly tired but kind" tradesman who has seen mystical things.
- **Maya**: Jessica (cgSgspJ2msm6clMCkdW9) selected for "playful, bright, warm" quality matching a six-year-old child's frightened-to-curious arc.

## Notes

- Score matches the 15-second target runtime for the Seedance video.
- Voice lines are shorter than the video runtime, allowing for atmospheric spacing and score presence.
- Combined voice runtime (~8.7s) plus pauses and score should layer well over 15s video.
- Maya's voice sounds young but not childish enough for a six-year-old; acceptable for proof-of-world but may need iteration with a different voice for final delivery.
