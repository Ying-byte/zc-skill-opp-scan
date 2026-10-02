# 渠道现搜

Standard **MCP + Skill** for any Agent Host (Cursor / Claude Code / Codex / Zhencheng).

按岗位/地点/公司做渠道接口现搜；返回候选，不自动入库。

> One capability = one GitHub project. This folder is the sellable unit.

## Quick start

```bash
cd zc-skill-opp-scan
npm i
node stdio_mcp_server.mjs
```

## Cursor (`~/.cursor/mcp.json`)

```json
{
  "mcpServers": {
    "zc-skill-opp-scan": {
      "command": "node",
      "args": ["/ABS/PATH/zc-skill-opp-scan/stdio_mcp_server.mjs"]
    }
  }
}
```

Optional (use Zhencheng live tools):

```json
"env": {
  "ZC_AGENT_API_URL": "https://your-zhencheng-host",
  "ZC_MCP_TOKEN": "your-token"
}
```

## Tools

| Tool | Args |
|------|------|
| `search_jobs` | `query?` `jdText?` `profileText?` `location?` `notes?` `limit?` (number) |

## Skill

See `skills/zc-skill-opp-scan/SKILL.md`.

## License

MIT — see `LICENSE`.
