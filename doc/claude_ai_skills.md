# 💙 5) Claude AI Skills

Build once. Call forever.

Save tokens. Save time. Scale leverage.

## 🔽 What Are Skills?

**Skills = reusable markdown workflows that Claude can call on demand.**

In **Claude Code**, they live in `.claude/commands/` as markdown files. In **Cowork** (the desktop app), they show up as `/slash commands` — built-in ones like `/pdf`, `/docx`, `/pptx`, `/xlsx`, and `/visuals` come pre-loaded, and you can install more via **plugins**.

Instead of re-typing long prompts:

- You write it once
- Save as a markdown file (Code) or install a plugin (Cowork)
- Call it anytime with a slash command or by referencing it naturally

Think: **SOPs for your AI.**

---

### 🔹 Skills vs MCPs vs Plugins

|  | Skills | MCP Servers | Plugins |
| --- | --- | --- | --- |
| What they are | Reusable prompt workflows | Live tool integrations | Bundles of skills + MCPs + tools |
| Token cost | Near zero until called | ~20% context just connected | Varies — loaded on demand |
| Best for | Repetitive workflows | Live external access | Full workflow packages |
| Works in | Claude Code + Cowork | Claude Code + Cowork | Claude Code + Cowork |
| Rule | Repetitive → Skill | Live data → MCP | Full workflow → Plugin |

---

## 🔽 Where Skills Live

**Claude Code:**

```text
project-root/
  .claude/
    commands/
      screenshot-to-website.md
      lead-research.md
      code-review.md
```

Claude auto-discovers them. Call them with slash commands like `/screenshot-to-website` or just reference them naturally in conversation.

**Cowork (Desktop App):**

Skills come pre-installed or via plugins. Built-in skills include:

- `/pdf` — Create, merge, split, fill, and extract PDFs
- `/docx` — Create and edit Word documents
- `/pptx` — Create and edit presentations
- `/xlsx` — Create and edit spreadsheets
- `/visuals` — Create branded infographics and social content
- `/schedule` — Create scheduled tasks that run automatically
- `/skill-creator` — Build and test new skills

You can also install **plugins** that add new skills, MCPs, and tools all at once.

---

## 🔽 🔥 NEW: Plugins (The Game-Changer)

Plugins are the biggest upgrade to the skills ecosystem. They bundle skills, MCP servers, and tools into one installable package.

### Why Plugins Matter

- **One install, everything works** — no manual config
- **Work in both Claude Code and Cowork** — install once, use everywhere
- **Community-built and growing fast** — new ones dropping constantly

### 🔹 Supabase Plugin (Highly Recommended)

If you're building anything with a database, the **Supabase MCP plugin** is a must-install. It gives Claude direct access to:

- Query and manage your Supabase database
- Create and modify tables
- Run SQL queries
- Manage authentication and storage
- Build full-stack apps with real backend power

This means you can say things like "create a users table with email and role columns" or "show me all orders from the last 7 days" and Claude just does it — no copy-pasting SQL, no switching tabs.

**How to install:** Search for Supabase in the plugin marketplace within Claude Code or Cowork and connect it to your project.

---

# 🔽 🔎 Best Places to Get Skills (Don't Build From Scratch)

## Curated Lists

- **awesome-claude-code** → https://github.com/hesreallyhim/awesome-claude-code
- **awesome-agent-skills** → https://github.com/VoltAgent/awesome-agent-skills
- **awesome-claude-skills** → https://github.com/travisvn/awesome-claude-skills

## Frameworks (Install & Go)

- **Anthropic Official Skills** — Gold standard. Built into Cowork (pdf, docx, pptx, xlsx, visuals)
- **Superpowers by obra** — TDD, debugging, planning, auto-triggers
- **everything-claude-code** — Hackathon mega pack

## Plugin Marketplace

Plugins are now the fastest way to extend Claude. Browse and install directly from within Claude Code or Cowork. Key categories include productivity, database (like Supabase), design, and developer tools.

## Marketplaces

