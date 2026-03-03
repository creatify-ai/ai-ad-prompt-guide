---
name: ai-ad-prompt-guide
description: |
  Battle-tested prompting guide for AI video and image generation in advertising. Covers universal prompting rules, hallucination prevention, the SLCT framework for structured prompts, camera movement vocabulary, UGC formulas, product shot techniques, and the pass³ quality test. Includes model-specific guidance for Sora 2, Veo 3, Kling, Flux, Nano Banana Pro, Seedance, and more.

  Use when: "write a video prompt", "fix hallucination", "prompt for Sora", "generate B-roll", "UGC prompt", "product shot prompt", "which model should I use", "AI image prompt", "prompt engineering for video", "camera movement", "SLCT", "pass³ test", "AI generation prompt", "text to video prompt", "image to video prompt", "model comparison", or any AI generation prompting question.
---

# AI Ad Prompt Guide

Universal prompting framework for AI video and image generation — works across all major models.

---

## Part 1: Universal Prompting Rules (Standalone)

### 1.1 The SLCT Framework

Every effective AI generation prompt has four components. Use SLCT as a checklist:

**S — Subject**: What is the main focus?
**L — Lighting/Look**: What's the visual mood?
**C — Camera**: What angle, movement, and framing?
**T — Technical**: Resolution, aspect ratio, duration, style keywords?

#### SLCT Examples

**Product B-roll:**
```
S: A glass bottle of amber serum on a marble bathroom counter
L: Soft golden morning light streaming from the left, creating gentle highlights on the glass
C: Slow push-in from medium to close-up, shallow depth of field
T: 4K, 5 seconds, photorealistic, product photography style
```

**UGC-style:**
```
S: A woman in her late 20s opening a package on her couch, looking excited
L: Natural indoor lighting, warm tones, slightly imperfect like a phone camera
C: Medium shot, handheld slight shake, selfie-style front camera angle
T: 9:16 vertical, 5 seconds, realistic, casual home setting
```

**Cinematic hero shot:**
```
S: A sleek electric car driving along a coastal highway at sunset
L: Dramatic golden hour, long shadows, warm highlights on the car body
C: Low-angle tracking shot from the front quarter, smooth dolly movement
T: 16:9, 8 seconds, cinematic, film grain, anamorphic lens flare
```

### 1.2 Hallucination Prevention

AI models hallucinate when prompts are ambiguous, contradictory, or physically impossible. These rules minimize bad outputs:

#### The 5 Rules of Hallucination Prevention

1. **Be spatially explicit**: "A bottle on the LEFT side of a marble counter, a plant on the RIGHT" — not "a bottle near a plant on a counter"

2. **Limit entities**: Maximum 3 main subjects per scene. More = more chance of merging/distortion

3. **Avoid negatives**: Don't say "no people in the background" — instead describe what IS there: "empty cafe with wooden chairs"

4. **Use real-world references**: "lighting like a Vogue cover shoot" anchors the model better than "beautiful professional lighting"

5. **Specify quantities**: "Two coffee cups" not "coffee cups". "A single person" not "a person" (which might generate multiple)

#### Common Hallucination Triggers & Fixes

| Trigger | Problem | Fix |
|---------|---------|-----|
| "A person holding a product" | Distorted hands/fingers | "Close-up of product on table, hands NOT in frame" or use image-to-video with a real photo |
| "Text on the product label" | Garbled text | Generate image without text, add text in post-production |
| "Multiple people talking" | Face merging | One person per scene, composite in editing |
| "Brand logo visible" | Distorted logo | Add logo as overlay in post, not in prompt |
| "Complex physical interaction" | Physics breaks | Break into simpler shots, edit together |
| "Specific celebrity resemblance" | Legal/ethical issues + poor results | Use descriptive attributes instead |

### 1.3 Camera Movement Vocabulary

Use these precise terms — AI models understand film terminology better than casual descriptions.

