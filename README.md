# ai-hotspot-intel-skill

A reusable Codex skill for generating a shareable daily AI hotspot intelligence roundup.

The repo is intentionally generic and does not include any user-specific local paths, private vault names, or personal browser-profile locations.

## Use Cases

This repo is useful when you want to:

- produce a daily AI news and product roundup
- summarize AI platform trends with links and visible signals
- collect public-search evidence from platforms such as Douyin, Xiaohongshu, and Bilibili
- generate a shareable intelligence brief before any creator-specific planning
- save the result into a local knowledge base, workspace, or notes system

## What It Does

This skill focuses on the fact-based intelligence layer only:

- recent AI news and product updates
- platform trend capture
- public-search evidence from Douyin / Xiaohongshu / Bilibili
- categorized hotspot summaries
- follow-up links and discussion focus

## What It Expects

The skill works best when the user can provide or confirm:

- a target output directory
- the desired time window, usually the last 24-72 hours
- preferred platforms or sources to emphasize
- local browser login state for platforms with partial public access

## Output Shape

The generated report is designed to stay neutral and shareable. Typical sections include:

- daily overview
- platform observations
- public-search records
- grouped hotspots
- discussion focus
- follow-up links
- platforms that still need screenshots, links, or login-state help

## Skill Folder

The actual skill lives in:

- `ai-hotspot-intel-report/`

## Repository Layout

```text
ai-hotspot-intel-skill/
├── README.md
└── ai-hotspot-intel-report/
    ├── SKILL.md
    └── agents/
        └── openai.yaml
```

## Install

Copy the skill folder into your local Codex skills directory:

```bash
mkdir -p ~/.codex/skills/ai-hotspot-intel-report
cp -R ai-hotspot-intel-report/. ~/.codex/skills/ai-hotspot-intel-report/
```

## Invoke

Use it in Codex with:

```text
Use $ai-hotspot-intel-report to produce today's shareable AI hotspot intelligence roundup.
```

## English Example

```text
Use $ai-hotspot-intel-report to generate today's AI hotspot intelligence roundup for the last 24-72 hours, with source links, visible platform signals, grouped themes, and clear `待补充` markers where access is limited.
```

## 中文使用示例

```text
用 $ai-hotspot-intel-report 生成今天的 AI 热点情报汇总，覆盖过去 24-72 小时的模型发布、产品更新、社区讨论、GitHub Trending、Hugging Face Papers，以及抖音 / 小红书 / B站的公开搜索结果。输出要保留来源链接、标题、发布时间、可见热度和待补充项。
```

## 中文快速开始

### 1. 安装 skill

先把 skill 复制到本地 Codex skills 目录：

```bash
mkdir -p ~/.codex/skills/ai-hotspot-intel-report
cp -R ai-hotspot-intel-report/. ~/.codex/skills/ai-hotspot-intel-report/
```

### 2. 准备输出目录

在你的本地知识库或工作区里准备一个用于存放日报的目录，例如：

```text
<你的知识库>/AI内容号/06-AI热点日报/
```

也可以用任意你自己的目录，例如：

```text
<你的工作区>/reports/ai-hotspots/
```

### 3. 直接调用

在 Codex 里输入类似下面的话：

```text
用 $ai-hotspot-intel-report 生成今天的 AI 热点情报汇总，覆盖过去 24-72 小时，输出到 <你的目录>/2026-07-05-AI热点情报汇总.md。
```

如果你希望强调特定来源，也可以直接补进去：

```text
用 $ai-hotspot-intel-report 生成今天的 AI 热点情报汇总，重点覆盖 OpenAI、Anthropic、Google DeepMind、GitHub Trending、Hugging Face Papers、Reddit、YouTube，以及抖音 / 小红书 / B站的公开搜索结果。
```

### 4. 你会得到什么

通常会输出一份中性、可分享的 Markdown 文件，常见内容包括：

- 今日总览
- 主流平台观察
- 平台公开搜索记录
- 热点分组
- 讨论焦点
- 可跟进链接
- 需要你补充/登录的平台
- 明天继续盯

### 5. 如果平台需要登录

这个 skill 不会绕过登录、验证码、App 限制或反爬限制。

更推荐的做法是：

- 你在本机浏览器里先登录相关平台
- 保留专用研究浏览器的登录态
- 或者把截图、链接、导出数据提供给 Codex 再整理

看不到的数据要明确写 `待补充`，不要猜测或编造。

### 6. 一个更完整的中文调用示例

```text
用 $ai-hotspot-intel-report 生成今天的 AI 热点情报汇总，覆盖过去 24-72 小时。重点关注模型发布、Agent / Workflow、AI 编程、研究与开源、国内外平台视频趋势。请覆盖 OpenAI、Anthropic、Google DeepMind、Meta AI、Microsoft AI、Product Hunt、Hacker News、GitHub Trending、Hugging Face Papers、arXiv，以及抖音 / 小红书 / B站 / YouTube / Reddit / 知乎。输出保存到 <你的目录>/YYYY-MM-DD-AI热点情报汇总.md，并保留来源链接、标题、发布时间、可见热度、讨论焦点和待补充项。
```

## Output Convention

By default, the skill is designed to write:

- `YYYY-MM-DD-AI热点情报汇总.md`

and keep the report neutral and shareable.

The exact output directory should be chosen from the user's own workspace or knowledge base.

## Notes

- This repo does not include a creator-planning layer.
- It is intended for the intelligence / evidence layer first.
- If a platform requires login, captcha, or app-only access, the skill should not bypass those restrictions.
