# 👾 3) 9 Claude Code Workflows

> Stop guessing what to type.
>
> These step-by-step workflows cover 90% of what you’ll do inside Claude Code.
>
> Battle-tested. Minimal friction. Maximum output.

---

# Workflow 1 — 🐞 Fix a Bug

**When to use:** Something’s broken and you want Claude to diagnose + fix it properly.

### Step 1 — Start with context

```text
claude "There's a bug where [describe the symptom]. It happens when [describe the trigger]."
```

### Step 2 — Force investigation first

```text
Read the relevant files and trace the logic before suggesting a fix.
```

### Step 3 — Review diagnosis

Confirm the root cause matches your understanding.

### Step 4 — Apply the fix

```text
Fix the bug and run the tests to make sure nothing else breaks.
```

### Step 5 — Commit

```text
/commit
```

**Pro Tips**

- Paste the full stack trace
- Point Claude to the suspected file
- Ask it to explain the root cause so you learn from it

---

# Workflow 2 — 🚀 Build a New Feature

**When to use:** Adding new functionality.

### Step 1 — Start in Plan Mode

```text
I want to add [feature]. Enter plan mode and design the approach before writing any code.
```

### Step 2 — Review the plan

Approve file changes, architecture, tradeoffs.

### Step 3 — Implement

Claude builds step-by-step.

### Step 4 — Test

```text
Run the tests and fix any failures.
```

### Step 5 — Polish

```text
Review what you just built. Is there anything we missed?
```

### Step 6 — Commit

```text
/commit
```

**Pro Tips**

- Break large features into smaller tasks
- Plan Mode prevents wasted tokens
- Write tests alongside the feature

---

# Workflow 3 — 🧼 Refactor Code

**When to use:** Improve structure without changing behavior.

### Step 1 — Understand current architecture

```text
claude "Read through [file/module] and explain the current architecture."
```

### Step 2 — Define the goal

```text
Refactor this to [goal]. Don't change any external behavior.
```

### Step 3 — Review the diff

Refactors touch a lot. Be careful.

### Step 4 — Run tests

```text
Run all tests to make sure nothing broke.
```

### Step 5 — Commit

```text
/commit
```

**Pro Tips**

- Have tests before refactoring
- Be specific about the goal
- Refactor in small commits

---

# Workflow 4 — 🧠 Understand a New Codebase

**When to use:** You just cloned a repo.

### Step 1 — Big picture

```text
claude "Explore this codebase and give me a high-level overview. What does it do? What's the tech stack? What's the structure?"
```

### Step 2 — Zoom in

```text
Walk me through how authentication works.
```

### Step 3 — Trace flow

```text
Trace what happens when a user submits the signup form.
```

### Step 4 — Create project memory

```text
/init
```

**Pro Tips**

- Start broad -> then narrow
- Ask “why” questions
- Use this when onboarding anywhere

---

# Workflow 5 — 🧪 Write Tests

**When to use:** Increasing test coverage.

### Step 1 — Identify gaps

```text
claude "Read [file/module] and identify what should be tested. Focus on edge cases."
```

### Step 2 — Generate tests

```text
Write comprehensive tests for [file/module].
```

### Step 3 — Verify

```text
Run the tests and make sure they pass.
```

### Step 4 — Coverage check

```text
Run tests with coverage and show me any gaps.
```

**Pro Tips**

- Define your test framework upfront
- Test behavior, not implementation
- Try TDD for new features

---

# Workflow 6 — 🔍 Code Review

**When to use:** Before pushing code.

### Step 1 — Ask for review

```text
claude "Review my current changes. Look for bugs, security issues, performance problems, and code quality."
```

### Or:

```text
/review
```

### Step 2 — Address feedback

Fix or justify.

### Step 3 — Re-review if needed

```text
Review the changes again after my fixes.
```

**Pro Tips**

- Focus review (security / performance)
- Use before every PR
- Ask: “What would a senior engineer flag?”

---

# Workflow 7 — 📦 Create a Pull Request

**When to use:** Changes are ready.

### Step 1

```text
/pr
```

Claude will:

- Analyze commits
- Generate title + description
- Create PR on GitHub

### Step 2 — Review description

Adjust if needed.

**Pro Tips**

- Commit everything first
- Clear commit messages = better PR descriptions

---

# Workflow 8 — 🪵 Debug With Logs or Errors

**When to use:** You have logs or stack traces.

### Option A — Paste error

```text
claude "I'm getting this error: [paste stack trace]. Help me fix it."
```

### Option B — Pipe it

```bash
cat error.log | claude -p "What's causing these errors and how do I fix them?"
```

### Step 3 — Trace root cause

Claude reads relevant files.

### Step 4 — Apply fix

```text
Fix it and verify the error is resolved.
```

**Pro Tips**

- Include full stack trace
- Describe what triggered it
- Mention if it’s intermittent

---

# Workflow 9 — 🏗 Multi-File Refactor / Migration

**When to use:** Large-scale changes across many files.

### Step 1 — Plan Mode

```text
claude "I need to [migrate/update/rename] [X] across the entire codebase. Enter plan mode."
```

### Step 2 — Review scope

Claude identifies all affected files.

### Step 3 — Execute in batches

```text
Start with the core module, then move to dependent modules.
```

### Step 4 — Test after each batch

```text
Run tests after each batch.
```

### Step 5 — Final sweep

```text
Do a final sweep — are there any files we missed?
```

**Pro Tips**

- Never do everything in one shot
- Keep tests green at all times
- Use `/compact` during long migrations

---

# 🎯 Quick Reference