- [**SkillsMP.com**](http://SkillsMP.com) — 270k+ aggregated skills
- [**SkillHub.club**](http://SkillHub.club) — AI-rated skills with playground
- [**awesomeclaude.ai**](http://awesomeclaude.ai) — Visual browsing
- [**mcpservers.org**](http://mcpservers.org) — Category-based skills

---

## ⚠ Security Warning (Critical)

Skill files and plugins have:

- Filesystem access
- Shell access
- Environment access

Before installing:

- Read raw markdown
- Look for hidden instructions
- Verify it does exactly what it claims
- For plugins: check the source and reviews before installing

---

# 🔽 Skill Template (Copy This)

```markdown
# Skill: [Name]

## Purpose
[One sentence describing the outcome]

## Inputs Required
- [User provides this]
- [Files / URLs / Context]

## Steps

### Step 1: [Action]
[Specific instruction]

### Step 2: [Action]
[Specific instruction]

### Step 3: [Action]
[Specific instruction]

## Quality Checks
- [ ] [Verification step]
- [ ] [Verification step]

## Output
[Clear description of expected final output]
```

---

# 🔽 Skill Example 1 — Screenshot to Website

## Purpose

Convert a design screenshot into a pixel-accurate responsive web page.

### Core System

1. Analyze layout (grid, spacing, color hex, typography)
2. Plan semantic HTML structure
3. Build using Tailwind
4. Screenshot comparison loop
5. Iterate until 95%+ match

### Quality Checklist

- [ ]  Layout matches
- [ ]  Exact color hex values
- [ ]  Typography accurate
- [ ]  Responsive across breakpoints
- [ ]  Hover + focus states included
- [ ]  No console errors

### Output

Production-ready HTML or component files.

---

# 🔽 Skill Example 2 — Lead Research

## Purpose

Research and structure business leads into spreadsheet-ready format.

### Core System

1. Confirm niche + location + data points
2. Research each lead
3. Classify (Hot / Warm / Cold)
4. Remove duplicates
5. Format as CSV or table

### Quality Checklist

- [ ]  All requested fields filled
- [ ]  No duplicates
- [ ]  URLs validated
- [ ]  Classification accurate
- [ ]  Test batch verified before scaling

### Output

Spreadsheet-ready table.

---

# 🔽 Skill Example 3 — Senior Code Review

## Purpose

Perform a pull-request level review with severity ratings.

### Review Layers

**Security**

- SQL injection
- XSS
- Exposed keys
- Auth gaps

**Bugs**

- Null references
- Race conditions
- Unhandled promises
- Type mismatches

**Performance**

- N+1 queries
- Memory leaks
- Missing DB indexes
- Large bundle imports

**Quality**

- Naming clarity
- DRY violations
- Functions > 50 lines
- Pattern consistency

### Output Format

**Critical**

- [file + line + issue + fix]

**Important**

- [...]

**Minor**

- [...]

**Positive**

- Call out good decisions

---

# 🔽 Claude Code ↔ Cowork: Syncing Skills

One of the most common questions: **"I have skills in Code but can't see them in Cowork — how do I sync them?"**

### Option 1: Select Your Skills Folder (Quickest)

In Cowork, select the folder where your Claude Code skills live (usually `~/.claude/commands/`). Claude can then read and follow them — they just won't appear as slash commands.

### Option 2: Package as a Plugin (Best Long-Term)

Use the `/skill-creator` or `/create-cowork-plugin` skill in Cowork to bundle your Code skills into a `.plugin` file. Install it once, and your skills show up natively with slash commands every time.

### Option 3: Rebuild in Cowork

For simple skills, just ask Claude in Cowork to create the skill for you. It takes seconds and the skill will be formatted correctly for the Cowork environment.

---

# 🔽 Writing Great Skills (Operator Rules)

1. Be specific — vague steps = vague output
2. Include checklists — self-verification is leverage
3. Start with 25 → then scale
4. Add WHY behind steps
5. Version your skills
6. Share in repo

---

# 🔽 Token Math (Why This Matters)

| Approach | Tokens Per Use | 100 Uses |
| --- | --- | --- |
| Re-typing prompt | ~500 | ~50,000 |
| Skill invocation | ~50 | ~5,000 |

**≈ 90% savings**

Over months, this compounds massively.

---

You're basically building an internal AI OS now. Skills are your SOPs, MCPs are your integrations, and Plugins tie it all together. Let's do it properly.
