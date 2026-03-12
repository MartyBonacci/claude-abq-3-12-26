# Example CLAUDE.md

Save this as `CLAUDE.md` in your project root. Claude Code reads it automatically.

```markdown
# CLAUDE.md

## Project Overview
<!-- What is this project? One paragraph. -->
This is a [type of project] built with [tech stack]. It [what it does] for [who].

## Tech Stack
<!-- List your core technologies so Claude knows what tools are available -->
- **Frontend:** React 19, React Router v7, TypeScript
- **Styling:** Tailwind CSS v4
- **Backend:** Node.js, Express (or: "No backend — static site")
- **Database:** PostgreSQL with Drizzle ORM (or: "No database")
- **Testing:** Vitest, Playwright

## Development Commands
<!-- The commands Claude needs to build, test, and run your project -->
- `npm run dev` — start dev server
- `npm run build` — production build
- `npm test` — run unit tests
- `npm run lint` — check for lint errors

## Project Structure
<!-- Help Claude navigate your codebase -->
- `app/routes/` — page routes (file-based routing)
- `app/components/` — shared UI components
- `app/lib/` — utilities and helpers
- `app/db/` — database schema and queries

## Coding Standards
<!-- Your preferences — Claude will follow these -->
- Use functional components with hooks (no class components)
- Prefer named exports over default exports
- Use TypeScript strict mode — no `any` types
- Write tests for all new features

## Patterns to Follow
<!-- Show Claude how you do things in this project -->
- Data loading happens in route loaders, not useEffect
- Forms use progressive enhancement (no preventDefault)
- Error boundaries on every route

## Things to Avoid
<!-- Prevent common mistakes -->
- Do NOT use `useEffect` for data fetching
- Do NOT install new dependencies without asking
- Do NOT modify the database schema without discussing migration strategy
- Do NOT use inline styles — use Tailwind classes
```
