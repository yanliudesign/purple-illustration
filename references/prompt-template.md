# 生图提示词模板

一次输出一张。默认交付**英文提示词**，因为 Nano Banana / GPT-image / Midjourney / Flux 对英文风格描述最稳。

## 主模板（复制填变量即可）

```text
A clean modern SaaS product hero illustration, {ASPECT_RATIO} horizontal composition, pure white background (#FFFFFF).

STYLE:
Flat vector line illustration, uniform medium-weight black line art (~2pt), no hand-drawn wobble, no shadows, no gradients, no textures, no noise, no 3D, no isometric. Only ONE accent color used throughout: {ACCENT_COLOR_NAME} ({ACCENT_HEX}), as solid fills for decorative bubbles, brand icons, sparkles, and small accents. Warm peach skin tone (#F4C7A8) for character faces and hands only. Solid black hair. Minimal 2-3 stroke facial features. Everything is flat, no shading anywhere.

LAYER 1 — BACKGROUND SCENE (line art only):
{BACKGROUND_SCENE_DESCRIPTION}
A very thin horizontal line under the scene suggesting a desk surface, fading out at both ends. Keep the background scene occupying only 60-70% of the frame — the right portion is intentionally overlapped by the foreground UI card.

LAYER 2 — FOREGROUND UI CARD (photorealistic product mockup, still vector-flat):
A tall rounded-rectangle app window floating in the foreground, overlapping the background scene. The card has:
- Top-left: three small window dots (red, yellow, green) and a tiny {ACCENT_COLOR_NAME} brand logo icon
- Content: {UI_CARD_CONTENT}
- Real, legible, specific text — no lorem ipsum
- 2-3 avatar circles with warm-skin line-art portraits, bold name in black, light-gray timestamp (#9CA3AF)
- Modern sans-serif UI typography (Inter / SF Pro feel)
- No drop shadow on the card — it floats via layering only

LAYER 3 — AI PROMPT PILL (signature element):
A small white rounded-pill overlay on the UI card, with a thin {ACCENT_COLOR_NAME} outline, a solid {ACCENT_COLOR_NAME} sparkle ✦ icon on the left, the action text "{AI_PILL_TEXT}" in the middle, and a small black hand-cursor pointer icon on the right edge.

LAYER 4 — SCATTERED FLOATING DECORATIONS (3-5 items total, evenly distributed around the UI card):
{DECORATION_LIST}
Decorations must float around the UI card — not touch the ground, not clump on one side.

CONSTRAINTS:
- Pure white background, absolutely no color wash, no gradient sky, no paper grain
- Exactly ONE accent color ({ACCENT_HEX}) — no rainbow, no secondary accent
- No drop shadows, no glow, no blur, no depth of field, no 3D
- UI card must clearly overlap and cut into the background scene (this is essential)
- Main subject occupies 55-70% of canvas, 30-45% clean white space around edges
- Illustration must look like it belongs on a modern SaaS company's landing page (Linear / Superhuman / Tactiq / Notion aesthetic)
- Do NOT add any watermark, "AI-generated" text, emoji stickers, or decorative typography
```

## 变量说明

| 变量 | 示例值 |
|---|---|
| `{ASPECT_RATIO}` | `3:2` (默认 landing hero) / `16:9` (blog header) / `1:1` (社交) |
| `{ACCENT_COLOR_NAME}` | `purple` / `blue` / `green` / `coral` / `teal` / `amber` |
| `{ACCENT_HEX}` | `#7C5CFF` 等，用户给的品牌色优先 |
| `{BACKGROUND_SCENE_DESCRIPTION}` | 见下方场景库 |
| `{UI_CARD_CONTENT}` | 用户产品的最核心一屏，具体到文案 |
| `{AI_PILL_TEXT}` | 一句产品的核心 AI 行动，例如 `Summarize this thread` |
| `{DECORATION_LIST}` | 见下方装饰库 |

