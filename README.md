<div align="center">

# Awesome AI Video Pipelines

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![Last Updated](https://img.shields.io/github/last-commit/InFrontWebs/Awesome-AI-Video-Pipelines?style=flat-square&label=Last%20Updated&color=green)
![Stars](https://img.shields.io/github/stars/InFrontWebs/Awesome-AI-Video-Pipelines?style=flat-square&color=orange)
![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/License-CC0_1.0-lightgrey?style=flat-square)

**A curated list of tools, models, APIs, and infrastructure for building end-to-end AI-powered video production pipelines.**

Maintained by [InFrontWebs](https://infrontwebs.com) — AI automation & cloud infrastructure engineering.

</div>

---

## What Is AI Video Pipeline Engineering?

AI video pipeline engineering is the discipline of chaining together generative AI systems — language models, neural TTS, image synthesis, video synthesis, and media assembly tools — into automated, production-grade workflows that can produce video content at scale without human intervention at each stage.

A typical pipeline: **LLM script** → **Neural TTS narration** → **AI image/video generation** → **Talking-head synthesis** → **FFmpeg assembly** → **Auto-upload**.

This list curates the best tools, models, and APIs at each layer of the stack — from open-source models you can run locally to cloud GPU platforms and media APIs.

---

## Table of Contents

- [Voice & TTS](#voice--tts)
- [Video Generation & Talking Head](#video-generation--talking-head)
- [Image Generation](#image-generation)
- [LLM & Orchestration](#llm--orchestration)
- [Stock & Media APIs](#stock--media-apis)
- [Assembly & Encoding](#assembly--encoding)
- [Cloud GPU Platforms](#cloud-gpu-platforms)
- [Contributing](#contributing)
- [License](#license)

---

## Voice & TTS

Neural text-to-speech engines for narration, voice cloning, and multi-speaker synthesis.

| Tool | Description | Stars |
|------|-------------|-------|
| [Chatterbox TTS](https://github.com/resemble-ai/chatterbox) | State-of-the-art open-source TTS by Resemble AI with zero-shot voice cloning. Excellent for consistent narrator voices across long-form content. | ![Stars](https://img.shields.io/github/stars/resemble-ai/chatterbox?style=flat-square) |
| [Kokoro TTS](https://github.com/hexgrad/kokoro) | Lightweight, fast TTS model with high naturalness. Small model footprint — runs on CPU efficiently. Great for local/offline pipelines. | ![Stars](https://img.shields.io/github/stars/hexgrad/kokoro?style=flat-square) |
| [Fish Audio](https://fish.audio) | Cloud TTS API with voice cloning, 100+ voices, multi-language. API-first design ideal for pipeline integration. | — |
| [Coqui TTS](https://github.com/coqui-ai/TTS) | Mature open-source TTS toolkit with XTTS, VITS, and YourTTS models. Voice cloning and multi-speaker support. Archived but widely used. | ![Stars](https://img.shields.io/github/stars/coqui-ai/TTS?style=flat-square) |
| [Bark](https://github.com/suno-ai/bark) | Transformer-based audio model by Suno. Supports speech, music, sound effects, and non-verbal sounds from text prompts. | ![Stars](https://img.shields.io/github/stars/suno-ai/bark?style=flat-square) |
| [StyleTTS2](https://github.com/yl4579/StyleTTS2) | Human-level TTS with style diffusion and adversarial training. Achieves near-human naturalness on LJSpeech benchmarks. | ![Stars](https://img.shields.io/github/stars/yl4579/StyleTTS2?style=flat-square) |
| [F5-TTS](https://github.com/SWivid/F5-TTS) | Flow-matching based TTS with exceptional voice cloning quality. Fast inference with full naturalness. | ![Stars](https://img.shields.io/github/stars/SWivid/F5-TTS?style=flat-square) |

---

## Video Generation & Talking Head

- [Ideoy](https://ideoy.ai) - Freemium AI meme & image-to-video generator: turn images/memes into short viral videos.
Models for generating talking-head video, lip-synced avatars, and full scene video synthesis.

| Tool | Description | Stars |
|------|-------------|-------|
| [MuseTalk](https://github.com/TMElyralab/MuseTalk) | Real-time talking face generation via latent diffusion. Syncs mouth movement to audio with high visual quality. Used in production video pipelines. | ![Stars](https://img.shields.io/github/stars/TMElyralab/MuseTalk?style=flat-square) |
| [Hallo2](https://github.com/fudan-generative-vision/hallo2) | Long-duration talking avatar generation with consistent identity and audio-driven animation. Strong temporal coherence for long-form content. | ![Stars](https://img.shields.io/github/stars/fudan-generative-vision/hallo2?style=flat-square) |
| [SadTalker](https://github.com/OpenTalker/SadTalker) | Learning Realistic 3D Motion Coefficients for Stylized Audio-Driven Single Image Talking Face Animation. Widely used, battle-tested. | ![Stars](https://img.shields.io/github/stars/OpenTalker/SadTalker?style=flat-square) |
| [Wan2.1](https://github.com/Wan-Video/Wan2.1) | State-of-the-art open-source video generation model by Alibaba. Supports text-to-video and image-to-video at high quality. | ![Stars](https://img.shields.io/github/stars/Wan-Video/Wan2.1?style=flat-square) |
| [CogVideoX](https://github.com/THUDM/CogVideo) | Open-source video generation model from Tsinghua. Strong semantic understanding and motion quality for cinematic output. | ![Stars](https://img.shields.io/github/stars/THUDM/CogVideo?style=flat-square) |
| [Wav2Lip](https://github.com/Rudrabha/Wav2Lip) | Accurately lip-syncs videos to any speech audio. Fast inference, production-proven, works with any face video. | ![Stars](https://img.shields.io/github/stars/Rudrabha/Wav2Lip?style=flat-square) |
| [LatentSync](https://github.com/bytedance/LatentSync) | ByteDance's audio-conditioned latent diffusion model for talking head generation with high-fidelity lip sync. | ![Stars](https://img.shields.io/github/stars/bytedance/LatentSync?style=flat-square) |

---

## Image Generation

Models and tools for generating cinematic stills, scene illustrations, and visual assets for video.

| Tool | Description | Stars |
|------|-------------|-------|
| [Flux](https://github.com/black-forest-labs/flux) | State-of-the-art text-to-image model by Black Forest Labs. Excellent prompt adherence, photorealism, and cinematic quality. Deployable on RunPod. | ![Stars](https://img.shields.io/github/stars/black-forest-labs/flux?style=flat-square) |
| [Stable Diffusion XL](https://github.com/Stability-AI/generative-models) | SDXL and SD3 from Stability AI. Robust ecosystem, extensive ControlNet and LoRA support. | ![Stars](https://img.shields.io/github/stars/Stability-AI/generative-models?style=flat-square) |
| [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | Node-based UI and API for building complex image generation workflows. Supports Flux, SDXL, ControlNet, and hundreds of custom nodes. | ![Stars](https://img.shields.io/github/stars/comfyanonymous/ComfyUI?style=flat-square) |
| [Midjourney API](https://docs.midjourney.com) | Leading commercial image generation via API. Exceptional aesthetic quality — useful for hero images and thumbnails. | — |
| [DALL-E 3](https://platform.openai.com/docs/guides/images) | OpenAI's image generation API. Strong at following complex text descriptions. Simple API integration. | — |
| [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) | Practical image/video upscaling for restoring details. Upscale AI-generated images to 4K for maximum Ken Burns headroom. | ![Stars](https://img.shields.io/github/stars/xinntao/Real-ESRGAN?style=flat-square) |

---

## LLM & Orchestration

Language models and orchestration tools for script generation, prompt building, and pipeline logic.

| Tool | Description | Stars |
|------|-------------|-------|
| [Ollama](https://github.com/ollama/ollama) | Run LLMs locally (Llama 3, Mistral, DeepSeek, Gemma) with a simple API. Essential for local/offline pipeline scripting. | ![Stars](https://img.shields.io/github/stars/ollama/ollama?style=flat-square) |
| [LM Studio](https://lmstudio.ai) | Desktop app for discovering, downloading, and running local LLMs. Great for model evaluation before pipeline integration. | — |
| [vLLM](https://github.com/vllm-project/vllm) | High-throughput and memory-efficient LLM inference engine. Best-in-class for serving LLMs in production at scale. | ![Stars](https://img.shields.io/github/stars/vllm-project/vllm?style=flat-square) |
| [LangChain](https://github.com/langchain-ai/langchain) | Framework for building LLM-powered applications with chains, agents, and retrieval. Broad ecosystem for pipeline orchestration. | ![Stars](https://img.shields.io/github/stars/langchain-ai/langchain?style=flat-square) |
| [LlamaIndex](https://github.com/run-llama/llama_index) | Data framework for LLM applications — RAG, knowledge bases, structured data querying. | ![Stars](https://img.shields.io/github/stars/run-llama/llama_index?style=flat-square) |
| [DeepSeek](https://github.com/deepseek-ai/DeepSeek-V3) | High-capability open-weight LLM with strong reasoning and coding ability. Cost-effective via API or self-hosted. | ![Stars](https://img.shields.io/github/stars/deepseek-ai/DeepSeek-V3?style=flat-square) |
| [DSPy](https://github.com/stanfordnlp/dspy) | Stanford's framework for programming with language models — optimises prompts and pipelines systematically. | ![Stars](https://img.shields.io/github/stars/stanfordnlp/dspy?style=flat-square) |

---

## Stock & Media APIs

APIs for sourcing stock video, images, and audio to supplement AI-generated assets.

| Tool | Description |
|------|-------------|
| [Pexels API](https://www.pexels.com/api/) | Free stock photos and videos API. Generous rate limits, high-quality assets, commercial use allowed. Excellent FFmpeg pipeline fallback. |
| [Pixabay API](https://pixabay.com/api/docs/) | Free stock images, vectors, and videos. No attribution required. Good alternative to Pexels with large library. |
| [Unsplash API](https://unsplash.com/developers) | High-quality free photos API. 50 requests/hour free tier. Best for landscape and architecture shots. |
| [Freesound API](https://freesound.org/docs/api/) | Collaborative sound database API. Ambient sounds, SFX, and music for video soundscapes. |
| [YouTube Data API v3](https://developers.google.com/youtube/v3) | Programmatic upload, scheduling, metadata management, and analytics for YouTube. Core to automated publishing pipelines. |

---

## Assembly & Encoding

Tools for compositing, encoding, and processing video and audio assets.

| Tool | Description | Stars |
|------|-------------|-------|
| [FFmpeg](https://ffmpeg.org) | The definitive video processing toolkit. Used for cutting, compositing, encoding, streaming, and format conversion in virtually every production pipeline. | — |
| [MoviePy](https://github.com/Zulko/moviepy) | Python library for video editing built on FFmpeg. Programmatic cuts, effects, subtitles, and transitions. Good for rapid scripting. | ![Stars](https://img.shields.io/github/stars/Zulko/moviepy?style=flat-square) |
| [Whisper](https://github.com/openai/whisper) | OpenAI's speech recognition model. Use for automatic caption generation and forced alignment for subtitle tracks. | ![Stars](https://img.shields.io/github/stars/openai/whisper?style=flat-square) |
| [faster-whisper](https://github.com/SYSTRAN/faster-whisper) | CTranslate2-powered reimplementation of Whisper. 4× faster with lower memory — production-grade caption pipeline tool. | ![Stars](https://img.shields.io/github/stars/SYSTRAN/faster-whisper?style=flat-square) |
| [PyDub](https://github.com/jiaaro/pydub) | Simple audio manipulation in Python. Chunk splitting, silence detection, normalisation — useful for TTS post-processing. | ![Stars](https://img.shields.io/github/stars/jiaaro/pydub?style=flat-square) |

---

## Cloud GPU Platforms

Infrastructure for running GPU-accelerated AI inference at scale without managing physical hardware.

| Platform | Description |
|----------|-------------|
| [RunPod](https://runpod.io) | Serverless and on-demand GPU cloud. Best serverless pricing for Flux, Stable Diffusion, and custom model endpoints. Supports Docker containers with custom model weights. |
| [Vast.ai](https://vast.ai) | Peer-to-peer GPU marketplace. Lowest per-hour rates for spot GPU rentals. Good for batch image generation jobs. |
| [Lambda Labs](https://lambdalabs.com) | On-demand and reserved GPU cloud from ML-focused provider. H100s and A100s available. Good uptime SLAs. |
| [Modal](https://modal.com) | Serverless Python cloud for ML workloads. Deploy any Python function to GPU in minutes. Excellent developer experience. |
| [Replicate](https://replicate.com) | Run open-source ML models via API. Pre-deployed Flux, SDXL, Whisper, and many others. No GPU management. |

---

## Contributing

Contributions are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

**Adding a tool:**
- Verify the project is actively maintained (last commit within 12 months, or note if archived but widely used)
- Include a one-sentence description focused on pipeline use cases
- Add the GitHub stars badge where applicable
- Place under the most relevant category

**Opening an issue:**
- Broken link → label `broken-link`
- Missing tool → label `tool-request`
- Wrong category → label `reorganise`

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

This list is released under CC0 — no rights reserved. Use it freely.

Maintained by [InFrontWebs](https://infrontwebs.com) · Bangladesh
