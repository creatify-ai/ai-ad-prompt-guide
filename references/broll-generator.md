# B-Roll Generator Prompt Templates

Ready-to-use prompt templates for common B-roll scenarios in video ads.

## Product B-Roll

### Hero Product Shot (Static)
```
A [product] centered on [surface], [environment].
Lighting: [Direction] studio lighting, [mood] tones, subtle reflections on [material].
Camera: Static, shallow depth of field, f/2.8 bokeh background.
Style: High-end product photography, clean composition.
```

### Product Orbit (Motion)
```
Slow 180-degree orbit around a [product] on a [surface].
Lighting: Even studio lighting, soft shadows, [color temperature].
Camera: Smooth arc movement at eye level, medium close-up.
Duration: 5 seconds.
Style: Product showcase, commercial quality.
```

### Product in Environment (Lifestyle)
```
A [product] on a [surface] in a [real-world setting].
[Contextual elements]: [1-2 complementary items].
Lighting: Natural [time of day] light, [mood].
Camera: Slow push-in from medium to close-up.
Duration: 5 seconds.
Style: Lifestyle photography, editorial.
```

## Texture & Detail B-Roll

### Texture Close-Up
```
Extreme close-up of [product surface/texture/material].
Lighting: Raking light from the [direction] to emphasize texture depth.
Camera: Macro lens, static or very slow pan, sharp focus.
Duration: 3-5 seconds.
Style: Sensory, tactile, premium feel.
```

### Pour / Flow / Application
```
[Liquid/cream/powder] being [poured/applied/sprinkled] in slow motion.
Lighting: Backlit to show translucency / Side-lit for dimension.
Camera: Close-up, 60fps slow motion, shallow DOF.
Duration: 5 seconds.
Style: Satisfying, ASMR quality, clean.
```

## Environment / Mood B-Roll

### Establishing Shot
```
Wide shot of [location] at [time of day].
Atmosphere: [Weather/mood], [color palette].
Camera: Slow pan or static wide, deep depth of field.
Duration: 3-5 seconds.
Style: Cinematic, establishing mood.
```

### Abstract / Mood
```
[Abstract visual]: Light through [material], shadows on [surface], [natural element in motion].
Lighting: [Dramatic/ethereal/warm], creating [mood].
Camera: Slow movement, dreamy quality, slight blur.
Duration: 3-5 seconds.
Style: Abstract, atmospheric, brand-mood filler.
```

## People B-Roll (Use with Caution)

### Hands-Only (Avoids Face Hallucination)
```
Close-up of hands [action with product] on a [surface].
Hands: Well-groomed, [skin tone], natural nail color.
Lighting: Natural light from above, soft shadows.
Camera: Top-down or 45-degree angle, medium close-up.
Duration: 5 seconds.
Style: Tutorial, clean, focus on the action.
```

### Crowd / Ambiance (No Faces)
```
[Location] with blurred people in background, shallow DOF.
Focus: [Subject in foreground], people as bokeh background.
Lighting: Natural environment lighting, [time of day].
Camera: Static or slow pan, f/1.8 extreme bokeh.
Duration: 5 seconds.
Style: Lifestyle ambiance, editorial.
```

## Tips for Better B-Roll Prompts

1. **Always specify duration** — models default differently
2. **Include "shallow depth of field"** for product shots — creates professional look
3. **Use "slow"** as a modifier for camera movements — AI models tend to move too fast
4. **Specify aspect ratio** in the API call, not the prompt
5. **For product shots** — generate the still image first (Nano Banana), then animate (Kling/Sora)
6. **Avoid humans** when possible — hands-only or blurred-background approaches work better
