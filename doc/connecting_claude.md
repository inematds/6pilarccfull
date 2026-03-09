# 🌍 6) Connecting Claude

> MCPs = USB ports for Claude.
>
> Powerful. Expensive. Use strategically.

---

## 🔽 The Token Tax (Read This First)

Every active MCP consumes context — even if unused.

| MCPs Connected | Context Overhead |
| --- | --- |
| 0 | 0% |
| 1–2 | ~5–10% |
| 3–5 | ~15–25% |
| 10+ | 30%+ ⚠ |

### Rule of Thumb

Only keep active the MCPs you’re using **right now**.

Your context window is your oxygen.

---

### 🔹 Skills vs MCPs Decision Framework

| If you need… | Use |
| --- | --- |
| Repeatable workflow | Skill |
| Live external tool/API | MCP |
| Data formatting | Skill |
| Browsing / scraping | MCP |
| Token efficiency | Skill |

**Repetitive → Skill**

**Live data → MCP**

---

# 🔽 MCP #1 — Filesystem

**What it does:**

Access files outside current repo.

**Why it’s high-value:**

You will constantly need Desktop, config files, or cross-project access.

---

### Install

```bash
claude mcp add filesystem -- npx @anthropic-ai/mcp-filesystem /path/to/directory
```

Example:

```bash
claude mcp add filesystem -- npx @anthropic-ai/mcp-filesystem /Users/you/Desktop /Users/you/Documents
```

---

### Use Cases

- Reference files from another project
- Save outputs externally
- Access environment configs

**Token Impact:** Low

(Loads content only when requested)

---

# 🔽 MCP #2 — GitHub

**What it does:**

Full GitHub integration (issues, PRs, search, CI status).

**Why it’s worth it:**

You manage everything without leaving Claude.

---

### Install

```bash
claude mcp add github -- npx @anthropic-ai/mcp-github
```

Set token:

```bash
export GITHUB_TOKEN=your_token_here
```

---

### Use Cases

- Create/manage issues
- Review PRs
- Search across repos
- Read CI results

**Token Impact:** Moderate

(Keep queries specific)

---

# 🔽 MCP #3 — Browser (Chrome DevTools)

**What it does:**

Browse, screenshot, interact with web pages.

**Why it’s elite:**

Screenshot verification loop for UI perfection.

---

### Install

```bash
claude mcp add browser -- npx @anthropic-ai/mcp-browser
```

---

### Use Cases

- Screenshot + compare UI
- Scrape websites
- Interact with deployed apps
- Validate production builds

**Token Impact:** HIGH ⚠

Screenshots are expensive.

**Operator Rule:**

Disconnect when not doing UI work.

---

# 🔽 MCP #4 — Database (Postgres / Supabase)

**What it does:**

Run live queries, inspect schema, manage data.

---

### Install — PostgreSQL

```bash
claude mcp add postgres -- npx @anthropic-ai/mcp-postgres postgresql://user:pass@localhost:5432/dbname
```

### Install — Supabase

```bash
claude mcp add supabase -- npx @anthropic-ai/mcp-supabase --url https://your-project.supabase.co --key your-anon-key
```

---

### Use Cases

- Debug production data
- Verify migrations
- Explore schema relationships
- Seed test data

**Token Impact:** Moderate

Use `LIMIT` in queries.

**Safety Rule:**

Production = read-only credentials.

---

# 🔽 MCP #5 — Google Sheets

**What it does:**

Read/write spreadsheets directly.

---

### Install

```bash
claude mcp add google-sheets -- npx @anthropic-ai/mcp-google-sheets
```

Follow setup prompts for API credentials.

---

### Use Cases

- Export scraped data
- Update dashboards
- Process spreadsheet workflows
- CRM syncing

**Token Impact:** Low → Moderate

Query ranges, not entire sheets.

---

# 🔽 Essential vs Optional Setup

### Install Immediately

- Filesystem
- GitHub

### Install When Needed

- Browser
- Database
- Google Sheets

### Also Useful

- Notion
- Slack
- Linear
- Gmail
- Figma

---

# 🔽 Managing MCPs

### See active MCPs

```bash
claude mcp list
```

### Remove unused

```bash
claude mcp remove <name>
```

### Re-add later

```bash
claude mcp add <name> -- <command>
```

---

# 🔽 Active Rotation Strategy (This Is Key)

| Task | Keep Active |
| --- | --- |
| Building features | Filesystem + GitHub |
| UI/design | Filesystem + Browser |
| Backend/data | Filesystem + Database |
| Lead scraping | Browser + Sheets |
| Code review | GitHub only |

Don’t run all MCPs at once. Rotate intentionally.

---

# 🔽 Troubleshooting

| Problem | Fix |
| --- | --- |
| Not connecting | Check install command + credentials |
| Permission denied | Verify tokens |
| High token usage | Disconnect unused MCPs |
| Slow responses | External API speed issue |
| Server not found | `claude mcp list` |

---

# 🔽 The Operator Mindset

1. Install only what you need
2. Disconnect unused MCPs
3. Use Skills when possible
4. Monitor `/cost`
5. Rotate intentionally

Your context window = budget.

Every MCP = recurring subscription.

Spend like a CEO.