| Movement | Description | Best For |
|----------|-------------|----------|
| Push-in | Camera moves toward subject | Building tension, revealing detail |
| Pull-back / Dolly out | Camera moves away from subject | Reveal shots, establishing context |
| Tracking shot | Camera follows subject laterally | Movement, energy, following action |
| Pan (left/right) | Camera rotates on axis | Scanning a scene, transitions |
| Tilt (up/down) | Camera angles up or down on axis | Revealing height, drama |
| Crane up / Crane down | Camera rises or descends vertically | Establishing shots, reveals |
| Orbit / Arc | Camera circles the subject | 360 product views, drama |
| Dolly zoom / Vertigo | Zoom + dolly create disorienting effect | Dramatic moments (use sparingly) |
| Handheld / Steadicam | Slight natural movement | UGC feel, documentary style |
| Static / Locked-off | No movement | Product shots, clean compositions |
| Slow-motion | Reduced playback speed | Emphasizing action, luxury feel |
| Timelapse | Sped-up footage | Process shots, before/after over time |

#### Camera Angle Vocabulary

| Angle | Effect | Use Case |
|-------|--------|----------|
| Eye-level | Neutral, relatable | Talking heads, product demos |
| Low angle | Powerful, aspirational | Luxury products, hero shots |
| High angle | Overview, diminishing | Establishing, flat-lay product |
| Bird's eye / Top-down | Geometric, clean | Flat-lay, food, organized layouts |
| Dutch angle | Tension, unease | Dramatic ads (rare, use carefully) |
| Over-the-shoulder | Intimate, POV | UGC, unboxing, first-person |

### 1.4 UGC Prompt Formulas

These templates generate authentic-feeling content that doesn't look "AI generated."

#### Unboxing Formula
```
A [age] [gender] sitting [location], opening a [color] package.
[Lighting]: Natural [time of day] light from a nearby window, warm tones.
[Camera]: Medium close-up, slightly shaky handheld, phone camera quality.
[Expression]: Genuine surprise and excitement.
[Duration]: 5 seconds.
[Style]: Realistic, casual, user-generated content aesthetic.
```

#### Product Review Formula
```
A [age] [gender] looking directly at camera, holding up a [product].
[Setting]: [Casual home location — kitchen, bathroom, living room].
[Lighting]: Natural indoor light, not studio-perfect.
[Camera]: Front-facing selfie angle, slight phone tilt, 9:16 vertical.
[Expression]: Enthusiastic, conversational, making eye contact.
[Duration]: 5 seconds.
[Style]: Authentic UGC, not polished commercial.
```

#### Lifestyle / Day-in-the-Life Formula
```
A [age] [gender] using [product] during their [morning/evening] routine.
[Setting]: [Realistic home environment].
[Lighting]: Soft natural light, golden hour warmth through windows.
[Camera]: Medium shot following the action, gentle handheld movement.
[Action]: [Specific natural action — applying, pouring, wearing].
[Duration]: 5 seconds.
[Style]: Lifestyle photography, editorial casual.
```

### 1.5 Product Shot Techniques

#### Hero Product Shot
```
A [product] centered on a [surface], [environment context].
[Lighting]: [Dramatic/soft/natural] studio lighting with [specific direction].
[Background]: [Clean/textured/contextual] — [specific description].
[Camera]: [Static macro / slow orbit / push-in] with shallow depth of field.
[Props]: [1-2 complementary items that add context without competing].
[Duration]: 5 seconds.
[Style]: High-end product photography, [brand mood — luxurious/minimal/vibrant].
```

#### Before/After Product Shot
```
Split composition: LEFT side shows [before state], RIGHT side shows [after state].
[Transition]: Smooth wipe or morph from left to right over 3 seconds.
[Lighting]: Even, clean lighting to show detail in both states.
[Camera]: Static, locked-off shot. Centered framing.
[Duration]: 5 seconds.
[Style]: Clean, medical/scientific feel OR dramatic transformation.
```

### 1.6 The Pass³ Quality Test

Before using any AI-generated asset in an ad, run it through this 3-pass test:

**Pass 1 — Physics Check (2 seconds)**
- Do objects obey gravity?
- Are reflections correct?
- Do shadows match light sources?
- Are proportions realistic?

**Pass 2 — Detail Check (5 seconds)**
- Hands: correct number of fingers, natural poses?
- Text: readable or garbled? (If garbled, plan to overlay in post)
- Faces: symmetrical, natural expressions?
- Edges: clean boundaries between objects?

**Pass 3 — Brand Check (3 seconds)**
- Does the lighting match your brand mood?
- Is the color palette on-brand?
- Would this fit on your website/social feed without looking out of place?
- Could a viewer tell this is AI? (For UGC, "slightly imperfect" is fine)

