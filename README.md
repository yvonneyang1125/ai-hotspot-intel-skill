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

## Output Convention

By default, the skill is designed to write:

- `YYYY-MM-DD-AI热点情报汇总.md`

and keep the report neutral and shareable.

The exact output directory should be chosen from the user's own workspace or knowledge base.

## Notes

- This repo does not include a creator-planning layer.
- It is intended for the intelligence / evidence layer first.
- If a platform requires login, captcha, or app-only access, the skill should not bypass those restrictions.
