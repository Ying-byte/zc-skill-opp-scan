---
name: zc-skill-opp-scan
description: >-
  按岗位/地点/公司做渠道接口现搜；返回候选，不自动入库。
  Use in any Agent Host that can mount stdio MCP. Pair with zc-skill-opp-scan.
---

# 渠道现搜 · Skill

## When to use

- User asks for: 渠道现搜
- 按岗位/地点/公司做渠道接口现搜；返回候选，不自动入库。

## Tools (`zc-skill-opp-scan`)

| Tool | Args |
|------|------|
| `search_jobs` | query, jdText, profileText, location, notes, limit |

## Example

```json
{
  "query": "Frontend Engineer",
  "location": "remote",
  "jdText": "<paste JD>",
  "profileText": "<paste profile>"
}
```

## Limits

- Do not invent employers, dates, or numbers
- Do not apply or send email unless the user confirms
- Unknown facts must be marked unknown

## Host install

Mount this repo as stdio MCP (see README). Not Zhencheng-only.