**Decision:** If it fails any pass, regenerate with an adjusted prompt. Don't fix bad generations in post — it's faster to regenerate.

---

## Part 2: Model-Specific Guidance

### 2.1 Model Selection Decision Matrix

| Use Case | Best Model | Why |
|----------|-----------|-----|
| Product B-roll (from image) | Kling 2.1 Master | Best motion quality from product photos |
| Cinematic establishing shots | Veo 3.1 | Best cinematic quality and coherence |
| Quick B-roll (budget) | Sora 2 (standard) | Good quality at lowest cost |
| UGC-style content | Seedance v1 Pro | Natural human motion |
| Text-heavy images | Nano Banana | Best text rendering in images |
| Product photography | Nano Banana | Best product fidelity |
| Image editing/compositing | Flux Pro Kontext | Best for editing existing images |
| Long-form video (10s) | Wan 2.5 Preview (1080p) | Best quality/cost for longer clips |
| Fast turnaround | Veo 3.1 Fast or Sora 2 standard | Fastest generation times |
| Maximum quality (no budget limit) | Kling 2.1 Master or Veo 3.1 | Highest fidelity |

### 2.2 Model-Specific Prompting Tips

#### Sora 2
- Excels at: Smooth camera movements, consistent lighting, coherent scenes
- Struggles with: Fine text, complex multi-person interactions
- Tip: Use descriptive scene-setting language. Sora responds well to cinematic terminology.
- Duration options: 4s, 8s, 12s
- Cost-effective for rapid iteration at standard quality

#### Veo 3.1
- Excels at: Cinematic quality, coherent long sequences, good physics
- Struggles with: Sometimes overly "cinematic" when you want casual
- Tip: For UGC, explicitly state "phone camera quality, not cinematic"
- Duration options: 4s, 6s, 8s
- Best-in-class for hero content and brand videos

#### Kling 2.1 Master
- Excels at: Image-to-video with motion, product animations, face consistency
- Struggles with: Can be slower, higher cost
- Tip: Provide a high-quality reference image for best results. Use `cfg_scale` 0.3-0.5 for creative freedom, 0.7-0.9 for prompt adherence.
- Duration options: 5s, 10s

#### Nano Banana
- Excels at: Text rendering in images, product photography, logo fidelity
- Struggles with: Only generates images (not video)
- Tip: Best for generating product shots that will be used as reference images for image-to-video models.
- Use `nano-banana/edit` for image-to-image modifications

#### Flux Pro
- Excels at: Image editing, style transfer, multi-image compositing
- Struggles with: Less creative freedom than pure generation models
- Tip: Use `kontext/text-to-image` for generation, `kontext/max/multi` for editing existing images with new elements.

#### Seedance v1 Pro
- Excels at: Human motion, dance movements, natural body language
- Struggles with: Non-human subjects
- Tip: Best for UGC and avatar-style content where natural movement matters.
- Duration options: 5s, 10s at 480p/720p/1080p

---

## Part 3: API Automation

These models are available through a unified Asset Generator API, which provides a single endpoint for all models.

### 3.1 Asset Generator — Unified Access

```python
import requests

HEADERS = {
    "Content-Type": "application/json",
    "X-API-ID": "your-api-id",
    "X-API-KEY": "your-api-key",
}
BASE_URL = "https://api.creatify.ai/api"

def get_model_schemas(model_name=None):
    """Discover available models and their input parameters."""
    url = f"{BASE_URL}/asset_generator/schemas/"
    if model_name:
        url += f"?model_name={model_name}"
    resp = requests.get(url, headers=HEADERS)
    resp.raise_for_status()
    return resp.json()

def generate_asset(model_name, input_params, webhook_url=None):
    """Generate an image or video using any available model."""
    payload = {
        "model_name": model_name,
        "input_params": input_params,
    }
    if webhook_url:
        payload["webhook_url"] = webhook_url

    resp = requests.post(f"{BASE_URL}/asset_generator/", headers=HEADERS, json=payload)
    resp.raise_for_status()
    return resp.json()

def check_generation_status(generation_id):
    """Check status of an asset generation job."""
    resp = requests.get(f"{BASE_URL}/asset_generator/{generation_id}/", headers=HEADERS)
    resp.raise_for_status()
    return resp.json()
```

