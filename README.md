# OmniAvatar ULTRA - RunPod Serverless

Full-body AI video generation for BroyhillGOP platform.

## Features
- **14B Model** - Highest quality full-body avatar generation
- **Audio-driven** - Lip-sync + natural body gestures from audio
- **Prompt control** - Customize emotions, poses, backgrounds

## GPU Requirements
- H100 80GB or A100 80GB (AMPERE_80)

## API Usage
```json
{
  "input": {
    "image_base64": "<base64 encoded image>",
    "audio_base64": "<base64 encoded audio>",
    "prompt": "professional speaking pose, confident and friendly",
    "num_steps": 30,
    "guidance_scale": 5.0
  }
}
```

## Response
```json
{
  "output": {
    "video_base64": "<base64 encoded mp4>",
    "quality_score": 95
  }
}
```

## Where this fits in the BroyhillGOP ecosystem map

Canonical numbering per `BROYHILLGOP_ECOSYSTEM_CATALOG.docx` (mirrored in `nexus-platform/reference/ecosystem-audit.md`):

- **E16B — Voice Synthesis** — candidate voice samples + TTS jobs (Chatterbox lives here, repo: `runpod_chatterbox`)
- **E45 — Video Studio** — video output + per-video performance (OmniAvatar extends this ecosystem with full-body avatar generation — **this repo**)

The "Video Stack" labels used in earlier drafts (E47/E48/E49/E50) were a per-repo sketch and do NOT match the canonical 56-ecosystem catalog. E47 is AI Script Generator, E48 is Communication DNA, E49 is Interview System, E50 is unassigned. Always defer to the canonical catalog over per-repo numbering.
