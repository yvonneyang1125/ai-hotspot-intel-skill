# ai-hotspot-intel-skill

A reusable Codex skill for generating a shareable daily AI hotspot intelligence roundup.

## What It Does

This skill focuses on the fact-based intelligence layer only:

- recent AI news and product updates
- platform trend capture
- public-search evidence from Douyin / Xiaohongshu / Bilibili
- categorized hotspot summaries
- follow-up links and discussion focus

It does not include creator-specific content planning.

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

## Output Convention

By default, the skill is designed to write:

- `YYYY-MM-DD-AI热点情报汇总.md`

and keep the report neutral and shareable.

