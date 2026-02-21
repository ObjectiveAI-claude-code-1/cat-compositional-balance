# cat-compositional-balance

Scores how well a cat is placed within a photograph's frame by evaluating intentionality of placement, spatial dialogue between subject and negative space, and compositional wholeness. Returns a scalar from 0 to 1 — high when placement feels purposeful and the frame feels built around the cat, low when it feels accidental.

## Input

The function accepts a single required field:

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `photograph` | `image` | Yes | Any photograph in which a cat is the subject. The image can range from professional studio portraits to casual phone snapshots, tightly cropped close-ups to wide landscape shots. The function examines the cat's position within the rectangle of the image and whether that placement produces compositional balance. |

## Output

A scalar score between **0** and **1**.

- **1.0** — The cat's placement radiates intentionality. The negative space and the subject are in perfect visual dialogue. The frame feels as though it was built around the cat in this exact position. Nothing is missing, nothing is extraneous.
- **0.5** — The cat's placement is adequate but unremarkable. There are hints of compositional consideration, but the arrangement doesn't fully commit to a strong choice. The photograph neither sings nor stumbles.
- **0.0** — The cat's placement feels arbitrary or careless. The subject appears to have ended up in its position by chance, the surrounding space serves no compositional purpose, and the photograph invites re-composition rather than resolution.

## What It Evaluates

The function assesses three distinct qualities. Each addresses a different dimension of the same core question — *does the cat belong exactly where it is?* — and together they form a complete picture of compositional balance.

### 1. Intentionality of Placement

Does the cat's position within the frame feel deliberately chosen, or does it feel accidental?

This evaluation reads the photograph itself — not the photographer's mind — to determine whether the cat's location communicates purpose. A cat centered with quiet symmetry, offset along a rule-of-thirds line, or partially hidden behind a doorframe in a way that serves a visual narrative all demonstrate intentionality. A cat awkwardly cropped at an edge, drifting out of frame as though it was about to leave, or placed with no discernible compositional logic does not.

The function does not prescribe a "correct" position. It asks whether the position that exists feels considered — as though someone or something decided that this was the spot.

### 2. Spatial Dialogue

How well do the cat and the negative space around it work together?

A photograph is not just a subject — it is a subject and everything that surrounds it. This evaluation measures whether the cat's visual weight and the surrounding empty space are in conversation, producing a sense of balance. When spatial dialogue is strong, the negative space feels purposeful: it gives the cat room to breathe, provides context and atmosphere, and anchors the subject within the frame. When it breaks down, the cat feels either suffocated — crammed against edges with no breathing room — or adrift in an aimless expanse that serves no compositional purpose.

The key question is whether subject and space are actively working together or merely coexisting without connection.

### 3. Compositional Wholeness

Does the photograph feel complete — like the frame was built around the cat?

This is the most holistic evaluation: the emergent sense that intentionality and spatial dialogue have combined to produce something that simply works. A photograph with strong compositional wholeness does not invite the viewer to re-compose it. You do not look at it and think the cat should be higher, or the crop should be tighter. Instead, you feel a quiet sense of resolution — the visual equivalent of a musical phrase landing on the tonic. The cat is where it is, the frame is what it is, and together they produce a closed circuit of compositional energy.

A photograph lacking this quality feels as though its composition is still searching for an arrangement that works.

## Use Cases

- **Photography culling**: Surface the strongest frames from a shoot by identifying the images where the cat's placement is most compositionally resolved.
- **Social media selection**: Help users choose the most visually compelling cat photograph from a set of candidates for posting.
- **Print and framing services**: Flag photographs where the cat's position may not hold up well when matted, mounted, and displayed on a wall.
- **Composition feedback**: Provide photographers with a signal about whether their framing choices are landing — whether the placement feels purposeful or like an afterthought.
- **Automated ranking**: Sort or filter large collections of cat photographs by the strength of their compositional balance.

## Important Notes

- The function evaluates **placement and composition only**. It does not assess the cat's beauty, the quality of the lighting, the interest of the background, or any other photographic quality beyond the cat's position within the frame.
- The function is **style-agnostic**. A centered composition, a rule-of-thirds offset, a tight crop, and a wide environmental shot can all score equally high, provided the placement feels intentional, the spatial relationship is balanced, and the composition feels whole.
- A high score does not mean a photograph is great. It means the cat's placement within the frame is working — purposeful, balanced, and complete.