# Sora 2 — Prompting Guide

Sora 2 (by OpenAI) excels at smooth camera movements, consistent lighting, and coherent scene generation.

## Key Strengths
- Smooth, cinematic camera movements
- Consistent lighting throughout the clip
- Good scene coherence and object persistence
- Fast generation at standard tier
- Cost-effective for rapid iteration

## Key Weaknesses
- Fine text rendering (garbled)
- Complex multi-person interactions (face merging)
- Very specific hand/finger poses

## Available Variants

| Variant | Type | Durations | Tier |
|---------|------|-----------|------|
| sora-2/text-to-video | Text → Video | 4s, 8s, 12s | Standard |
| sora-2/text-to-video/pro | Text → Video | 4s, 8s, 12s | Pro (720p/1080p) |
| sora-2/image-to-video | Image → Video | 4s, 8s, 12s | Standard |
| sora-2/image-to-video/pro | Image → Video | 4s, 8s, 12s | Pro (720p/1080p) |

## Prompting Best Practices

### Scene Description
Sora 2 responds well to rich, descriptive language. Paint a picture:

**Good:**
```
A slow dolly forward through a sunlit forest path, morning mist hanging between tall pine trees, golden light filtering through the canopy, creating volumetric light rays. Moss-covered ground, a gentle breeze moving the leaves. Cinematic, film grain, shallow depth of field.
```

**Bad:**
```
A nice forest with sunlight (too vague, no camera direction, no mood)
```

### Camera Movements
Sora 2 understands standard film terminology:
- "Dolly forward/back" — smooth push-in/pull-out
- "Tracking shot left/right" — lateral following
- "Crane up/down" — vertical movement
- "Slow orbit" — circling subject
- "Static shot" — no movement (use for product stills)

Always prefix camera movements with "slow" or "gentle" — Sora defaults to faster-than-expected movement.

### Duration Guide
- **4s**: Single action or static beauty shot — cheapest
- **8s**: Complete scene with one camera movement — best value
- **12s**: Multi-action or complex scene — use for hero content

### Standard vs Pro
- **Standard**: Good for iteration, testing prompts, B-roll at scale
- **Pro**: 720p or 1080p. Use for hero content and final production assets

## Ad-Specific Templates

### Product Establishing Shot
```
A [product] on a [surface] with [background context]. Slow push-in from medium to close-up. [Lighting description]. Shallow depth of field, commercial quality. 4K, photorealistic.
```

### Lifestyle Moment
```
A [person descriptor — age, gender, setting] [performing action with product]. [Location]. [Lighting — natural/warm/golden]. Medium shot, gentle handheld movement. Authentic, lifestyle photography feel.
```

### Abstract/Mood
```
[Abstract visual — light, water, texture, nature]. [Mood — serene, energetic, warm, dramatic]. Slow [camera movement]. Cinematic, [color palette]. Background footage for [brand type].
```