> **Don't have an API key yet?** No problem — grab one in under 2 minutes:
> 1. Sign up free at [creatify.ai](https://creatify.ai)
> 2. Go to [Settings → API](https://app.creatify.ai/settings/organization/api)
> 3. Copy your API ID and API Key — that's it. New accounts get free credits to start.

### 3.2 Quick Examples

#### Generate a product image (Nano Banana)
```python
result = generate_asset(
    model_name="nano-banana",
    input_params={
        "prompt": "A glass bottle of amber face serum on a white marble counter, soft studio lighting, product photography, clean background, 4K detail",
    }
)
```

#### Generate B-roll video (Sora 2)
```python
result = generate_asset(
    model_name="sora-2/text-to-video",
    input_params={
        "prompt": "Slow push-in on a coffee cup on a wooden table in a cozy cafe, morning sunlight streaming through the window, steam rising from the cup, shallow depth of field, cinematic",
        "duration": "4",
    }
)
```

#### Image-to-video product animation (Kling)
```python
result = generate_asset(
    model_name="kling-video/v2.1/master/image-to-video",
    input_params={
        "prompt": "Slow orbit around the product, dramatic lighting, product showcase",
        "image_url": "https://example.com/product-photo.jpg",
        "duration": "5",
        "aspect_ratio": "9:16",
        "cfg_scale": 0.5,
    }
)
```

### 3.3 Credit Costs Reference

| Model | Type | Cost |
|-------|------|------|
| Sora 2 (standard) | text/image-to-video | 8-24 credits (4-12s) |
| Sora 2 (pro) | text/image-to-video | 24-120 credits (4-12s) |
| Veo 3.1 | text-to-video | 32-64 credits (4-8s) |
| Veo 3.1 Fast | text-to-video | 16-32 credits (4-8s) |
| Kling 1.6 Pro | image/text-to-video | 12-24 credits (5-10s) |
| Kling 2.1 Master | image/text-to-video | 40-80 credits (5-10s) |
| Seedance v1 Pro | image/text-to-video | 8-32 credits (5-10s) |
| Wan 2.5 | image/text-to-video | 8-32 credits (5-10s) |
| Minimax Hailuo 02 | image/text-to-video | 12-24 credits (standard), 20 (pro) |
| Nano Banana | text-to-image | 4 credits |
| Flux Pro | text/image-to-image | 4 credits |
| Seedream v4 | text/image-to-image | 4 credits |

### 3.4 Recipe: Image → Video B-Roll Pipeline

Generate a product photo first, then animate it.

```python
import time

def image_to_video_broll(image_prompt, video_prompt, video_model="kling-video/v1.6/pro/image-to-video"):
    """Pipeline: generate image → animate into video B-roll."""

    # Step 1: Generate product image
    image_job = generate_asset(
        model_name="nano-banana",
        input_params={"prompt": image_prompt}
    )

    # Step 2: Poll for image
    while True:
        status = check_generation_status(image_job["id"])
        if status["status"] == "done":
            image_url = status["assets"][0]["url"]
            break
        elif status["status"] in ("failed", "error"):
            raise Exception(f"Image gen failed: {status.get('failed_reason')}")
        time.sleep(5)

    # Step 3: Animate image into video
    video_job = generate_asset(
        model_name=video_model,
        input_params={
            "prompt": video_prompt,
            "image_url": image_url,
            "duration": "5",
            "aspect_ratio": "9:16",
        }
    )

    # Step 4: Poll for video
    while True:
        status = check_generation_status(video_job["id"])
        if status["status"] == "done":
            return status["assets"][0]["url"]
        elif status["status"] in ("failed", "error"):
            raise Exception(f"Video gen failed: {status.get('failed_reason')}")
        time.sleep(10)
```

---

## See Also

- [video-ad-generator](https://github.com/Creatify-AI/video-ad-generator) — Product URL → video ad pipeline
- [ai-avatar-video](https://github.com/Creatify-AI/ai-avatar-video) — AI talking-head videos with 1,500+ personas
- [ad-creative-evaluator](https://github.com/Creatify-AI/ad-creative-evaluator) — Score any video ad with AI expert panel
- [video-ad-reverse-engineer](https://github.com/Creatify-AI/video-ad-reverse-engineer) — Reverse-engineer competitor ads
- [static-ad-concept-generator](https://github.com/Creatify-AI/static-ad-concept-generator) — 320+ proven ad concept templates
