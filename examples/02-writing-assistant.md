# 02 · AI Writing Assistant

**Composition**: C. Single person + foreground UI card  
**Accent**: `#7C5CFF` (default signal purple)  
**Aspect**: 3:2 (900 × 600)

## Brief

Product: a writing app that suggests a sharper opening line for a draft, in the author's own voice. The human is present in the scene, reaching toward the card — communicating "the human still decides".

## Target output

See [`02-writing-assistant.svg`](./02-writing-assistant.svg).

## Prompt

```text
A clean modern SaaS product hero illustration, 3:2 horizontal composition, pure white background (#FFFFFF).

STYLE:
Flat vector line illustration, uniform medium-weight black line art (~2pt), no hand-drawn wobble, no shadows, no gradients, no textures, no noise, no 3D. Only ONE accent color used throughout: purple (#7C5CFF), as solid fills for decorative bubbles, brand icons, sparkles, and small accents. Warm peach skin tone (#F4C7A8) for character face and hands only. Solid black hair. Minimal 2-3 stroke facial features. Everything is flat, no shading.

LAYER 1 — BACKGROUND SCENE:
A half-body line-art character positioned center-left, warm peach skin, solid black hair in a shoulder-length bob, wearing a simple crew-neck sweater outlined in black, calm confident expression with 2-stroke eyes and a small smile. One arm extends toward the foreground UI card, hand open as if about to tap it. A thin horizontal desk line fades out at both ends behind the character. Background occupies only 55-60% of the frame.

LAYER 2 — FOREGROUND UI CARD:
A tall rounded-rectangle document window floating in the center-right, overlapping the character's outstretched hand. The card has:
- Top-left: three small window dots (red, yellow, green); top-right: a small solid purple circular brand icon
- A slim toolbar with B / I / U icons, H1, H2, and a "Draft · saved" indicator in light gray
- Bold document title in black: "On-call rotation, redesigned"
- Four horizontal lines representing body paragraphs
- A highlighted suggestion block with a soft purple background (#F5F1FF) and a purple left border, labeled "SUGGESTED — sharper opener" in small purple caps, containing three lines of the suggested rewrite in real English
- An "Accept" solid-purple pill button, a "Rewrite" purple text link, and a light-gray "Dismiss" link
- Three more body lines below
- Modern sans-serif UI typography, no lorem ipsum
- No drop shadow — floats via layering only

LAYER 3 — AI PROMPT PILL:
A small white rounded-pill overlay on the top edge of the UI card, with a thin purple (#7C5CFF) outline, a solid purple sparkle ✦ on the left, the text "Rewrite in your voice" in the middle in black, and a small black hand-cursor pointer icon on the right edge.

LAYER 4 — SCATTERED DECORATIONS (4 items):
- A solid purple oval thought bubble with 3 short white horizontal lines inside, floating above the character's head, with two small trailing dots
- A small tilted purple pencil at ~30° in the bottom-right corner
- A small purple four-point sparkle ✦ near the top-right corner of the UI card
- A small light-purple (#F0EAFF) note card with 3 thin lines, half-hidden behind the main UI card on the right side
- An outlined black-only speech bubble with 2 short black lines inside, floating in the bottom-left

CONSTRAINTS:
- Pure white background, no wash, no gradient, no texture
- Exactly ONE accent color (#7C5CFF)
- No shadows, no glow, no 3D
- The character's hand must clearly reach toward / point at the UI card
- UI card must overlap the character's hand
- No watermark, no meta text, no emoji stickers
- No blush, no eye highlights, no cartoon expression — minimal 2-3 stroke face
```
