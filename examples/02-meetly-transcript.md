# 02 · Meetly — live transcript & decision detection

**Composition**: A. Laptop + foreground UI card  
**Accent**: `#5B47F5` (electric purple)  
**Aspect**: ~16:10 landscape

![Meetly live transcript](./02-meetly-transcript.png)

## What this illustration says

*During the meeting*: Meetly listens to the video call in the background and quietly surfaces a "Decision detected" card the moment the group commits to something. The AI is present but doesn't interrupt — it earns its place by capturing what would otherwise slip.

## Prompt

```text
A clean modern SaaS product hero illustration, ~16:10 horizontal composition, pure white background (#FFFFFF).

STYLE:
Flat vector line illustration, uniform medium-weight black line art (~2pt), no hand-drawn wobble, no shadows, no gradients, no textures, no noise, no 3D, no isometric. Only ONE accent color used throughout: purple (#5B47F5), as solid fills for decorative bubbles, brand icons, sparkles, selection highlights, and small accents. Warm peach skin tone (#F4C7A8) for character faces only. Solid black hair. Minimal 2-3 stroke facial features. Everything is flat.

LAYER 1 — BACKGROUND SCENE:
An open laptop drawn in clean black line art, positioned on the left half of the canvas, sitting on a thin horizontal desk line that fades out at both ends. The laptop screen shows a 2x2 video call grid — four participants, each a simple flat line-drawn portrait with warm peach skin and solid black hair. The top-right video tile has a solid purple (#5B47F5) border indicating "active speaker", and a small solid purple circle overlay on that tile containing a white microphone icon. A small potted plant with a few outlined leaves sits to the left of the laptop. A white circle with a thin black outline containing a video camera icon is attached to the top-left edge of the laptop. Background occupies only ~55% of the frame.

LAYER 2 — FOREGROUND UI CARD (Meetly · Live transcript):
A tall rounded-rectangle app window floating on the right, overlapping the laptop's right half. The card has:
- Top-left: three small window dots (red, yellow, green)
- Top-center: a small solid purple "M" logo mark next to the wordmark "Meetly" in bold black
- A small red dot + "REC 12:34" recording indicator (red dot is the ONLY red allowed in the illustration)
- Large bold black heading: "Live transcript"
- Three message rows, each with a warm-skin line-art circular avatar, bold speaker name, a middle dot, a timestamp (10:03 / 10:04 / 10:05), and a light-gray "#9CA3AF" style hex tag on the far right (mimicking a color tag), plus 2 lines of real transcript text below:
   • Sarah — "I think the drop-off is in the third onboarding step, not the second."
   • Ken — "Agree — the analytics data from last week supports that."
   • Priya — "Should we A/B test a simpler version this sprint?"
- Below the transcript, a soft-purple-tinted (#F1EEFF) rounded rectangle block labeled with a solid purple bullet + bold "Decision detected", and a second line containing the decision text: "Test simpler onboarding step 3 next sprint."
- Modern sans-serif UI typography (Inter / SF Pro feel), real legible text, no lorem ipsum
- No drop shadow — floats via layering only

LAYER 3 — AI PROMPT PILL:
A wide white rounded-pill overlay sitting on the bottom-right edge of the UI card, slightly offset outward, with a thin purple (#5B47F5) outline, a solid purple circular badge with a white sparkle ✦ inside on the far left, the text "Highlight decisions in real time" in the middle in bold black, and a small black hand-cursor pointer icon on the right edge.

LAYER 4 — SCATTERED FLOATING DECORATIONS (4-5 items):
- A solid purple rounded speech bubble with 2-3 short white horizontal lines inside, floating in the upper-left between the laptop and the card
- A small solid purple four-point sparkle ✦ near the top-right corner of the UI card
- A solid purple speech bubble containing a white microphone icon, floating on the right side of the card at roughly mid-height
- An outlined black-only speech bubble with a single short black line inside, floating on the right side of the card at lower height

CONSTRAINTS:
- Pure white background, no color wash, no gradient, no paper grain
- Exactly ONE accent color (#5B47F5) — the only exception is the small red "REC" dot
- No drop shadows, no glow, no blur, no 3D
- UI card must clearly overlap the laptop behind it
- The "active speaker" video tile must be visually distinguished by a purple border + purple mic overlay
- No watermark, no "AI-generated" text, no emoji stickers
```
