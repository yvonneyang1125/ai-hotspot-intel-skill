# ai-hotspot-intel-skill

A reusable Codex skill for generating a shareable daily AI hotspot intelligence roundup.

## What It Does

This skill focuses on the fact-based intelligence layer only:

- recent AI news and product updates
- platform trend capture
- public-search evidence from Douyin / Xiaohongshu / Bilibili
- categorized hotspot summaries
- follow-up links and discussion focus

## Skill Folder

The actual skill lives in:

- `ai-hotspot-intel-report/`

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

## 中文使用示例

```text
用 $ai-hotspot-intel-report 生成今天的 AI 热点情报汇总，覆盖过去 24-72 小时的模型发布、产品更新、社区讨论、GitHub Trending、Hugging Face Papers，以及抖音 / 小红书 / B站的公开搜索结果。输出要保留来源链接、标题、发布时间、可见热度和待补充项。
```

## Output Convention

By default, the skill is designed to write:

- `YYYY-MM-DD-AI热点情报汇总.md`

and keep the report neutral and shareable.
