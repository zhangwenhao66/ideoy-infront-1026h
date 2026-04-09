# Contributing to Awesome AI Video Pipelines

Thank you for helping keep this list high-quality and current.

## What Belongs Here

This list is specifically for tools that are useful in **AI-powered video production pipelines** — covering any of these stages:

- Script generation (LLMs, prompt engineering)
- Voice synthesis & TTS (neural TTS, voice cloning)
- Image generation (diffusion models, GAN-based, API services)
- Video synthesis (talking head, text-to-video, lip sync)
- Media assembly & encoding (FFmpeg wrappers, subtitle tools)
- Cloud GPU infrastructure (serverless, spot GPU)
- Stock media APIs (video, image, audio)

**What does NOT belong:**
- Generic ML frameworks not specific to video pipelines (e.g., PyTorch itself)
- Non-AI traditional video editors (Premiere, DaVinci, etc.)
- Tools that are purely for video consumption/streaming, not creation

## Quality Bar

Before submitting a tool, verify:

- **Active**: last commit within 12 months, OR project is archived but still widely used in the community (note this explicitly)
- **Functional**: the tool demonstrably works for the described use case
- **Not a duplicate**: check that it isn't already listed under a different name or category

## How to Add a Tool

1. Fork this repository
2. Add your tool to the relevant category table in `README.md`:
   ```markdown
   | [Tool Name](https://github.com/org/repo) | One-sentence description focused on pipeline use cases. | ![Stars](https://img.shields.io/github/stars/org/repo?style=flat-square) |
   ```
3. If it's a paid/closed-source API (no GitHub repo), omit the Stars column:
   ```markdown
   | [Tool Name](https://example.com) | Description. | — |
   ```
4. Place it in the **most appropriate category**. If genuinely cross-category, pick the primary use case.
5. Open a pull request with the title: `Add: [Tool Name]`

## How to Report Issues

| Issue Type | Label to Use |
|-----------|-------------|
| Broken or redirecting link | `broken-link` |
| Tool no longer maintained and not widely used | `stale` |
| Wrong category placement | `reorganise` |
| Missing high-quality tool | `tool-request` |
| Inaccurate description | `description` |

## Pull Request Checklist

- [ ] Tool is in the correct category
- [ ] Description is one sentence, pipeline-focused
- [ ] GitHub stars badge included (where applicable)
- [ ] Link is correct and opens the right page
- [ ] No duplicate of an existing entry

## Code of Conduct

Be direct and professional. Focus on the technical merit of the tool. No promotional language.

---

Maintained by [InFrontWebs](https://infrontwebs.com)
