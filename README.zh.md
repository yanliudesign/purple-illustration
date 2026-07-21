<div align="center">

**中文** · [English](./README.md)

# 🎨 SaaS 插画

---

**单一品牌色的 SaaS 产品英雄插画 — 真实 UI 卡片 × 线稿场景 × 一个强调色。**

[![License](https://img.shields.io/badge/LICENSE-MIT-4c8bf5?style=flat-square&labelColor=333)](./LICENSE)
[![Version](https://img.shields.io/badge/VERSION-1.0.0-2ea44f?style=flat-square&labelColor=333)]()
[![Examples](https://img.shields.io/badge/EXAMPLES-3-2ea44f?style=flat-square&labelColor=333)](./examples)
[![Stars](https://img.shields.io/github/stars/yanliudesign/saas-illustration?style=flat-square&label=STARS&color=e37f2c&labelColor=333)](https://github.com/yanliudesign/saas-illustration/stargazers)

[![Claude Code](https://img.shields.io/badge/Claude_Code-Skill-d97757?style=flat-square&labelColor=1a1a1a&logo=anthropic&logoColor=white)](https://claude.ai/code)
[![Codex](https://img.shields.io/badge/Codex-Skill-2ea44f?style=flat-square&labelColor=1a1a1a)]()
[![OpenCode](https://img.shields.io/badge/OpenCode-Skill-4c8bf5?style=flat-square&labelColor=1a1a1a)]()
[![OpenClaw](https://img.shields.io/badge/OpenClaw-Skill-8b5cf6?style=flat-square&labelColor=1a1a1a)]()
[![Hermes](https://img.shields.io/badge/Hermes-Skill-e879a8?style=flat-square&labelColor=1a1a1a)]()

</div>

一个"审美克制"的 skill，把任何 SaaS 产品的一句话简报变成**能直接放在官网首屏、Blog 顶图、Feature Section** 的英雄插画。标志性动作：**真产品 UI 卡片漂浮在前景 + 线稿场景在后景 + 一个品牌强调色**做所有点缀。

不是解释性配图，不是漫画，不是手绘 zine，不是概念艺术。就是当代 SaaS 那种收敛、专业、能过设计评审的插画 —— Linear · Superhuman · Tactiq · Notion 那种手感，用一段 prompt 生出来。

**同 DNA 也适用于邻近的数字产品场景** —— 技术 talk 封面、portfolio featured project 卡、workshop / course landing page、research paper 发布图、产品发布邮件顶图、内部 all-hands / 路线图封面。只要能凑出"一个可展示的 artifact + 一个品牌色 + 一个干净场景"，就走这个 skill。

<p align="center">
  <img src="./examples/01-teams-copilot.png"      width="32%" alt="Group Copilot approval">
  <img src="./examples/02-meetly-transcript.png"  width="32%" alt="Meetly live transcript">
  <img src="./examples/03-meetly-agenda.png"      width="32%" alt="Meetly pre-meeting agenda">
</p>

## 目录

| 文件 | 作用 |
|---|---|
| [`SKILL.md`](./SKILL.md) | Skill 主入口 —— Claude 读它来决定何时 / 如何触发 |
| [`references/style-dna.md`](./references/style-dna.md) | 调色板、线条、材质、禁忌 |
| [`references/composition-patterns.md`](./references/composition-patterns.md) | 5 种主构图 + 装饰物摆放法 |
| [`references/prompt-template.md`](./references/prompt-template.md) | 单张生图提示词模板（含变量 · 场景库 · 装饰库） |
| [`references/qa-checklist.md`](./references/qa-checklist.md) | 生成后检查清单 + 常见问题的局部修图提示 |
| [`examples/`](./examples/) | 3 张真实生成图 + 可复制 prompt |

## 三条铁律

1. **只有一种强调色。** 不允许彩虹。任何跑出来的第二种颜色都是 bug。紫色只是默认，你可以换成任何品牌 HEX。
2. **UI 卡必须是"真产品"。** 展示的是**这个产品**最核心的一屏 —— 真人名、真数字、真文案。不写 lorem ipsum，不画通用聊天窗。
3. **靠层叠，不靠阴影。** 卡片"浮起来"是因为它遮住了后景，而不是因为投影。禁止 glow、渐变、3D、isometric。

## 安装

丢到 Claude Code 的 skills 目录：

```bash
git clone https://github.com/yanliudesign/saas-illustration.git \
  ~/.claude/skills/saas-illustration
```

重启 Claude Code。触发关键词见 [`SKILL.md`](./SKILL.md) 顶部。

## 触发关键词

| 你说 | 会触发 |
|---|---|
| *"给我做张官网首图 / Landing page hero illustration"* | 本 skill |
| *"Feature section 配图 / Blog 顶图"* | 本 skill |
| *"技术 talk 封面 / portfolio 首图 / workshop landing 插画"* | 本 skill |
| *"我要 Linear / Superhuman 那种插画"* | 本 skill |
| *"紫色插画"* / *"purple illustration"* / *"one-brand-color illustration"*（历史别名） | 本 skill |

## 适用

- **SaaS 一切营销表面** —— 官网首屏、Feature Section、Pricing 页配图、Blog 顶图、Twitter 发布卡片
- **B2B / 企业级产品发布** —— 发布邮件顶图、Changelog 封面、PLG 风格的新功能高亮
- **需要"专业感"的商务内容** —— 投资人 deck 封面、pitch deck、融资页 hero、白皮书封面
- **开发者 / 技术内容** —— 技术 talk 封面、Conference 首图、Dev blog 顶图、API 文档头图、SDK release notes
- **AI / 数据 / Research** —— Research paper 封面、model card 顶图、AI 产品发布图、evals dashboard
- **教育 / Workshop / 课程** —— Course landing、Bootcamp 招生页、Workshop 报名页、Notion 学习模块
- **Portfolio / Case study** —— Featured project 卡、Case study 顶图、设计师 / PM / 工程师个人网站 hero

## 什么时候**不要**用

- **娱乐 / 影视 / 游戏推广图** —— 需要氛围和戏剧张力，UI 卡在这儿没意义
- **消费品 / 时尚 / 美妆 / 餐饮** —— 需要真实产品照 + 情绪，不是矢量线稿
- **小说 / 童书 / 漫画 / 出版物封面** —— 需要叙事插画，不是营销屏
- **音乐会 / 展览 / 活动海报** —— 那是排版设计，不是产品插画
- **中文文章正文的怪诞手绘配图** （风格完全相反）
- **小红书 / 抖音 真人爆款封面**
- **编辑类杂志 / 报刊插图** —— 需要艺术性和故事感

## 交付格式

一次交付给你：

1. **配图策略**（2–4 行：为啥选这个构图、UI 卡展示什么、装饰用什么）
2. **可直接复制的英文 prompt**（代码块里）
3. **可选备用变体**（最多 2 个：换构图 / 换视角 / 换装饰）
4. **局部修图提示**（"如果 XX 跑歪了，追加这句"）

不写风格理论解说，不生成 shot-list 长清单。这个 skill 是为"出一张图"优化的。

## License

MIT — see [LICENSE](./LICENSE).
