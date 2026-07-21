---
name: saas-illustration
description: SaaS 产品英雄插画风格 —— 单一品牌强调色 + 真产品 UI 卡片 + 线稿场景。用于官网首屏、Landing Page、Feature Section、Blog Header、演讲首页，以及邻近场景（技术 talk 封面、portfolio featured project、workshop landing、research paper 顶图、产品发布邮件顶图）。把"一个真实的产品 UI 卡片"叠在"线稿场景（笔电/桌面/协作场景）"之上，配以品牌强调色的漂浮装饰（聊天气泡、小图标、logo、植物）。视觉特征：纯白底、黑色矢量线稿、单一品牌强调色（默认紫 #7C5CFF，可换任意品牌 HEX）+ 温暖肤色、干净不手绘、UI 卡越出后景边界。默认输出可直接喂给 Nano Banana / GPT-image / Midjourney / Flux 的英文提示词。关键词：SaaS illustration, SaaS hero illustration, product hero, landing page illustration, 官网插画, 产品首屏, feature illustration, hero image, purple illustration, 紫色插画, 单强调色插画, single-accent illustration, duotone illustration, Tactiq 风格, Superhuman 风格, Linear 风格。
---

# SaaS Illustration（SaaS 产品英雄插画）

## 核心定位

为 SaaS / AI 产品的**营销场景**生成一张干净、专业、可信、能"一眼看懂产品在做什么"的英雄插画。不是解释性配图，不是漫画，不是手绘草图，也不是概念艺术——是一张**能直接放在官网首屏或博客顶图**的插画。

同 DNA 也适用于**邻近的数字产品场景**：技术 talk 封面、portfolio featured project 卡、workshop / course landing page、research paper 顶图、产品发布邮件顶图、内部 all-hands / 路线图封面 —— 任何"一个可展示的 artifact + 一个品牌色"的组合都走这个 skill。

标志性动作：**真产品 UI 卡片漂浮在前景 + 线稿场景在后景 + 少量品牌色装饰散落周围**。

## 先读这些参考

按任务需要读取：

- `references/style-dna.md` — 调色板、线条、材质、禁忌
- `references/composition-patterns.md` — 5 种主构图套路 + 装饰物摆放法
- `references/prompt-template.md` — 单张生图提示词模板（含变量）
- `references/qa-checklist.md` — 生成后检查和迭代规则

## 工作流

### 1. 只问 3 个问题（一次性发出，不要一问一答）

```
Q1. 你的产品是什么？
    一句话：品类 + 核心功能。
    e.g. "一个 AI 会议纪要工具，自动抓决策和 action items"

Q2. 想要的主题色是？
    给我一个 HEX。没有的话就用默认紫 #7C5CFF。
    e.g. #5B47F5

Q3. UI 卡片想展示什么信息？
    越具体越好 —— 真实文案、数字、字段名、按钮文字。
    e.g. "一份 Q3 launch retro 会议纪要 · 标题 + 3 条决策（带责任人）+ 2 条 blocker + 底部 Post 按钮"
```

**发问规则**：三个问题一起发，一次性等回复。用户答全了直接走下一步；只答了一部分再补问，不要重复已经答过的。

### 2. 从答案自动推断其余参数（**不要再问**）

从 Q1 的品类 + Q3 的内容型态推断，不要让用户选。

| 要决定的 | 推断规则 |
|---|---|
| **主构图** | 团队协作 / 会议类 → **A**（笔电+视频会议）；移动 / 消费 / 通讯 → **B**（手机）；创作者 / 写作 / 单人生产力 → **C**（单人）；白板 / 共享文档 / 双人协作 → **D**（双人）；API / 开发者 / 数据 / 基础设施 → **E**（抽象工作空间无人物） |
| **画面比例** | 默认 3:2 横版 landing hero；用户明说 blog / social / slide 场景再换（16:9 / 1:1） |
| **人物数量** | 跟随主构图（A=3-4 视频头像；B=0；C=1；D=2；E=0） |
| **AI pill 文案** | 从 Q1 的核心功能提炼成一句 imperative 短句（"Summarize this thread" / "Draft a reply" / "Generate this query"），4-6 词 |
| **装饰物 3-5 件** | 从产品品类挑：写作 → 铅笔+便签；会议 → 摄像头+对话气泡；数据 → 图表碎片；开发 → sparkle+光标；协作 → 多方气泡+第三方 logo（Teams/Slack/Notion） |

推断有多个合理选项时，选**该品类最常见的那个**，不要停下来问用户。

### 3. 出提示词

用 `references/prompt-template.md` 填变量，一次性输出**一段可复制的英文提示词**。

- UI 卡片内容用 **Q3 的原文**（真实文案 > 通用占位）
- 强调色用 **Q2 的 HEX**，全图只用这一个色
- **不要停下来等确认**；直接出 prompt

### 4. 检查与迭代

生成后按 `references/qa-checklist.md` 自查。最常见的失败：
- UI 卡画得太抽象、不像真产品
- 装饰物太多，喧宾夺主
- 出现渐变、阴影、纸纹、噪点、3D 感
- 强调色被误用到 UI 卡内部（应该只用于装饰和 UI 卡里的品牌点缀）
- 人物有阴影/腮红/复杂五官（应该扁平线稿）

给出**局部编辑提示词**修补，不要让用户全部重生成。

### 5. 交付

- **只交付提示词**：默认模式，用户拿去自己的图像模型生。
- **写入 workspace**：如果在 workspace 内工作且用户明确要求保存，写入 `assets/<slug>-hero/01-topic.png` 占位说明文件 + 提示词 `.md`。

## 输出口径

一次交付包含：

1. **配图策略**（2-4 行）：为什么选这个构图、UI 卡展示什么、装饰用什么
2. **可复制的完整英文提示词**（放在代码块里，方便一键复制）
3. **可选的备用变体**（换构图 / 换视角 / 换装饰组合，最多 2 个）
4. **迭代提示片段**（"如果 XX 不对，追加这句话"）

不要写风格理论解说，也不要生成 shot list 一样长的清单——这个 skill 的输出是**一张可直接生成的插画**，不是多图 story。

## 与其他 skill 的边界

- **不要与 `ian-xiaohei-illustrations` 混用**。Ian 风格是白纸手绘怪诞正文配图；这个 skill 是干净矢量 SaaS 营销插画，两者美学正相反。
- **不要与 `atutun-xhs-cover` 混用**。那是小红书竖版真人封面。
- **不要与 `cover-design-open` 混用**。那是公众号封面。
- 如果用户想给一篇中文文章配"正文插图"（低密度、怪诞、白底手绘），走 `ian-xiaohei-illustrations`。
- 如果用户想做产品官网首图、feature section 插画、SaaS blog 顶图，走**本 skill**。
