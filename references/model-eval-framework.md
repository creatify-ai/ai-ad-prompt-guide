# Model Evaluation Framework

How to systematically test and compare AI generation models for your specific use case.

## Evaluation Criteria

### Visual Quality (Score 1-10)
- **Resolution clarity**: Is the output sharp at intended display size?
- **Color accuracy**: Do colors match the prompt description?
- **Detail level**: Fine details (textures, edges, small objects) rendered well?
- **Consistency**: Are elements consistent throughout the clip?

### Motion Quality (Video Only, Score 1-10)
- **Smoothness**: No jitter, no frame drops?
- **Physics adherence**: Objects move naturally? Gravity, inertia respected?
- **Camera movement**: Smooth camera paths? No sudden jumps?
- **Subject motion**: Natural movement of people, objects, liquids?

### Prompt Adherence (Score 1-10)
- **Subject match**: Does the output contain what was described?
- **Composition match**: Is the layout/framing as specified?
- **Mood match**: Does the lighting/atmosphere match?
- **Action match**: Is the described action happening?

### Practical Metrics
- **Generation time**: How long from submit to complete?
- **Success rate**: What percentage of generations are usable?
- **Cost per usable output**: Credits/dollars per output that passes quality check
- **Iteration speed**: How quickly can you test prompt variations?

## Evaluation Protocol

### Step 1: Create Test Prompts
Create 5 standardized test prompts that cover your use cases:
1. Simple product on white background
2. Product in lifestyle context
3. Person using product (hardest for AI)
4. Abstract/mood B-roll
5. Your most common real use case

### Step 2: Run Each Model
- Generate each prompt 3 times per model (AI output varies)
- Record: time, cost, usability (yes/no), quality score
- Save all outputs for comparison

### Step 3: Score Matrix

```
| Model | Prompt | Quality | Motion | Adherence | Time | Cost | Usable? |
|-------|--------|---------|--------|-----------|------|------|---------|
| Sora 2 | #1 | 7 | 7 | 8 | 45s | 8cr | Yes |
| Veo 3.1 | #1 | 9 | 9 | 9 | 90s | 32cr | Yes |
| Kling 2.1 | #1 | 8 | 8 | 7 | 120s | 40cr | Yes |
```

### Step 4: Calculate Cost Per Usable Output
```
Cost per usable output = (Total credits spent) / (Number of usable outputs)
```

If Model A costs 8 credits but only 50% are usable, effective cost = 16 credits.
If Model B costs 32 credits but 90% are usable, effective cost = 35 credits.
Sometimes the "expensive" model is cheaper per usable output.

### Step 5: Decision
Select models by use case tier:
- **Hero content** (homepage, primary ad): Best quality model
- **Testing/iteration** (prompt refinement, A/B hooks): Fastest/cheapest model
- **Batch production** (catalog-scale generation): Best cost/quality ratio

## Model Selection Cheat Sheet

```
FAST ITERATION:
  Images → Nano Banana (4 credits, seconds)
  Video → Sora 2 standard (8 credits, ~45 seconds)

PRODUCTION QUALITY:
  Images → Flux Pro or Nano Banana
  Video → Veo 3.1 or Kling 2.1 Master

BEST VALUE:
  Short video (5s) → Seedance v1 Pro at 480p (8 credits)
  Long video (10s) → Wan 2.5 at 480p (16 credits)

SPECIFIC NEEDS:
  Product animation → Kling 2.1 Master (image-to-video)
  Human motion → Seedance v1 Pro
  Cinematic → Veo 3.1
  Text in image → Nano Banana
  Image editing → Flux Pro Kontext
```
