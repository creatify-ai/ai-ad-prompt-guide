# AI Model Catalog

Complete reference of available models for AI video and image generation.

## Video Models

### Sora 2 (OpenAI)
- **Type:** text-to-video, image-to-video
- **Durations:** 4s, 8s, 12s
- **Tiers:** Standard, Pro (720p/1080p)
- **Strengths:** Smooth camera movements, consistent lighting, fast generation
- **Weaknesses:** Fine text rendering, complex multi-person scenes
- **Best for:** Quick B-roll, establishing shots, product animations

### Veo 3.1 (Google)
- **Type:** text-to-video, image-to-video, first-last-frame-to-video, reference-to-video
- **Durations:** 4s, 6s, 8s
- **Tiers:** Standard, Fast
- **Strengths:** Best cinematic quality, physics coherence, long sequence consistency
- **Weaknesses:** Can be overly cinematic for casual content
- **Best for:** Hero content, brand videos, cinematic ads

### Kling (Kuaishou)
- **Type:** text-to-video, image-to-video
- **Versions:** v1.6 Pro, v2.1 Master
- **Durations:** 5s, 10s
- **Strengths:** Best image-to-video motion, face consistency, product animation
- **Weaknesses:** Higher cost at Master tier, slower generation
- **Best for:** Product showcases, face-driven content, image animation
- **Special:** `cfg_scale` parameter (0-1) controls prompt adherence

### Seedance v1 Pro (ByteDance)
- **Type:** text-to-video, image-to-video
- **Durations:** 5s, 10s
- **Resolutions:** 480p, 720p, 1080p
- **Strengths:** Natural human motion, dance/movement, body language
- **Weaknesses:** Less suitable for non-human subjects
- **Best for:** UGC-style content, avatar content, human-centric ads

### Wan 2.5 Preview
- **Type:** text-to-video, image-to-video, text-to-image, image-to-image
- **Durations:** 5s, 10s
- **Resolutions:** 480p, 720p, 1080p
- **Strengths:** Versatile (video AND image), good cost/quality ratio
- **Weaknesses:** Preview quality (may improve)
- **Best for:** Budget-conscious video at longer durations

### Minimax Hailuo 02
- **Type:** text-to-video, image-to-video
- **Durations:** 6s, 10s
- **Tiers:** Standard, Pro
- **Strengths:** Consistent quality, reliable output
- **Weaknesses:** Less distinctive style
- **Best for:** Reliable batch generation, B-roll at scale

### Veo 3 Fast (Google, Previous Gen)
- **Type:** text-to-video, image-to-video
- **Durations:** 4s, 6s, 8s
- **Note:** Previous generation. Use Veo 3.1 for better quality.

## Image Models

### Nano Banana (Creatify)
- **Type:** text-to-image, image-to-image (edit)
- **Strengths:** Best text rendering, logo fidelity, product photography
- **Weaknesses:** Image only (no video)
- **Best for:** Product shots, text-heavy images, reference images for I2V

### Flux Pro (Black Forest Labs)
- **Type:** text-to-image, image-to-image (Kontext)
- **Versions:** v1.1-ultra, kontext, kontext/max/multi, redux
- **Strengths:** Image editing, style transfer, compositing, high resolution
- **Weaknesses:** Less creative freedom than pure gen models
- **Best for:** Editing existing images, style transfer, multi-image compositing

### Seedream v4 (ByteDance)
- **Type:** text-to-image, image-to-image (edit)
- **Strengths:** High quality image generation, good editing
- **Weaknesses:** Newer model, less established
- **Best for:** General image generation, image editing
