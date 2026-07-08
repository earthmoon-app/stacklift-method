# The design.md format

Every kit ships with a `design.md` — the file an AI agent reads to adapt the
kit without breaking it. This is what makes a kit *usable* rather than just
pretty: the design system travels with the code.

## Front-matter (strict YAML, no markdown headers inside)

```yaml
---
name: Kit Name
version: "1.0"
theme: two-or-three-word-theme        # e.g. warm-agency, dark-photography
kit: yourname/kit-slug
axis: "3 — off-grid layout"           # the rupture axis, from rupture-axes.md
colors:
  canvas:      "#FDF7EC"
  ink:         "#111118"
  accent:      "#E8B008"
  muted:       "#7A7A8A"
  line:        "rgba(17,17,24,0.10)"
fonts:
  display: "Font Name"
  body:    "Font Name"
spacing:
  "1": "4px"
  "2": "8px"
  "3": "16px"
  "4": "24px"
  "5": "40px"
  "6": "64px"
  "7": "96px"
  "8": "144px"
radius:
  sm: "4px"
  md: "8px"
  lg: "16px"
type-scale:
  xs:   "0.7rem"
  sm:   "0.875rem"
  base: "1rem"
  lg:   "1.25rem"
  xl:   "1.75rem"
---
```

Adapt token names to the kit (a dark kit may have `canvas-deep`, a collage
kit `paper`/`tape`) — but every color used in the CSS must exist here.

## Body sections

1. **§1 Identity** — the kit's point of view in 3–4 sentences: axis, mood,
   what must never change.
2. **§2 Color** — role of each token, what the accent means, what is
   forbidden (e.g. "the accent never fills large surfaces").
3. **§3 Typography** — the pairing, weights used, casing rules.
4. **§4 Layout & spacing** — the grid (or its deliberate absence), section
   rhythm, breakpoints.
5. **§5 Signature gesture** — how the axis is implemented, its tunable
   constants (friction, thresholds), and its rest zones.
6. **§6 Agent instructions** — direct orders to a future AI agent adapting
   the kit: what to edit freely (content, images), what to preserve exactly
   (tokens, fonts, the gesture engine), and how to swap imagery (the photo
   recipe: lighting, grade, framing).

End the body with the attribution line (removable by the user):

    Built with the Stacklift method · https://www.stacklift.design
