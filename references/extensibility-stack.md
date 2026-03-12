# The Claude Code Extensibility Stack

## Overview

Claude Code's power comes from layers of configuration that build on each other. Each layer serves a different purpose. Understanding when to use each one is the key skill.

## The Layers

### 1. CLAUDE.md — The Employee Manual

**What:** A markdown file in your project root that Claude reads at the start of every session.

**When it runs:** Always. Automatically. Every conversation.

**Use for:**
- Project context (what is this, what tech stack, how to build/test)
- Coding standards and conventions
- Things to avoid
- Project-specific patterns

**The analogy:** The employee manual every new hire reads on day one. The hammer will never go missing.

### 2. Skills — The Training Program

**What:** Reusable prompt templates that Claude can invoke when relevant.

**When it runs:** When Claude determines a skill matches the current task, or when triggered by a command.

**Use for:**
- Complex multi-step workflows (spec writing, code review, debugging)
- Standardized processes that should be consistent every time
- Domain expertise that applies across projects

**The analogy:** Specialized training courses. Not everyone needs every course, but when the situation calls for it, the knowledge is there.

### 3. Commands — The Shortcuts

**What:** `/slash` commands that users type to trigger specific actions.

**When it runs:** When the user types the command.

**Use for:**
- Common actions that users want on demand (`/commit`, `/test`, `/review`)
- Entry points into complex workflows
- Quick-access to frequently needed operations

**The analogy:** Speed-dial buttons on the workshop phone.

### 4. Hooks — The Safety Rules

**What:** Shell scripts that execute at specific lifecycle events (before/after tool calls, on stop).

**When it runs:** Always. Automatically. Cannot be skipped by Claude.

**Use for:**
- Enforcing rules that MUST always apply (linting, formatting)
- Preventing dangerous operations (blocking force-push, catching secrets)
- Logging and auditing

**The analogy:** Safety rules posted on the wall. Doesn't matter if you're a new hire or a 20-year veteran — you wear the safety glasses.

### 5. Subagents — The Specialists

**What:** Isolated Claude instances with their own context, spawned to handle specific subtasks.

**When it runs:** When Claude decides to delegate, or when configured in a plugin.

**Use for:**
- Parallel execution of independent tasks
- Isolating work that needs different context
- Preventing context window pollution

**The analogy:** Calling in a specialist. The electrician doesn't need to know about the plumbing.

### 6. Plugins — The Toolbox

**What:** Bundles of skills, commands, hooks, agents, and configuration that can be installed and shared.

**When it runs:** Mixed — depends on what's inside the plugin.

**Use for:**
- Packaging everything above into a shareable unit
- Distributing team workflows and standards
- Community-shared best practices

**The analogy:** The complete training kit for new hires — manual, courses, safety rules, and specialist contacts all in one box.

## Decision Framework

| I need to... | Use... |
|---|---|
| Give Claude project context | CLAUDE.md |
| Standardize a multi-step workflow | Skill |
| Let users trigger an action on demand | Command |
| Enforce something that MUST always happen | Hook |
| Run independent work in parallel | Subagent |
| Share my setup with others | Plugin |

## The Key Insight

> **Hooks are the only deterministic layer.** Everything else is probabilistic — Claude *might* use it, *might* follow it, *might* invoke it. Hooks ALWAYS fire. If something must happen every time, make it a hook.
