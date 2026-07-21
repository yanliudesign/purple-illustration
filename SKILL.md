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

### 1. 问清关键参数

如果用户没说全，问最少的问题拿到这些：

| 参数 | 必须 | 默认值 |
|---|---|---|
| 产品是什么、核心功能 | ✅ | — |
| 品牌强调色（HEX） | ✅ | 若无则用 `#7C5CFF`（紫）作占位 |
| UI 卡片要展示什么内容 | ✅ | — |
| 后景场景（笔电/手机/办公桌/协作场景等） | 可选 | 笔电 + 视频会议 |
| 人物数量（0 / 1 / 2 / 小组） | 可选 | 视频会议里 3-4 人小头像 |
| 画面比例 | 可选 | 3:2 横版（landing hero）；1:1 备选；16:9 备选 |

不要为了问而问；能推断就直接推断。

### 2. 构图选型

从 `composition-patterns.md` 里选**一种**主构图。默认走 **A. 笔电 + 前景 UI 卡**，因为它最泛用。其他选项：

- B. 手机 + 前景 UI 卡（适合 mobile-first 产品）
- C. 单人 + 前景 UI 卡（适合创作者工具）
- D. 双人协作 + 前景 UI 卡（适合团队协作产品）
- E. 抽象工作空间 + 前景 UI 卡（无人物，适合基础设施类产品）

### 3. 出提示词

用 `references/prompt-template.md` 填变量，一次性输出一段可复制的英文提示词。**不要停下来等确认**，除非用户给的信息真的不够。

如果 UI 卡片内容很具体（例如要展示某段真实的产品对话/表格/日程），把内容原文放到提示词里让模型渲染。

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
