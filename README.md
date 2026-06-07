# 🛠️ IndieKit

**Open-source developer tools with MCP support.** Focused on PostgreSQL tooling and developer workflow automation.

## Flagship: pg-dash

**AI-native PostgreSQL health checker** — 25 MCP tools, CI integration, migration safety checks, multi-env diff, bloat detection.

```bash
# One-shot health check
npx @indiekitai/pg-dash check postgres://user:pass@host/db

# Migration safety check (catches lock risks before production)
npx @indiekitai/pg-dash check-migration ./migrations/015_add_index.sql

# CI pipeline with GitHub Actions annotations
npx @indiekitai/pg-dash check $DATABASE_URL --ci --diff --format md
```

[![npm](https://img.shields.io/npm/v/@indiekitai/pg-dash)](https://www.npmjs.com/package/@indiekitai/pg-dash)  [![GitHub](https://img.shields.io/github/stars/indiekitai/pg-dash)](https://github.com/indiekitai/pg-dash)

**SQL safety by design** — read-only by default, strict write allowlist, no raw SQL passthrough. [Details →](https://github.com/indiekitai/pg-dash#security-sql-safety-by-design)

## Other Tools

| Package | Description | npm |
|---------|-------------|-----|
| [@indiekitai/pg-safe-migrate](https://github.com/indiekitai/pg-safe-migrate) | Catch unsafe migrations before production (JS/TS equivalent of strong_migrations) | [![npm](https://img.shields.io/npm/v/@indiekitai/pg-safe-migrate)](https://www.npmjs.com/package/@indiekitai/pg-safe-migrate) |
| [@indiekitai/throttled](https://github.com/indiekitai/throttled) | Rate limiting — 5 algorithms (Fixed Window, Sliding Window, Token Bucket, Leaky Bucket, GCRA) | [![npm](https://img.shields.io/npm/v/@indiekitai/throttled)](https://www.npmjs.com/package/@indiekitai/throttled) |
| [@indiekitai/env-audit](https://github.com/indiekitai/env-audit) | Scan codebases for env vars, generate .env.example | [![npm](https://img.shields.io/npm/v/@indiekitai/env-audit)](https://www.npmjs.com/package/@indiekitai/env-audit) |

## 🤖 MCP Integration

All tools ship with MCP server support. One config for AI agent integration:

```json
{
  "mcpServers": {
    "pg-dash": {
      "command": "npx",
      "args": ["-y", "-p", "@indiekitai/pg-dash", "pg-dash-mcp", "postgresql://user:pass@host/db"]
    }
  }
}
```

## 🌐 Links

- 🏠 [indiekit.ai](https://indiekit.ai)
- 📦 [npm org](https://www.npmjs.com/org/indiekitai)
