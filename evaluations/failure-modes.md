# Common AI Video Failure Modes

| Failure | Signal | Prompt Fix |
| --- | --- | --- |
| Product drift | Shape, label, or color changes during motion | Add preservation constraints and use a cleaner start frame |
| Identity drift | Face or outfit changes | Use subtle motion and stronger identity preservation language |
| Camera jump | Sudden or chaotic camera movement | Use locked camera, slow push-in, or gentle orbit |
| Text distortion | Generated labels or UI text becomes unreadable | Avoid generated text; add real text in editing |
| Background replacement | Scene changes unexpectedly | Add "no background replacement" and simplify the start image |
| Delayed motion | Clip stays static too long | Describe motion that begins immediately |
| Overproduction | Clip is too cinematic for product use | Use minimal product-ad style and reduce camera intensity |
| Moderation rejection | Prompt or image triggers policy filters | Remove sensitive claims, unsafe likeness use, or restricted content |

## Failure Note Format

```text
Observed failure:
Where it appears:
Likely cause:
Prompt change:
Asset change:
Try same model again:
Try different model:
```

Do not only save successful clips. Failure notes are what make the next prompt more repeatable.
