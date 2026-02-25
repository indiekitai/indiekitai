# 🛠️ IndieKit

**Open-source tools that make developers's lives easier.**

We port proven libraries across languages and make them agent-friendly with [MCP](https://modelcontextprotocol.io) support.

## 🔧 Tools

### PostgreSQL Toolkit
| Package | Description | npm |
|---------|-------------|-----|
| [@indiekitai/pg-inspect](https://github.com/indiekitai/pg-inspect) | Schema inspection — tables, views, indexes, functions, and more | [![npm](https://img.shields.io/npm/v/@indiekitai/pg-inspect)](https://www.npmjs.com/package/@indiekitai/pg-inspect) |
| [@indiekitai/pg-diff](https://github.com/indiekitai/pg-diff) | Schema diff — compare databases, generate migration SQL | [![npm](https://img.shields.io/npm/v/@indiekitai/pg-diff)](https://www.npmjs.com/package/@indiekitai/pg-diff) |
| [@indiekitai/pg-top](https://github.com/indiekitai/pg-top) | Real-time activity monitor — like `top` for PostgreSQL | [![npm](https://img.shields.io/npm/v/@indiekitai/pg-top)](https://www.npmjs.com/package/@indiekitai/pg-top) |
| [@indiekitai/pg2ts](https://github.com/indiekitai/pg2ts) | Generate TypeScript types from your database schema | [![npm](https://img.shields.io/npm/v/@indiekitai/pg2ts)](https://www.npmjs.com/package/@indiekitai/pg2ts) |

### Developer Tools
| Package | Description | npm |
|---------|-------------|-----|
| [@indiekitai/just](https://github.com/indiekitai/just-ts) | Command runner — TypeScript port of [casey/just](https://github.com/casey/just) | [![npm](https://img.shields.io/npm/v/@indiekitai/just)](https://www.npmjs.com/package/@indiekitai/just) |
| [@indiekitai/throttled](https://github.com/indiekitai/throttled) | Rate limiting — 5 algorithms, memory + Redis backends | [![npm](https://img.shields.io/npm/v/@indiekitai/throttled)](https://www.npmjs.com/package/@indiekitai/throttled) |
| [@indiekitai/lipgloss](https://github.com/indiekitai/lipgloss-ts) | Terminal styling & layout — TypeScript port of [charmbracelet/lipgloss](https://github.com/charmbracelet/lipgloss) | [![npm](https://img.shields.io/npm/v/@indiekitai/lipgloss)](https://www.npmjs.com/package/@indiekitai/lipgloss) |
| [@indiekitai/env-audit](https://github.com/indiekitai/env-audit) | Scan code for env vars, generate .env.example | [![npm](https://img.shields.io/npm/v/@indiekitai/env-audit)](https://www.npmjs.com/package/@indiekitai/env-audit) |

## 🤖 MCP — One Config, All Tools

```json
{
  "mcpServers": {
    "indiekit": {
      "command": "npx",
      "args": ["@indiekitai/mcp"]
    }
  }
}
```

16 tools across 8 packages. Auto-discovers new packages when installed.

[![npm](https://img.shields.io/npm/v/@indiekitai/mcp?label=@indiekitai/mcp)](https://www.npmjs.com/package/@indiekitai/mcp)

## 🌐 Links

- 🏠 [indiekit.ai](https://indiekit.ai)
- 🐦 [@indiekitai](https://twitter.com/indiekitai)
- 📦 [npm org](https://www.npmjs.com/org/indiekitai)