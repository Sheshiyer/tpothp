# Generation Log - Episode 01 Seedance Run 01

## Request

- Date/time: 2026-06-16
- Backend: RunComfy CLI
- Model attempted first: `bytedance/seedance-v2/pro`
- First attempt result: `API error 404: model not found`
- Current RunComfy API model id: `bytedance/seedance-2.0/pro`
- Input file: `01-prompts/episode-01-arterial-nightmare/seedance-input.json`
- Output directory: `04-generations/video/episode-01`
- Request ID: `6f21c6f0-4a25-49ee-b720-ac33b9323f5d`

## Input Reference

- Public keyframe URL: `https://raw.githubusercontent.com/Sheshiyer/tpothp/main/04-generations/images/episode-01-seedance-keyframe-01.png`
- Local keyframe: `04-generations/images/episode-01-seedance-keyframe-01.png`
- Prompt chars in payload: `2173`
- Aspect ratio: `16:9`
- Duration: `15`
- Resolution: `720p`
- Generate audio: `true`

## Output

- RunComfy result URL: `https://playgrounds-storage-public.runcomfy.net/eNqzME9KNTUxStM1MjRP0jVJtTTVtTRNS9VNsjQxSzNPTko0Sk4DAK4KCes%3D/eNozMjAy0zUw0zU0CzE0szI2tDIy1DMzNDOyNNA2MLAyMAAAay4Gcw%3D%3D/output/e5ef985b222de7858d80763a7873b4a3_1781627474_siay9jex.mp4`
- Local file: `04-generations/video/episode-01/e5ef985b222de7858d80763a7873b4a3_1781627474_siay9jex.mp4`
- File size: `7146768` bytes
- SHA-256: `bbbda4f8f77107f12597f56f07c064435e5326fdab07cfeeb5af007e2e0856e3`
- Duration: `15.092971` seconds
- Video: `h264`, `1280x720`, `24 fps`
- Audio: `aac`, stereo, `44100 Hz`

## Preview Frames

- `04-generations/video/episode-01/preview/frame-01s.jpg`
- `04-generations/video/episode-01/preview/frame-05s.jpg`
- `04-generations/video/episode-01/preview/frame-10s.jpg`
- `04-generations/video/episode-01/preview/frame-14s.jpg`

## Visual Notes

- Works: arterial tunnel, golden flow path, dream plaque, Maya with comfort blanket, Pichet kneeling, and final plaque-clearing arc all survived the generation.
- Works: video output has synchronized audio track and correct 15-second runtime.
- Caveat: Pichet drifts younger and cleaner than the strongest still reference.
- Caveat: some wall marks read as faint pseudo-UI, though there are no subtitles or explicit foreground text.
- Caveat: the scene is more polished sci-fi tunnel than organic anatomical-city texture.

## Lesson

RunComfy's page path still uses `/models/bytedance/seedance-v2/pro`, but the CLI/API model id exposed on the page is `bytedance/seedance-2.0/pro`. Use the latter for `runcomfy run`.
