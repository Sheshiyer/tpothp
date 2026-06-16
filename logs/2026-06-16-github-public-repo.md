# Publishing Log - GitHub Public Repo

## Repository

- Owner/repo: `Sheshiyer/tpothp`
- URL: `https://github.com/Sheshiyer/tpothp`
- Visibility: public
- Default branch: `main`
- Initial commit: `c6d2c40` (`Initial TPoTHP production assets`)

## Public Seedance Keyframe URL

```text
https://raw.githubusercontent.com/Sheshiyer/tpothp/main/04-generations/images/episode-01-seedance-keyframe-01.png
```

## Verification

- Repo live probe: `gh repo view Sheshiyer/tpothp --json nameWithOwner,visibility,url,defaultBranchRef`
- Repo result: `visibility=PUBLIC`, `defaultBranchRef=main`
- Raw image probe: `curl -L -o /dev/null -w "%{http_code} %{content_type} %{url_effective}\n" <raw-url>`
- Raw image result: `200 image/png`

## Public Surface Policy

The repository intentionally excludes private source docs, `.docx` inputs, copied workflow example media, `.DS_Store`, local credentials, raw source media, generated videos/audio, and `pichet.glb`.
