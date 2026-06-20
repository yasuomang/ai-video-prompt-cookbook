# AI Video Workflow Scorecard

Use this scorecard to evaluate outputs by workflow usefulness, not only visual quality.

| Criterion | Weight | What to Check |
| --- | ---: | --- |
| Subject fidelity | 25% | Product, character, or object stays recognizable |
| Motion coherence | 20% | Motion is smooth and starts early enough |
| Prompt adherence | 20% | Output follows camera, style, and duration instructions |
| Editability | 20% | Clip can be cropped, captioned, or placed in a sequence |
| Iteration cost | 15% | Number of regenerations needed for a usable result |

## Review Template

```text
Use case:
Input type:
Prompt version:
Model:
Attempt number:
Subject fidelity:
Motion coherence:
Prompt adherence:
Editability:
Iteration cost:
Failure notes:
Decision:
```

## Decision Labels

- `use`: suitable for editing or publishing.
- `revise prompt`: usable direction, needs prompt changes.
- `try another model`: prompt is clear but model fit is weak.
- `discard`: output fails core constraints.
