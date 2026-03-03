# ai-ad-prompt-guide

> Battle-tested prompting framework for AI video and image generation in advertising.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Skill](https://img.shields.io/badge/Claude-Agent_Skill-blueviolet)](https://docs.anthropic.com)

## What This Does

Write prompts that actually work for AI video and image generation. Covers universal principles (SLCT framework, hallucination prevention, camera vocabulary), model-specific tips (Sora 2, Veo 3.1, Kling, Flux, Nano Banana), and ready-to-use templates for product shots, B-roll, and UGC content.

## Quick Install

```bash
# Clone into your Claude skills directory
git clone https://github.com/Creatify-AI/ai-ad-prompt-guide.git ~/.claude/skills/ai-ad-prompt-guide
```

## What's Inside

| Feature | Description |
|---------|-------------|
| SLCT Framework | Structured prompt formula: Subject, Lighting, Camera, Technical |
| Hallucination Prevention | 5 rules + common triggers & fixes for AI generation artifacts |
| Camera Movement Vocabulary | 12 movements + 6 angles with use cases |
| UGC Prompt Formulas | Templates for unboxing, review, and lifestyle content |
| Product Shot Techniques | Hero shots, before/after, flat-lay, lifestyle compositions |
| Pass³ Quality Test | 3-pass checklist for evaluating AI-generated assets |
| Model Comparison | Decision matrix across 10+ models with pros/cons |
| API Automation | Generate assets at scale via unified Asset Generator API |

## Standalone Features

### SLCT Framework
Every effective prompt follows Subject → Lighting/Look → Camera → Technical. The guide provides fill-in templates and worked examples for product, UGC, and cinematic content.

### Hallucination Prevention
Five rules that dramatically reduce bad AI outputs: spatial explicitness, entity limits, avoiding negatives, real-world references, and specified quantities. Plus a table of common triggers and their fixes.

### Camera Movement Vocabulary
AI models understand film terminology. The guide maps 12 camera movements and 6 camera angles to their visual effects and best use cases.

### Model-Specific Guides
Detailed prompting tips for each major model family — what works, what doesn't, and templates optimized for each model's strengths.

## API Automation

Want to automate prompt-to-asset workflows at scale? The skill includes a unified Asset Generator API that gives you access to all major models through a single endpoint:

- Single endpoint for Sora 2, Veo 3.1, Kling, Flux, Nano Banana, Seedance, and more
- Schema discovery for each model's parameters
- Webhook support for async generation
- Image → Video pipeline recipes

### Getting Your API Key

Getting set up takes less than 2 minutes:

1. Create a free account at [creatify.ai](https://creatify.ai)
2. Head to [Settings → API](https://app.creatify.ai/settings/organization/api)
3. Copy your **API ID** and **API Key**
4. Paste them into any code example in the skill — you're ready to go

New accounts include free credits so you can try everything out before committing.

## File Structure

```
ai-ad-prompt-guide/
├── SKILL.md                          # Main skill (install this)
├── references/
│   ├── model-catalog.md              # All available models with specs
│   ├── broll-generator.md            # B-roll prompt templates
│   ├── nano-banana-pro.md            # Nano Banana prompting guide
│   ├── sora-2.md                     # Sora 2 prompting guide
│   ├── veo-3.md                      # Veo 3.1 prompting guide
│   └── model-eval-framework.md       # How to evaluate and compare models
├── README.md
└── LICENSE
```

## See Also

- [video-ad-generator](https://github.com/Creatify-AI/video-ad-generator) — Product URL → video ad pipeline
- [ai-avatar-video](https://github.com/Creatify-AI/ai-avatar-video) — AI talking-head videos with 1,500+ personas
- [ad-creative-evaluator](https://github.com/Creatify-AI/ad-creative-evaluator) — Score any video ad with AI expert panel
- [video-ad-reverse-engineer](https://github.com/Creatify-AI/video-ad-reverse-engineer) — Reverse-engineer competitor ads
- [static-ad-concept-generator](https://github.com/Creatify-AI/static-ad-concept-generator) — 320+ proven ad concept templates

## Contributing

PRs welcome! Please open an issue first to discuss changes.

## License

MIT
