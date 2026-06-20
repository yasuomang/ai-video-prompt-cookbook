# Same-Prompt Model Comparison Example

Same-prompt testing is not a perfect benchmark because each model may respond better to different prompt styles. It is still useful as a baseline when the goal is to compare workflow fit.

## Test Setup

```text
Use case: product image-to-video
Input image: one clean product start frame
Prompt versions:
  1. baseline prompt
  2. camera-specific prompt
  3. production prompt with preservation constraints
Evaluation: workflow scorecard
```

## Baseline Prompt

```text
Make this product image into a clean product video.
```

## Camera-Specific Prompt

```text
Slow push-in toward the product. Soft studio light moves across the surface.
```

## Production Prompt

```text
Slow push-in toward the product.
The product shape, label, color, and position stay unchanged.
Soft studio light moves across the surface.
Clean product-ad motion, no extra objects, no label distortion, no background replacement.
Vertical social video framing.
```

## What to Compare

- Did the product stay consistent?
- Did the motion match the camera instruction?
- Did the clip leave room for captions?
- How many attempts were needed?
- Which prompt version produced the most editable output?
