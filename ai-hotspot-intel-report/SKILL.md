---
name: ai-hotspot-intel-report
description: Produce a shareable AI hotspot intelligence roundup from the last 24-72 hours. Use when the user wants AI news collection, platform trend capture, source-based hotspot summaries, public-search evidence from Douyin/Xiaohongshu/Bilibili, categorized daily AI briefings, or an Obsidian-ready `AI热点情报汇总` file without creator-specific content strategy.
---

# AI Hotspot Intel Report

Use this skill to generate the fact-only daily AI hotspot intelligence document.

Default vault:

`/Users/yvonneyang/Desktop/羊会卷/杨一万的知识库`

Default output directory:

`/Users/yvonneyang/Desktop/羊会卷/杨一万的知识库/AI内容号/06-AI热点日报`

## Use This Skill For

- Daily or ad hoc AI hotspot intelligence collection
- Shareable AI news roundups that should stay neutral
- Platform observation across Douyin, Xiaohongshu, Bilibili, YouTube, X, Reddit, Zhihu, WeChat official accounts, and similar sources
- Public-search evidence capture from Douyin / Xiaohongshu / Bilibili
- Fact-based categorized AI briefings for teams or friends

Do not use this skill for creator-facing topic judgment, script angles, or account-specific content recommendations. Use `yangyiwan-content-planner` for that layer.

## Output Rule

Write one file directly under the hotspot directory using this fixed name:

`YYYY-MM-DD-AI热点情报汇总.md`

Do not create a date subfolder unless the user explicitly asks for that structure.

## Report Boundary

Keep the document shareable and neutral. Include:

- facts
- links
- visible metadata
- platform observation
- grouped hotspots
- discussion focus
- follow-up links
- what still needs user-supplied login or screenshots

Do not include:

- "杨一万应该怎么拍"
- content-angle recommendations for a specific account
- topic priority judgments aimed at a creator workflow

## Required Sections

Follow the structure in:

`/Users/yvonneyang/Desktop/羊会卷/杨一万的知识库/AI内容号/06-AI热点日报/热点情报模板.md`

At minimum, preserve these sections:

1. 今日总览
2. 主流平台观察
3. 平台公开搜索记录
4. 热点分组
5. 讨论焦点
6. 可跟进链接
7. 需要你补充/登录的平台
8. 明天继续盯

## Platform Access Rules

Use the dedicated research browser profile when platform login state is needed:

`/Users/yvonneyang/Documents/ds&AI/.browser-profiles/ai-hotspot-research`

If access is blocked, login expires, or a captcha appears:

- do not bypass restrictions
- keep collecting from other public sources
- mark the affected item `待补充`
- state what the user should provide locally: screenshot, link, or exported data

Never record passwords, one-time codes, cookies, recovery codes, or raw tokens.

## Evidence Standard

For each useful hotspot, prefer to capture:

- source
- title
- link
- date
- account or author
- visible engagement signals when publicly visible

If a metric is not visible, write `待补充` instead of inferring.

## Category Standard

Group hotspots under:

1. 模型与产品发布
2. Agent / Workflow / 企业落地
3. AI 编程与工具链
4. 研究、开源与数据
5. 国内平台视频趋势
6. 海外平台视频趋势

Each item should explain:

- what happened
- why it is hot now
- source link

## File Hygiene

- Keep Chinese concise and scannable
- Favor links over unsupported claims
- Avoid copying long third-party text
- Keep the file useful even when shared outside the Yang Yiwan workflow

