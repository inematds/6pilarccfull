# 🎬 2) Claude Starter Pack

🧠 Make Claude 10x Smarter in 60 Seconds

> Drop this into your repo and Claude instantly understands your stack, rules, and conventions.
>
> No more re-explaining your project every session.

---

# What is `CLAUDE.md`?

`CLAUDE.md` is a **project memory file** that lives in your repository root.

Every time you start a Claude Code session, Claude reads this file first — giving it instant context about:

- Your tech stack
- Your coding conventions
- Your project structure
- Your rules

Think of it as **onboarding documentation for your AI coding partner**.

---

# 📂 Where To Place It

| Location | Scope |
| --- | --- |
| `project-root/CLAUDE.md` | Applies to the entire project |
| `project-root/src/CLAUDE.md` | Applies only when working in `/src` |
| `~/.claude/CLAUDE.md` | Applies to ALL projects (global memory) |

> 💡 **Pro Tip:** You can have multiple `CLAUDE.md` files.
>
> Claude reads all relevant ones depending on which directory you're working in.

---

# 📋 The Template

Copy everything below and customize it for your project:

```
# CLAUDE.md

## Project Overview
This is [PROJECT NAME], a [brief description of what it does].
Built with [primary tech stack].

## Tech Stack
- Language: [e.g., TypeScript, Python, Go]
- Framework: [e.g., Next.js, FastAPI, Express]
- Database: [e.g., PostgreSQL, MongoDB, Supabase]
- Styling: [e.g., Tailwind CSS, styled-components]
- Testing: [e.g., Jest, Pytest, Vitest]
- Package Manager: [e.g., npm, pnpm, bun, uv]

## Project Structure
- src/ — Main application source code
- src/components/ — Reusable UI components
- src/lib/ — Utility functions and shared logic
- src/api/ — API routes and handlers
- tests/ — Test files
- docs/ — Documentation

## Commands
- Dev server: npm run dev
- Build: npm run build
- Test: npm test
- Lint: npm run lint
- Type check: npx tsc --noEmit

## Code Conventions
- Use [functional components / class-based] approach
- Prefer [named exports / default exports]
- File naming: [kebab-case / camelCase / PascalCase]
- Use [single quotes / double quotes] for strings

## Important Patterns
- Error handling: [describe your approach]
- State management: [describe your approach]
- API calls: [describe your approach]
- Authentication: [describe your approach]

## Things To Avoid
- Never modify [specific files or directories]
- Don't use [deprecated patterns or libraries]
- Avoid [anything specific to your project]

## Additional Context
- [Links to relevant docs]
- [Known issues or quirks]
- [Deployment process notes]
```

---

# 🚀 Real-World Example: Next.js SaaS App

```
# CLAUDE.md

## Project Overview
SaaSify is a B2B subscription management platform.
Built with Next.js 14 (App Router), TypeScript, and Supabase.

## Tech Stack
- Language: TypeScript (strict mode)
- Framework: Next.js 14 with App Router
- Database: Supabase (PostgreSQL)
- Styling: Tailwind CSS + shadcn/ui
- Testing: Vitest + Playwright
- Package Manager: pnpm

## Commands
- Dev: pnpm dev
- Build: pnpm build
- Test: pnpm test
- E2E: pnpm test:e2e
- Lint: pnpm lint

## Code Conventions
- Use Server Components by default, Client Components only when needed
- Named exports for all components
- File naming: kebab-case for files, PascalCase for components
- Colocate tests next to source files as *.test.ts
- Use Zod for all input validation

## Things To Avoid
- Never use "any" type — use "unknown" and narrow
- Don't use the Pages Router — App Router only
- Never commit .env files
- Don't install new dependencies without discussing first
```

---

# 🐍 Real-World Example: Python API

```
# CLAUDE.md

## Project Overview
FastAPI backend for a real-time analytics dashboard.

## Tech Stack
- Language: Python 3.12
- Framework: FastAPI
- Database: PostgreSQL with SQLAlchemy
- Package Manager: uv

## Commands
- Dev: uv run uvicorn app.main:app --reload
- Test: uv run pytest
- Lint: uv run ruff check .
- Format: uv run ruff format .
- Migrate: uv run alembic upgrade head

## Code Conventions
- Type hints on all function signatures
- Pydantic models for all request/response schemas
- Dependency injection for database sessions
- Async handlers for all endpoints

## Things To Avoid
- Never use raw SQL — use SQLAlchemy ORM
- Don't use sync DB calls in async handlers
- Never expose internal IDs — use UUIDs
```

---

# 🏆 Tips for a Powerful `CLAUDE.md`

1. **Keep it concise**
   Claude reads this every session — don’t write a novel.

2. **Focus on what’s unique**
   Document *your* conventions, not general language features.

3. **Update it regularly**
   As your stack evolves, keep this current.

4. **Include commands**
   The most useful thing you can add is how to run, test, and build.

5. **Add “Things To Avoid”**
   Preventing mistakes is just as powerful as guiding behavior.

6. **Use directory-specific files**
   Add a `CLAUDE.md` to subdirectories that have special rules or constraints.
