# AI Video Prompt Cookbook

> **Publish status:** REVISION_DRAFT
> **Resource cluster:** `templates-reusable-assets`
>
> Use this draft only to repair the already-published GitHub README. Do not publish it as a new page until the linked LumiYing targets exist, the examples are checked, and this status is changed to `READY`.

Practical prompt patterns for creators testing image-to-video and text-to-video workflows.

This cookbook is for creators, marketers, and small content teams who need usable AI video clips, not one-off demo prompts. It focuses on source image prep, motion wording, preservation constraints, repeatable testing, and failure review.

## Who This Is For

- Product marketers turning one product image into a short ad clip.
- Social creators testing hooks, UGC-style motion, and vertical framing.
- Brand teams that need a repeatable way to compare AI video outputs.
- Editors who need clips that can still be cropped, captioned, and reused.

This is not an API integration guide. The goal is to make prompt testing easier for people who judge the output visually.

## Prompt Card Format

Use one prompt card per test so the idea, constraints, and result stay connected.

```text
Clip job:
Source image:
Subject to preserve:
Motion:
Camera:
Framing:
Style:
Negative constraints:
Success criteria:
Result notes:
Next change:
```

The two most important fields are `Subject to preserve` and `Motion`. Many weak AI video prompts describe the image again, but they do not explain what should move.

## Image-to-Video Product Prompt

Use this when the source image is already the creative anchor.

```text
Clip job: 5-second vertical product ad.
Source image: one clear studio image of the product.
Subject to preserve: keep the product shape, cap, label, color, and position unchanged.
Motion: soft light sweeps across the product surface while small background shadows move naturally.
Camera: slow push-in with stable framing.
Framing: 9:16 vertical, leave clean space near the top for a caption.
Style: realistic ecommerce product video, polished but not over-stylized.
Negative constraints: no extra objects, no label distortion, no melted edges, no background replacement.
Success criteria: product stays recognizable and the clip can be used in a short ad edit.
```

## UGC-Style Hook Prompt

Use this when the output needs to feel like a creator shot, but the product still needs to stay readable.

```text
Clip job: creator-style social hook for a product recommendation.
Source image: product held near a simple tabletop background.
Subject to preserve: keep the product label, package shape, and hand position stable.
Motion: subtle handheld movement, product tilts slightly toward camera, natural light shifts.
Camera: close vertical phone shot, mild handheld energy, no dramatic zoom.
Framing: 9:16, product centered, room for captions on the lower third.
Style: clean UGC product clip, realistic, casual, not cinematic.
Negative constraints: no fake text overlays, no changed packaging, no extra hands, no warped fingers.
Success criteria: the product is readable in the first second and can support a voiceover.
```

## Same-Prompt Model Test

When comparing models, keep the job and prompt stable. Do not change the prompt after seeing the first result, or the comparison becomes a prompt rewrite test instead of a model comparison.

```text
Test name: Product bottle, slow push-in, vertical ad.
Input: same source image for every model.
Prompt version: v1, unchanged for the first round.
Models tested: Model A, Model B, Model C.
Scoring: subject fidelity, motion coherence, prompt adherence, editability, retry cost.
Decision: keep, retry with constraints, or reject for this job.
```

## Evaluation Scorecard

| Criterion | Weight | What to Check |
| --- | ---: | --- |
| Subject fidelity | 30% | Product, character, or object stays recognizable |
| Motion usefulness | 20% | Motion starts early and supports the clip job |
| Prompt adherence | 20% | Camera, framing, and constraints are followed |
| Editability | 20% | Clip can be captioned, cropped, or placed in a sequence |
| Retry cost | 10% | Number of regenerations needed for a usable result |

Do not keep a clip just because it looks impressive. Keep it only if it solves the original clip job.

## Failure Notes

| Failure | What It Looks Like | Next Prompt Change |
| --- | --- | --- |
| Product drift | Shape, color, or label changes | Add stricter preservation constraints and simplify the source image |
| Background takeover | Background moves more than the subject | Ask for subtle environmental motion and no background replacement |
| Text distortion | Labels or UI text becomes unreadable | Avoid generating new text; add text later in editing |
| Motion too static | First seconds barely move | Describe motion that starts immediately |
| Over-cinematic output | Clip looks like a trailer, not a usable ad | Lower style intensity and specify platform/use case |

## Suggested Folder Structure

```text
ai-video-prompt-cookbook/
  product-video-prompts/
  ugc-ad-prompts/
  same-prompt-tests/
  failure-notes/
  scorecards/
```

## LumiYing References

Existing useful target:

- Image-to-video workflow: https://lumiying.com/tools/image-to-video

Planned targets to add before this draft becomes `READY`:

- AI video prompt builder
- AI video evaluation scorecard
- AI video prompt template library
- Same-prompt AI video comparison guide

## License

MIT for prompt templates and scorecard structures. Adapt them to your own product, brand, safety rules, and editing workflow.
