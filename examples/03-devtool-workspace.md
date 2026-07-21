# 03 · Developer / Data Tool

**Composition**: E. Abstract workspace (no character)  
**Accent**: `#3B6DFF` (Focus Blue) — **demonstrates that the accent color is a variable, not fixed to purple**  
**Aspect**: 3:2 (900 × 600)

## Brief

Product: a SQL / data workspace where the user types natural language and the tool generates the query. No people in the scene — the focus is the tool itself and the module cards floating around it.

## Target output

See [`03-devtool-workspace.svg`](./03-devtool-workspace.svg).

## Prompt

```text
A clean modern SaaS product hero illustration, 3:2 horizontal composition, pure white background (#FFFFFF).

STYLE:
Flat vector line illustration, uniform medium-weight black line art (~2pt), no hand-drawn wobble, no shadows, no gradients, no textures, no noise, no 3D, no isometric. Only ONE accent color used throughout: blue (#3B6DFF), as solid fills for decorative bubbles, brand icons, sparkles, chart bars, code keywords, and small accents. NO other accent color. No skin tones, no characters in this composition.

LAYER 1 — BACKGROUND SCENE (abstract workspace):
Three small module cards float in the left half of the canvas, each in clean black line art on white:
- A calendar snippet card labeled "Aug 2026" with a 5x3 grid and one date circled in solid blue
- A weekly-runs bar chart card with 7 blue vertical bars of increasing height and a "+12%" indicator
- A "Runners" settings card with an outlined gear icon on the left, "us-east · 4 active" text, and a small blue pill
The cards are staggered vertically. A small blue "PG" logo circle is attached to the top-left of the calendar card. A thin dashed horizontal desk line sits at the bottom-left. Background occupies only 55-60% of the frame.

LAYER 2 — FOREGROUND UI CARD (SQL query builder):
A large rounded-rectangle app window floating on the right, overlapping the module cards behind. The card has:
- Top-left: three small window dots (red, yellow, green); top-right: a small solid blue circular brand icon
- Title in bold black: "query · orders_daily" with a light-gray subtitle "postgres · warehouse-prod"
- A code editor block with a soft blue-tinted background (#F7F8FF) and a numbered gutter (1-7). Each line shows real SQL:
   SELECT date_trunc('day', created_at) AS d,
          count(*) AS orders,
          sum(total) AS gmv
   FROM orders
   WHERE created_at > now() - interval '30 days'
   GROUP BY 1
   ORDER BY 1;
- SQL keywords (SELECT, FROM, WHERE, GROUP BY, ORDER BY) rendered in bold blue (#3B6DFF); rest of the code in black monospaced type
- Below the editor: a result table with header row (day · orders · gmv) and three data rows of realistic numbers
- A solid blue "Run" pill button, a "Save as view" outlined blue pill, and a light-gray "last run · 2s ago" caption
- Modern sans-serif UI + monospaced code (Inter + SF Mono / JetBrains Mono feel), no lorem ipsum
- No drop shadow

LAYER 3 — AI PROMPT PILL:
A small white rounded-pill overlay on the top edge of the UI card, with a thin blue (#3B6DFF) outline, a solid blue sparkle ✦ on the left, the text "Generate this query for me" in the middle in black, and a small black hand-cursor pointer icon on the right edge.

LAYER 4 — SCATTERED DECORATIONS (4-5 items):
- A solid blue rounded speech bubble with 3 short white horizontal lines inside, floating in the upper-right near the card
- A small blue four-point sparkle ✦ just above the top-right of the UI card
- An outlined black-only speech bubble with 2 short black lines inside, floating in the bottom-right
- A three-dot horizontal loader in blue floating below the card (two solid + one lighter blue) — represents "querying"
- No plants, no coffee cups — the vibe is workspace-abstract, not personal-desk

CONSTRAINTS:
- Pure white background, no color wash, no gradient, no paper grain, no noise
- Exactly ONE accent color (#3B6DFF) — no purple, no green, no red
- No shadows, no glow, no 3D, no isometric
- UI card must clearly overlap the module cards behind it
- Code inside the card must be legible, correct SQL, not lorem ipsum
- No watermark, no "AI-generated" text, no emoji stickers
```
