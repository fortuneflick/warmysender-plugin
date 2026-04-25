# WarmySender Plugin for Claude

Cold email campaigns, email warmup, LinkedIn outreach, and 20M+ B2B lead database -- all accessible via natural language through Claude Code and Claude Cowork.

## Installation

```bash
claude plugin install warmysender
```

Or browse for it in the Claude Cowork plugin directory.

## What It Does

WarmySender connects Claude to your outreach platform via a remote MCP server at `https://warmysender.com/mcp`. OAuth 2.1 with PKCE handles authentication automatically.

| Category | Capabilities |
|----------|-------------|
| Campaigns | Create, manage, and monitor cold email campaigns with multi-step sequences |
| Prospects | Import, search, and manage prospect lists |
| Email Warmup | Configure and monitor email warmup settings and performance |
| Mailboxes | View connected mailboxes and delivery stats |
| LinkedIn | Manage LinkedIn outreach sequences and connections |
| B2B Leads | Search 20M+ verified contacts by industry, location, and job title |
| Suppressions | Manage suppression lists to protect sender reputation |

## MCP Server

Connects to the WarmySender remote MCP server at `https://warmysender.com/mcp` via OAuth 2.1 with PKCE. No API keys needed -- authentication is handled through the browser.

## Manual Setup (Claude Desktop)

Add to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "warmysender": {
      "command": "npx",
      "args": ["-y", "mcp-remote", "https://warmysender.com/mcp"]
    }
  }
}
```

## ChatGPT

1. Settings > Advanced > Enable Developer Mode
2. Settings > Connectors > Create
3. Paste: `https://warmysender.com/mcp`

## Links

- [WarmySender](https://warmysender.com) -- Main platform
- [Documentation](https://warmysender.com/documentation) -- API and feature docs
- [MCP Registry](https://registry.modelcontextprotocol.io) -- Listed as `com.warmysender/mcp`

## License

MIT
