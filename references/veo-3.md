# Veo 3.1 — Prompting Guide

Veo 3.1 (by Google) delivers the highest cinematic quality with excellent physics coherence.

## Key Strengths
- Best-in-class cinematic quality
- Excellent physics simulation (water, cloth, fire)
- Strong coherence in long sequences
- Multiple input modes (text, image, first-last-frame, reference)
- Good understanding of lighting and atmosphere

## Key Weaknesses
- Can be "too cinematic" for casual/UGC content
- Higher cost than standard-tier competitors
- May add dramatic flair to simple requests

## Available Variants

| Variant | Type | Durations | Notes |
|---------|------|-----------|-------|
| veo3.1 | Text → Video | 4s, 6s, 8s | Highest quality |
| veo3.1/fast | Text → Video | 4s, 6s, 8s | Faster, lower cost |
| veo3.1/image-to-video | Image → Video | — | 64 credits per output |
| veo3.1/fast/image-to-video | Image → Video | — | 32 credits per output |
| veo3.1/first-last-frame-to-video | Keyframe → Video | — | Specify start + end frames |
| veo3.1/fast/first-last-frame-to-video | Keyframe → Video | — | Faster variant |
| veo3.1/reference-to-video | Reference → Video | — | Style-match from reference |

## Prompting Best Practices

### Override the Cinematic Default
Veo 3.1 defaults to a cinematic look. If you want casual/UGC:
```
Shot on iPhone 14, casual quality. NOT cinematic.
Natural indoor lighting, slightly overexposed.
Phone camera, vertical format, slight motion blur.
```

### Use Veo's Physics Strengths
Veo 3.1 handles physical simulations better than most models:
- Pouring liquids
- Fabric draping and flowing
- Smoke and steam
- Reflections on water/glass
- Fire and candle flames

### Lighting Descriptions
Veo responds exceptionally well to detailed lighting:
```
Key light from the upper left at 45 degrees, warm 3200K color temperature.
Soft fill light from the right, 2 stops under the key.
Subtle rim light from behind, separating subject from background.
```

### Duration Strategy
- **4s**: Tight shots, single actions — best value
- **6s**: Standard scenes with one camera movement
- **8s**: Hero content, complex scenes

### Standard vs Fast
- **Standard**: Maximum quality. Use for hero shots, final assets.
- **Fast**: Half the cost. Great for iteration, B-roll, secondary content.

## Ad-Specific Templates

### Luxury Product Shot
```
A [product] floating/resting on [luxurious surface]. Dramatic rim lighting creating a halo effect. Deep black background. Slow rotation revealing product details. Premium commercial aesthetic, jewelry-ad quality lighting. [Duration].
```

### Environmental Establishing Shot
```
Wide establishing shot of [location] at [time]. [Weather/atmosphere]. Cinematic drone-style slow descent. [Color palette description]. Deep depth of field, sharp across the frame. Film grain, anamorphic lens characteristics. [Duration].
```

### First-Last-Frame (Unique to Veo)
Veo 3.1 supports specifying both start and end frames, giving you precise control over the transition:
- Generate or provide two images (first and last frame)
- The model interpolates smoothly between them
- Perfect for before/after reveals, product transformations, dramatic transitions
