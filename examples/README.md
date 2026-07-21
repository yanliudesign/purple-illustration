# Examples

Three real generations that came out of this skill's prompt template, kept as **canonical reference outputs**. Each has:

- the **rendered PNG** — what "good" looks like
- a **`.md` brief** — the exact prompt used, so you can reproduce or riff on it

<p>
  <img src="./01-teams-copilot.png"      width="32%" alt="Group Copilot approval">
  <img src="./02-meetly-transcript.png"  width="32%" alt="Meetly live transcript">
  <img src="./03-meetly-agenda.png"      width="32%" alt="Meetly pre-meeting agenda">
</p>

| # | Composition | Scenario | Accent |
|---|---|---|---|
| [01](./01-teams-copilot.md) | C · single person + UI card | Copilot drafted a plan, human is about to tap **Approve** | `#5B47F5` |
| [02](./02-meetly-transcript.md) | A · laptop + UI card | Meetly listens to a live meeting, surfaces a "Decision detected" card | `#5B47F5` |
| [03](./03-meetly-agenda.md) | A · laptop + UI card | Meetly drafts a pre-meeting agenda 12 min before the call | `#5B47F5` |

## How to use these

1. Pick the example whose composition and moment match your product
2. Open its `.md`, copy the prompt block, and paste into your image model of choice (GPT-image / Nano Banana / Midjourney / Flux)
3. Swap the specific brand color, UI card content, and AI pill text for your product
4. When the output drifts, use the local-edit prompts in [`../references/prompt-template.md`](../references/prompt-template.md#图像编辑局部修图提示)
5. Cross-check against [`../references/qa-checklist.md`](../references/qa-checklist.md) before shipping

## Why 02 and 03 share a product

They're the same product (**Meetly**) at two different moments — *before* the meeting and *during* the meeting. A single skill can carry one product's identity across a whole marketing site: same character DNA, same accent color, same decoration vocabulary, different UI cards.
