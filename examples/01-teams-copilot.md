# 01 · Group Copilot for Microsoft Teams

**Composition**: A. Laptop + foreground UI card  
**Accent**: `#5B47F5` (electric purple)  
**Aspect**: 3:2 (900 × 600)

## Brief

Product: a Copilot bot inside Microsoft Teams that reads a group chat and produces a shared summary the whole team can post with one tap. AI initiates the summary; humans decide whether to post or edit first.

## Target output

See [`01-teams-copilot.svg`](./01-teams-copilot.svg) — an SVG mock of what a "good" generation should look like. Use it as a visual reference / final QA target.

## Prompt (copy into any image model)

```text
A clean modern SaaS product hero illustration, 3:2 horizontal composition, pure white background (#FFFFFF).

STYLE:
Flat vector line illustration, uniform medium-weight black line art (~2pt), no hand-drawn wobble, no shadows, no gradients, no textures, no noise, no 3D, no isometric. Only ONE accent color used throughout: purple (#5B47F5), as solid fills for decorative bubbles, brand icons, sparkles, and small accents. Warm peach skin tone (#F4C7A8) for character faces only. Solid black hair. Minimal 2-3 stroke facial features. Everything is flat, no shading anywhere.

LAYER 1 — BACKGROUND SCENE:
An open laptop drawn in clean black line art, positioned on the left half of the canvas, sitting on a thin horizontal desk line that fades out at both ends. The laptop screen shows a 4-person video call grid — each participant a simple flat line-drawn portrait with warm peach skin and solid black hair. A small potted plant with a few outlined leaves sits to the left of the laptop. Background occupies only 55-65% of the frame.

LAYER 2 — FOREGROUND UI CARD:
A tall rounded-rectangle app window floating on the right, overlapping the laptop's right half. The card has:
- Top-left: three small window dots (red, yellow, green); top-right: a small solid purple circular brand icon
- Title in bold black: "Product Sync — chat" with light-gray subtitle "4 participants · today 10:00"
- Three message rows, each with a warm-skin line-art avatar, bold name (Ken · Sarah · Marco), light-gray timestamp, and one line of real content
- A soft-purple-tinted summary block labeled "Copilot summary" with three bullet lines: "3 decisions captured / 2 blockers flagged / 5 action items owned"
- A solid purple "Post to thread" pill button and a text link "Edit first"
- Modern sans-serif UI typography (Inter / SF Pro feel), no lorem ipsum
- No drop shadow — floats via layering only

LAYER 3 — AI PROMPT PILL:
A small white rounded-pill overlay sitting on the top edge of the UI card, with a thin purple (#5B47F5) outline, a solid purple sparkle ✦ on the left, the text "Summarize this thread" in the middle in black, and a small black hand-cursor pointer icon on the right edge.

LAYER 4 — SCATTERED DECORATIONS (4-5 total, distributed around the card):
- A solid purple rounded speech bubble with 3 short white horizontal lines inside, floating in the upper-left near the laptop
- An outlined black-only speech bubble with 3 short black lines inside, floating on the right side of the UI card
- A small tilted purple pencil at ~30° in the lower area
- A small purple four-point sparkle ✦ near the top-right corner of the UI card
- A white circle with a thin black outline containing the Microsoft Teams logo (a purple "T" on a rounded square), attached to the left edge of the laptop

CONSTRAINTS:
- Pure white background, no color wash, no gradient, no paper grain, no noise
- Exactly ONE accent color (#5B47F5) — no rainbow, no blue, no green
- No drop shadows, no glow, no blur, no 3D
- UI card must clearly overlap and cut into the laptop behind it (essential)
- No watermark, no "AI-generated" text, no emoji stickers
```
