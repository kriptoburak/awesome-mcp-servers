# 🤖 Awesome MCP Servers

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![License: CC0](https://img.shields.io/badge/License-CC0-lightgrey.svg)](LICENSE)
[![Last Updated](https://img.shields.io/badge/Updated-June%202026-blue.svg)]()

> A curated list of **Model Context Protocol (MCP) servers** — the open standard that gives AI assistants real tools, real data, and real superpowers.

MCP was created by Anthropic in November 2024 and adopted by OpenAI, Google DeepMind, and Microsoft in early 2025. In December 2025, it was donated to the **Linux Foundation's Agentic AI Foundation (AAIF)**, making it a true open standard.

---

## 📖 Contents

- [What is MCP?](#what-is-mcp)
- [How to Use This List](#how-to-use-this-list)
- [🚀 Starter Kit](#-starter-kit-install-these-first)
- [🧑‍💻 Developer Tools](#-developer-tools)
- [🗄️ Databases](#️-databases)
- [🌐 Web & Browser](#-web--browser)
- [📂 File Systems & Storage](#-file-systems--storage)
- [💬 Communication](#-communication)
- [📊 Data & Analytics](#-data--analytics)
- [🤖 AI & Memory](#-ai--memory)
- [☁️ Cloud & DevOps](#️-cloud--devops)
- [🔒 Security](#-security)
- [📝 Productivity & Knowledge](#-productivity--knowledge)
- [🗺️ Maps & Location](#️-maps--location)
- [📚 Learning Resources](#-learning-resources)
- [🤝 Contributing](#-contributing)

---

## What is MCP?

**Model Context Protocol (MCP)** is an open standard that lets AI assistants (Claude, Cursor, Windsurf, VS Code Copilot, etc.) connect to external tools, databases, and services in a standardized way.

Think of it like a USB-C port for AI — one protocol, plug in any tool.

```
Your AI Assistant ←→ MCP Client ←→ MCP Server ←→ Real World Tool
```

**Without MCP:** Your AI can read/write files and run terminal commands. That's it.  
**With MCP:** Your AI can query databases, search the web, control browsers, post to Slack, manage GitHub issues, and thousands more things.

### Two types of MCP servers:
- **Local (stdio)** — Runs on your machine, installed via `npx` or `pip`. Fast, private.
- **Remote (HTTP)** — Hosted by the service provider. Zero local setup, just auth.

---

## How to Use This List

Each entry follows this format:

```
- [Server Name](link) — What it does. `language` · ⭐ stars · 🔑 auth-needed
```

**Icons:**
- 🔑 Requires API key or OAuth
- 🆓 Free tier available
- ☁️ Remote/hosted (no local install)
- 🏠 Local only
- ⚡ Official / maintained by the service itself

---

## 🚀 Starter Kit (Install These First)

The three servers that cover 80% of developer workflows. Start here.

| Server | What it does | Install |
|--------|-------------|---------|
| [GitHub MCP](https://github.com/github/github-mcp-server) | Read/write repos, issues, PRs | `npx @modelcontextprotocol/server-github` |
| [Context7](https://github.com/upstash/context7) | Up-to-date library docs in context | `npx @upstash/context7-mcp` |
| [Playwright](https://github.com/microsoft/playwright-mcp) | Browser control & web scraping | `npx @playwright/mcp` |

---

## 🧑‍💻 Developer Tools

For coding, version control, CI/CD, and project management.

- [GitHub MCP](https://github.com/github/github-mcp-server) ⚡ — Search code, manage issues, review PRs, clone repos. The most essential dev MCP. `TypeScript` · 🔑 GitHub token
- [GitLab MCP](https://gitlab.com/gitlab-org/modelcontextprotocol) ⚡ — Full GitLab API access: MRs, pipelines, issues, wikis. `TypeScript` · 🔑 GitLab token
- [Context7](https://github.com/upstash/context7) — Pulls live, version-accurate library docs so your AI never hallucinates an API. `TypeScript` · 🆓 Free
- [Linear MCP](https://github.com/linear/linear-mcp) ⚡ — Create and manage Linear issues, cycles, and projects from AI chat. `TypeScript` · 🔑 Linear API key
- [Jira MCP](https://github.com/sooperset/mcp-atlassian) — Read/write Jira tickets and Confluence pages. `Python` · 🔑 Atlassian token
- [Sentry MCP](https://docs.sentry.io/platforms/mcp/) ⚡ ☁️ — Query Sentry errors, stack traces, and release health. `Remote` · 🔑 Sentry token
- [Docker MCP](https://github.com/docker/mcp-servers) ⚡ — Manage containers, images, and compose stacks. `TypeScript` · 🏠 Local

---

## 🗄️ Databases

Query and manage databases with natural language.

- [PostgreSQL MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/postgres) — Read-only Postgres queries with schema introspection. Official reference implementation. `TypeScript`
- [SQLite MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/sqlite) — Full read/write SQLite access. Great for local prototyping. `TypeScript`
- [Supabase MCP](https://supabase.com/docs/guides/getting-started/mcp) ⚡ ☁️ — Query Supabase Postgres, manage auth, storage, and edge functions. `Remote` · 🔑 Supabase token
- [MySQL MCP](https://github.com/benborla/mcp-server-mysql) — Connect to MySQL databases for read/write operations. `TypeScript` · 🔑 DB credentials
- [MongoDB MCP](https://github.com/kiliczsh/mcp-mongo-server) — Query and manage MongoDB collections. `TypeScript` · 🔑 Connection string
- [Redis MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/redis) — Read and write Redis keys, lists, sets, hashes. `TypeScript`

---

## 🌐 Web & Browser

Fetch, scrape, and interact with the web.

- [Playwright MCP](https://github.com/microsoft/playwright-mcp) ⚡ — Full browser automation: click, fill forms, take screenshots, scrape. `TypeScript` · 🏠 Local
- [Fetch MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch) — Simple web content fetching and HTML-to-markdown conversion. Official reference. `Python`
- [Firecrawl MCP](https://github.com/mendableai/firecrawl-mcp) — Scrape and crawl entire websites, extract structured data. `TypeScript` · 🔑 Firecrawl API key · 🆓 Free tier
- [Bright Data MCP](https://github.com/luminati-io/brightdata-mcp) ☁️ — Reliable real-time web data at scale. 5,000 free requests/month. `Remote` · 🔑 API key · 🆓
- [Puppeteer MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/puppeteer) — Browser control via Puppeteer. Official reference implementation. `TypeScript`

---

## 📂 File Systems & Storage

Access and manage files, local and cloud.

- [Filesystem MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) — Read/write local files within a sandboxed directory. Official reference. `TypeScript`
- [Google Drive MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/gdrive) — Search, read, and list Google Drive files. Official reference. `TypeScript` · 🔑 Google OAuth
- [Dropbox MCP](https://github.com/smadikanti/mcp-dropbox-server) — Upload, download, list Dropbox files. `TypeScript` · 🔑 Dropbox token
- [AWS S3 MCP](https://github.com/aws-samples/amazon-s3-mcp) — List buckets, upload and download S3 objects. `Python` · 🔑 AWS credentials

---

## 💬 Communication

Slack, email, and messaging integrations.

- [Slack MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/slack) — Read channel history, search messages, post to channels. Respects workspace permissions. Official reference. `TypeScript` · 🔑 Slack token
- [Gmail MCP](https://github.com/GongRzhe/Gmail-MCP-Server) — Search, read, draft, and send Gmail emails. `Python` · 🔑 Google OAuth
- [Telegram MCP](https://github.com/kfastov/mcp-telegram) — Send messages and read chats from Telegram. `Python` · 🔑 Bot token
- [Discord MCP](https://github.com/v-3/discordmcp) — Read/write Discord channels, manage server info. `TypeScript` · 🔑 Bot token

---

## 📊 Data & Analytics

Financial data, search APIs, and analytics platforms.

- [Alpha Vantage MCP](https://github.com/calvernaz/alphavantage) — Real-time and historical stock, ETF, forex, crypto, and fundamental data. `Python` · 🔑 API key · 🆓 Free tier
- [Google Analytics MCP](https://github.com/jasonkneen/mcp-analytics) — Query GA4 reports and events with natural language. `TypeScript` · 🔑 Google OAuth
- [Brave Search MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search) — Web and local search via Brave Search API. Official reference. `TypeScript` · 🔑 Brave API key · 🆓 Free tier
- [Google Maps MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/google-maps) — Geocoding, directions, place search. Official reference. `TypeScript` · 🔑 Maps API key

---

## 🤖 AI & Memory

Persistent memory, RAG, and AI tooling integrations.

- [Memory MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/memory) — Gives AI persistent key-value memory across conversations. Official reference. `TypeScript`
- [Obsidian MCP](https://github.com/MarkusPfundstein/mcp-obsidian) — Read/write Obsidian vault notes, traverse backlinks. `Python` · 🏠 Local
- [Notion MCP](https://github.com/makenotion/notion-mcp-server) ⚡ — Create, search, and update Notion pages and databases. `TypeScript` · 🔑 Notion API key

---

## ☁️ Cloud & DevOps

AWS, Cloudflare, and infrastructure tools.

- [Cloudflare MCP](https://github.com/cloudflare/mcp-server-cloudflare) ⚡ ☁️ — Manage Workers, KV, R2, D1, and DNS from your AI. `Remote` · 🔑 Cloudflare token
- [AWS MCP](https://github.com/awslabs/mcp) ⚡ — Suite of AWS service MCPs: S3, DynamoDB, Lambda, CloudFormation. `Python` · 🔑 AWS credentials
- [Kubernetes MCP](https://github.com/strowk/mcp-k8s-go) — Query pods, deployments, services, and logs from kubectl context. `Go` · 🏠 Local

---

## 🔒 Security

- [Semgrep MCP](https://github.com/semgrep/mcp) ⚡ — Run static analysis scans on code using Semgrep rules. `Python` · 🔑 API key
- [Shodan MCP](https://github.com/BurtTheCoder/mcp-shodan) — Query Shodan for internet-exposed hosts and CVEs. `TypeScript` · 🔑 Shodan API key

> ⚠️ **Security note:** Per BlueRock Security research, 36.7% of public MCP servers carry SSRF vulnerabilities and 41% have no authentication. Only install servers you trust. Review what each server can access before giving it write permissions.

---

## 📝 Productivity & Knowledge

- [Google Calendar MCP](https://github.com/nspady/google-calendar-mcp) — Read events, create meetings, check availability. `TypeScript` · 🔑 Google OAuth
- [Todoist MCP](https://github.com/Doist/todoist-mcp) ⚡ — Manage tasks, projects, and labels in Todoist. `TypeScript` · 🔑 Todoist token
- [Airtable MCP](https://github.com/rashidazarang/airtable-mcp) — Query and update Airtable bases and records. `TypeScript` · 🔑 Airtable token

---

## 🗺️ Maps & Location

- [Google Maps MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/google-maps) — Directions, geocoding, place search. Official reference. `TypeScript` · 🔑 Maps API key
- [OpenStreetMap MCP](https://github.com/leynier/mcp-osm) — Free geocoding and map data via OpenStreetMap Nominatim. `Python` · 🆓 No key needed

---

## 📚 Learning Resources

### Official
- [MCP Specification](https://spec.modelcontextprotocol.io) — The full protocol spec
- [MCP Quickstart](https://modelcontextprotocol.io/quickstart) — Build your first MCP server in 15 minutes
- [Official MCP Examples](https://github.com/modelcontextprotocol/servers) — Reference implementations in Python & TypeScript
- [MCP Inspector](https://github.com/modelcontextprotocol/inspector) — Debug and test your MCP servers locally

### Directories (find even more MCPs)
- [Glama.ai](https://glama.ai/mcp) — 22,000+ indexed MCP servers with quality scores
- [MCPServers.org](https://mcpservers.org) — Community-curated directory
- [mcp-awesome.com](https://mcp-awesome.com) — 1,200+ quality-verified servers

### SDKs (to build your own MCPs)
- [Python SDK](https://github.com/modelcontextprotocol/python-sdk) — Official Python SDK (`pip install mcp`)
- [TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk) — Official TypeScript SDK (`npm install @modelcontextprotocol/sdk`)

### Key facts to know
- MCP was created by Anthropic (Nov 2024), now governed by Linux Foundation AAIF (Dec 2025)
- Every connected MCP server injects ~2,000–5,000 tokens of schema into your context — connect only what you need
- Remote MCP servers (HTTP/Streamable HTTP) are the fastest-growing category — zero install, just auth
- Anthropic archived 13 of its 20 original reference servers in 2025; always check if a server is actively maintained before installing

---

## 🤝 Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a PR.

**Criteria for inclusion:**
- ✅ The server must be functional and publicly accessible
- ✅ Must have a README with installation instructions
- ✅ Must be maintained (last commit within 6 months, or officially supported)
- ✅ No purely commercial spam listings

**To add a server:** Fork → add your entry in the right category → open a PR with a brief description of what it does and why it belongs.

---

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)

This list is released under CC0 — do whatever you want with it.

---

*Maintained by the community. Star ⭐ the repo if you find it useful!*
