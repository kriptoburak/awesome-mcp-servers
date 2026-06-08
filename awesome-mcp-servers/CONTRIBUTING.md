# Contributing to Awesome MCP Servers

Thank you for helping make this list better! This guide explains how to submit new MCP servers, fix errors, or improve the documentation.

---

## Quick Rules

1. **It must work** — test the server yourself before submitting
2. **It must be maintained** — last commit within 6 months, or officially supported by the service
3. **One entry per PR** — keep PRs small and focused
4. **No spam** — commercial listings are welcome only if the server provides genuine value

---

## How to Add a Server

### Step 1: Fork this repository
Click the **Fork** button at the top right of this page.

### Step 2: Find the right category
Look through the README sections. If your server fits an existing category, add it there. If not, propose a new one.

### Step 3: Use the correct format

```markdown
- [Server Name](link) — One-sentence description of what the server does. `language` · 🔑 auth-needed
```

**Icons to use:**
| Icon | Meaning |
|------|---------|
| 🔑 | Requires API key or OAuth |
| 🆓 | Free tier available |
| ☁️ | Remote/hosted — no local install |
| 🏠 | Local only |
| ⚡ | Official server maintained by the service |

**Language badges:** Use `Python`, `TypeScript`, `Go`, `Rust`, or `Remote` (for hosted servers with no local code to run).

### Step 4: Add in alphabetical order (within a category)

### Step 5: Open a Pull Request
Use this title format: `Add: [Server Name] to [Category]`

In the PR description, briefly answer:
- What does this server do?
- Why should it be included in this list?
- Have you tested it yourself?

---

## What Gets Rejected

- Servers with no README or installation instructions
- Servers that haven't been updated in over 6 months (unless officially supported)
- Duplicate entries
- Entries that don't follow the format
- Servers with clear security issues (e.g., no auth on sensitive operations)

---

## Reporting Issues

Found a broken link, outdated entry, or incorrect info?

Open an [Issue](../../issues) with:
- The entry in question
- What's wrong
- A suggested fix (if you have one)

---

## Code of Conduct

Be respectful. We're all here to build something useful for the MCP community.
