# Getting Started with Claude Code

## 1. Install Claude Code

```bash
npm install -g @anthropic-ai/claude-code
```

Requires Node.js 18+. If you don't have Node.js: https://nodejs.org

## 2. Authenticate

```bash
claude
```

The first time you run it, Claude Code will walk you through authentication. You'll need an Anthropic account with API access or a Claude Max/Team/Enterprise subscription.

## 3. Your First Session

Navigate to any project directory and launch Claude Code:

```bash
cd your-project
claude
```

Try something simple:

```
> Explain this project to me
> What does the main entry point do?
> Add a .gitignore if there isn't one
```

## 4. Create Your First CLAUDE.md

In your project root, create a `CLAUDE.md` file. This is the "employee manual" — Claude reads it automatically at the start of every session.

```bash
claude "Create a CLAUDE.md for this project"
```

Or create one manually. See `example-claude-md.md` in this folder for a template.

## 5. Learn the Keyboard Shortcuts

- **Enter** — send message
- **Escape** — cancel current generation
- **/** — browse available commands
- **S** (in browser presentation) — open speaker notes

## 6. Next Steps

- Read the extensibility stack: `extensibility-stack.md`
- Browse the example CLAUDE.md: `example-claude-md.md`
- Try installing a plugin: `claude plugin install specswarm`
- Join the community: https://claudeabq.dev

## Official Documentation

https://docs.anthropic.com/en/docs/claude-code/getting-started
