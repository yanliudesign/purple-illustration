# Examples

Three worked examples showing the range of the skill: a **collaborative product**, a **single-user creator tool**, and an **abstract dev/data tool**. Each example has:

- an **SVG mockup** of the target output (use it as your visual QA target)
- a **`.md` brief** with the fully-filled prompt (copy-paste into any image model)

| # | Composition | Product | Accent |
|---|---|---|---|
| 01 | A · laptop + UI card | [Group Copilot for Teams](./01-teams-copilot.md) | `#5B47F5` electric purple |
| 02 | C · single person + UI card | [AI writing assistant](./02-writing-assistant.md) | `#7C5CFF` default signal purple |
| 03 | E · abstract workspace | [Developer / data tool](./03-devtool-workspace.md) | `#3B6DFF` focus blue (shows accent is a variable) |

## How to use these

1. Pick the example whose composition and vibe match your product
2. Open its `.md` and copy the prompt
3. Swap the specific brand color, UI card content, and AI pill text for your product
4. Feed it to your image model of choice (GPT-image / Nano Banana / Midjourney / Flux)
5. Open the SVG side by side as a visual QA reference — line weight, layering, decoration density, no-shadow discipline
6. If the output drifts, use the local-edit prompts in [`../references/prompt-template.md`](../references/prompt-template.md#图像编辑局部修图提示)

## What the SVGs are (and aren't)

- ✅ Faithful visual targets that show how the four layers stack (background scene → UI card → AI pill → decorations)
- ✅ Editable — open in Figma / Illustrator to inspect exact positions, sizes, spacing
- ❌ Not the "final" illustration for these products — real generations will have subtly hand-drawn character features and more organic linework than pure SVG can convey
- ❌ Not templates — do not just recolor and ship; regenerate with your own product content per the skill's core rule ("UI card shows THIS product's most core screen")
