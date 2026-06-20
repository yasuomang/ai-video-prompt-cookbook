# AI Video Prompt Cookbook

Practical prompt patterns for image-to-video and text-to-video workflows.

This cookbook is built for creators, marketers, and developers who want repeatable AI video workflows instead of one-off demo prompts. It focuses on prompt structure, source image quality, motion constraints, model comparison, and failure review.

## What Is Included

- Image-to-video prompt templates
- Text-to-video prompt templates
- Product video prompt patterns
- Social ad prompt patterns
- Same-prompt model comparison notes
- Failure mode checklists
- Evaluation rubrics for real workflows

## Core Prompt Structure

```text
Subject:
Input type:
Camera movement:
Motion description:
Style:
Duration:
Aspect ratio:
Preservation constraints:
Negative constraints:
Evaluation notes:
```

## Recommended Workflow

1. Pick one use case: product demo, social ad, explainer, cinematic concept, or creator short.
2. Prepare a strong source image if using image-to-video.
3. Write one baseline prompt and two controlled variations.
4. Run the same prompt set across your chosen model or model workspace.
5. Score outputs by consistency, subject fidelity, motion coherence, editability, and regeneration cost.
6. Save the winning prompt with notes about what failed.

For a browser-based image-to-video workflow, see LumiYing's image-to-video tool:
https://lumiying.com/tools/image-to-video

For API-oriented notes around Seedance workflows, see:
https://lumiying.com/resource/seedance-2-api

## Folder Structure

```text
prompts/
  image-to-video/
  text-to-video/
  product-videos/
  social-ads/
evaluations/
examples/
```

## License

MIT for code-like examples and prompt templates. Use the prompts as starting points and adapt them to your own project, brand, and safety constraints.
