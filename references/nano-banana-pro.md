# Nano Banana Pro — Prompting Guide

Nano Banana is optimized for product photography and text rendering in images.

## Key Strengths
- **Best text rendering** of any generation model — logos, labels, packaging text
- **Product fidelity** — maintains product shape, color, and detail accurately
- **Clean compositions** — naturally generates professional product photography
- **Edit mode** — modify existing images while preserving structure

## Prompting Best Practices

### Product Photography
```
[Product name] on a [surface], [setting].
Professional product photography, studio lighting from [direction].
Clean [color] background, [depth of field description].
[Specific detail to emphasize about the product].
```

**Good example:**
```
A 500ml glass bottle of amber face serum with a gold dropper cap on white marble.
Professional product photography, soft key light from upper left.
Clean white background with subtle gradient shadow. Sharp focus on label text.
```

**Bad example:**
```
A serum bottle (too vague — what material? what color? what size?)
```

### Text-Heavy Images
Nano Banana handles text better than other models, but still follow these rules:
- Keep text to 3-5 words maximum per image
- Use common fonts/styles (the model knows "bold sans-serif" better than "Futura Bold")
- Specify text position: "text reading 'SALE' in the upper left"
- For longer text, generate the image without text and add text in post

### Image Editing (nano-banana/edit)
For modifying existing images:
- Provide the source image URL
- Describe ONLY what should change, not the entire scene
- Be specific about the change: "Change the background from white to light blue gradient"
- Preserve language: "Keep the product exactly as-is, only modify the background"

## Common Use Cases

### 1. Product on White Background
```
[Product] centered on pure white background.
E-commerce product photography, even studio lighting, no shadows.
Sharp focus, true-to-life colors.
```

### 2. Lifestyle Product Shot
```
[Product] on a [surface] in a [setting], surrounded by [1-2 complementary props].
Natural [time] lighting, [mood] tones.
Shallow depth of field, focus on product.
Lifestyle editorial photography.
```

### 3. Flat Lay Composition
```
Top-down view of [product] with [complementary items] arranged on [surface].
Even lighting from above, no harsh shadows.
Organized, aesthetically balanced layout.
Social media flat lay style.
```

### 4. Hero Banner Image
```
[Product] prominently featured with [background scene/gradient].
Space for text overlay on [left/right/top] side.
[Brand color] accents, professional marketing photography.
16:9 aspect ratio, clean composition.
```
