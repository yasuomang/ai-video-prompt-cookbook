# Camera Moves and Shot Terms

Use standard camera words and put them in the `Camera:` field, separate from subject motion. Models are less likely to mix up "the camera moves" with "the subject moves" when the two sit in different lines.

## Camera Movement

| Term | What It Does | Prompt Wording |
| --- | --- | --- |
| Static / locked-off | No camera movement; only the subject moves | `camera locked off on a tripod, no movement` |
| Push-in / dolly in | Moves toward the subject, adds focus or intensity | `slow dolly in toward the product` |
| Pull-out / dolly out | Reveals context around the subject | `camera slowly pulls back to reveal the room` |
| Pan left/right | Rotates horizontally from a fixed point | `slow pan right across the shelf` |
| Tilt up/down | Rotates vertically from a fixed point | `camera tilts up from the shoes to the face` |
| Tracking / truck | Moves alongside the subject | `camera tracks alongside the runner at shoulder height` |
| Orbit / arc | Circles the subject | `camera orbits 180 degrees around the bottle` |
| Crane / jib | Rises or lowers vertically | `crane shot rising above the market crowd` |
| Aerial / drone | High, sweeping movement | `aerial drone shot gliding over the coastline` |
| Handheld | Slight natural shake, documentary or UGC feel | `handheld, subtle natural shake` |
| FPV | Fast first-person drone, swooping moves | `FPV drone dives down and skims the river` |
| Dolly zoom | Background stretches while the subject stays the same size | `dolly zoom on the man as the hallway stretches behind him` |
| Whip pan | Very fast pan, often used as a cut | `quick whip pan to the right` |
| Rack focus | Focus shifts between foreground and background | `rack focus from the raindrops on the glass to the face behind it` |

## Shot Size

| Shot | Use It For | Prompt Wording |
| --- | --- | --- |
| Extreme wide | Establishing place, scale | `extreme wide shot, small figure in a vast desert` |
| Wide | Full body plus surroundings | `wide shot, full body visible` |
| Medium | Waist up; a safe default for people | `medium shot, waist up` |
| Close-up | Face or product detail | `close-up on the label` |
| Macro | Texture, liquids, small details | `macro shot of coffee crema swirling` |

## Angle and Lens

- `low angle`: subject feels larger or more powerful.
- `high angle` / `top-down`: subject feels smaller; works well for flat lays and desk scenes.
- `eye level`: neutral, natural for talking-to-camera clips.
- `24mm wide-angle`: more space, slight edge distortion.
- `50mm`: natural perspective.
- `85mm portrait, shallow depth of field`: soft background, subject isolation.
- `anamorphic, horizontal lens flares`: cinematic widescreen look.

## Practical Rules

- One camera move per clip. "Push-in then orbit then crane up" in 5 seconds usually turns messy.
- If the camera is ignored, write it as its own sentence and use the plain terms above.
- If you want only the subject to move, say `camera locked off`. Don't leave the camera field blank.
- Keep the same camera wording when comparing models, so the test stays fair (see [Same-Prompt Test](../examples/same-prompt-test.md)).
