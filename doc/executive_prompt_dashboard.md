# 🧑‍💻 4) Executive Prompt Dashboard

> Your daily-use prompt system.

---

# 🏆 Top 5 Prompts (Daily Drivers)

These handle 80% of real-world work.

---

## 🔹 1) 95% Confidence (Start Anything Properly)

```text
Ask me clarifying questions one at a time until you're 95% confident you can complete the task successfully.
```

**Use for:** Any new feature, migration, complex change

**Why:** Prevents blind-spot coding

---

## 🔹 2) Plan Mode Blueprint (Before Building)

```text
I want to add [feature].

Enter plan mode. Before writing any code:
1. Identify all files that need to change
2. Outline the approach step by step
3. Flag tradeoffs or risks
4. Wait for my approval
```

**Use for:** Non-trivial features

**Why:** Think first. Build second.

---

## 🔹 3) Structured Bug Report

```text
When I do [action], I get [error].

Expected behavior: [...]
Actual behavior: [...]

Here is the stack trace:
[paste]

Investigate the root cause before attempting a fix.
```

**Use for:** Any bug

**Why:** Forces diagnosis before patching

---

## 🔹 4) Brutal Audit

```text
I just built [X].

Audit this for:
1. Edge cases
2. Security vulnerabilities
3. Performance bottlenecks
4. Crash scenarios
5. Anything a senior engineer would flag

Be brutally honest.
```

**Use for:** After building anything meaningful

**Why:** Finds what you don’t know you missed

---

## 🔹 5) Teach Me What You Did

```text
I just watched you [do X].

Now teach me:
1. The root cause or core concept
2. Why this approach was chosen
3. What would break if we didn’t fix it
4. What to watch for next time

Explain it so I could do it myself.
```

**Use for:** After fixes / refactors

**Why:** Turns AI from tool -> skill amplifier

---

---

# 🧠 Collapsible Prompt Library (Full System)

---

## ▶ Getting Started

### 95% Confidence

```text
Ask me clarifying questions one at a time until you're 95% confident you can complete the task successfully.
```

### Project Kickoff

```text
I want to build [describe].

Before writing code:
1. Ask clarifying questions
2. Propose tech stack + explain why
3. Create milestone plan
4. Wait for approval
```

### Codebase Onboarding

```text
Read this codebase and give me:
1. High-level overview
2. Tech stack
3. Structure
4. Data flow
5. Conventions used
```

---

## ▶ Building Features

### Feature Blueprint

```text
I want to add [feature].

Enter plan mode:
1. Identify affected files
2. Outline approach
3. Flag risks
4. Wait for approval
```

### Build With Tests

```text
Build [feature].

For each piece:
1. Write test first
2. Write implementation
3. Run tests
4. Move to next piece

Do not batch tests.
```

---

## ▶ Debugging

### Structured Bug

```text
When I do [action], I get [error].

Expected:
Actual:

[stack trace]

Investigate root cause first.
```

### Log Analysis

```text
Here are logs:

[paste]

1. Identify distinct errors
2. Group related ones
3. Rank by severity
4. Trace root cause of critical ones
```

---

## ▶ Code Quality

### Code Review

```text
Review this branch for:
1. Bugs
2. Security
3. Performance
4. Readability
5. Missing error handling

Rate: Critical / Important / Minor / Nitpick
```

### Refactor Guardrails

```text
Refactor [file] to [goal].

Rules:
1. No behavior change
2. Run tests after each change
3. Stop if tests fail
4. Small incremental edits only
```

---

## ▶ Architecture

### Architecture Decision

```text
Compare [Option A] vs [Option B]:

1. Pros/Cons
2. Complexity
3. Scalability
4. Long-term maintenance
5. Recommendation
```

### API Design

```text
Design a REST API for [feature].

Include:
1. Endpoints
2. Schemas
3. Auth
4. Error format
5. Pagination/filtering
```

---

## ▶ Deployment

### Deployment Prep

```text
Prepare this project for deployment to [platform].

1. Check localhost configs
2. Validate env vars
3. Ensure build passes
4. Check security issues
5. Update deployment config
```

### CI/CD

```text
Set up CI/CD using [platform].

Pipeline must:
1. Run on PR
2. Lint + typecheck
3. Run tests
4. Build
5. Deploy on merge
```

---

# 🎯 Usage Strategy (Operator Level)

If you want maximum leverage:

1. Always start complex work with **95% Confidence**
2. Always build in **Plan Mode**
3. Always end major work with **Brutal Audit**
4. Always finish learning moments with **Teach Me**
5. Clear context before large migrations

That alone puts you ahead of 90% of Claude users.