## 场景库（填 `{BACKGROUND_SCENE_DESCRIPTION}`）

**A. 笔电 + 视频会议**
```
An open laptop drawn in clean black line art, positioned on the left side of the canvas. The laptop screen shows a 4-person video call grid — each participant a simple flat line-drawn portrait with warm peach skin and solid black hair. A small potted plant with a few leaves sits to the left of the laptop.
```

**B. 手机 + 通知**
```
A vertical smartphone drawn in clean black line art, standing on a subtle desk line, positioned center-left. The phone screen shows a simple app notification with an avatar and a message preview.
```

**C. 单人角色**
```
A half-body line-art character positioned center-left, warm peach skin, solid black hair, wearing a simple sweater outlined in black, gesturing toward the foreground UI card with one hand, calm smile.
```

**D. 双人协作**
```
Two half-body line-art characters standing side by side on the left, both with warm peach skin and solid black hair, both facing and looking toward the foreground UI card, one holding a small notebook.
```

**E. 抽象工作空间**
```
A flat top-down suggestion of a workspace: a floating stack of small UI module cards (calendar snippet, a small chart, a settings gear) arranged loosely in the left half of the canvas, all in clean black line art with occasional accent-color fills.
```

## 装饰库（填 `{DECORATION_LIST}`，选 3-5 个）

```
- A solid {ACCENT_COLOR_NAME} rounded speech bubble with 2-3 short white horizontal lines inside, floating in the upper-left near the UI card
- An outlined (black-only) speech bubble with 2-3 black horizontal lines inside, floating on the right side of the UI card
- A small tilted {ACCENT_COLOR_NAME} pencil floating in the lower area, at about 30° angle
- A white circle with a thin black outline containing a recognizable third-party app icon (e.g., Teams / Zoom / Slack / Notion / Figma), attached to the left edge of the laptop
- A small {ACCENT_COLOR_NAME} four-point sparkle ✦ near the top-right corner of the UI card
- A partial rounded-rectangle notification card in a very light {ACCENT_COLOR_NAME} tint, half-hidden behind the main UI card
```

## 图像编辑（局部修图）提示

**UI 卡太抽象、想让它更像真产品：**
```
Edit the provided illustration. Keep everything the same except redraw the foreground UI card to look more like a real modern SaaS app screenshot: add a clear top bar with three window dots, replace the generic content with a specific message thread containing 2-3 named user rows with avatars, bold names, and light-gray timestamps. Keep the same {ACCENT_HEX} accent color, same flat vector style, no shadows.
```

**装饰太多 / 太乱：**
```
Edit the provided illustration. Remove all decorative floating elements except: one solid {ACCENT_COLOR_NAME} speech bubble on the upper left, one small tilted {ACCENT_COLOR_NAME} pencil at the bottom. Keep the UI card, the background scene, and the AI prompt pill exactly as they are. Fill removed areas with clean white background.
```

**出现了阴影 / 渐变：**
```
Edit the provided illustration. Remove all drop shadows, gradients, glows, and depth-of-field effects. Everything must be perfectly flat: solid fills only, uniform line weights, pure white background. The layering effect between the UI card and background should come purely from overlap, not from any shadow.
```

**强调色跑歪 / 出现第二种颜色：**
```
Edit the provided illustration. Remove any color other than: pure white background, black line art, warm peach skin (#F4C7A8), and the single accent color {ACCENT_HEX}. Recolor any stray red / green / other accents back to the single {ACCENT_HEX}.
```

**AI pill 缺失或不显眼：**
```
Edit the provided illustration. Add a small white rounded-pill overlay on the foreground UI card with a thin {ACCENT_HEX} outline, a solid {ACCENT_HEX} four-point sparkle ✦ icon on the left, the text "{AI_PILL_TEXT}" in black in the middle, and a small black hand-cursor pointer icon on the right edge. The pill should sit slightly off the edge of the card to feel like a live UI suggestion.
```
