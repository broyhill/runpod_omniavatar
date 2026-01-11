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

## Part of BroyhillGOP Video Stack
- E47: Voice Engine (Chatterbox)
- E48: Lip-Sync Engine (Hallo/SadTalker)  
- E49: GPU Orchestrator
- **E50: Full-Body (OmniAvatar) ← THIS**
