# Kairov - AI Automation Platform

## Project Overview
Kairov is an AI automation company that creates automated workflows for companies to reduce manual workload and eliminate time waste. The platform leverages Claude Code's MCP ecosystem, skills, and agent orchestration to build, test, and deploy workflow automations.

## Automated Testing Protocol (MANDATORY)
**Every code change MUST be followed by running tests.** No functionality should be lost as we progress.

### Before ANY commit:
1. Run `npm test` to execute all Playwright tests
2. If tests fail, fix the regression before committing
3. Add new tests for any new feature or page added

### Test Structure:
- `tests/smoke.spec.ts` — Homepage and basic navigation smoke tests
- `tests/` — All Playwright test files live here
- Run `npm run test:headed` for visual debugging
- Run `npm run test:report` to view HTML test reports

### When adding new pages/features:
1. Create the feature
2. Write a corresponding test in `tests/`
3. Run full test suite
4. Only commit if all tests pass

## Tech Stack
- **Runtime**: Node.js 20+
- **Testing**: Playwright (Chromium)
- **Web Server**: localhost:3333
- **Version Control**: GitHub (nickmincu/Kairov)

## MCP Servers Installed (6 connected)
Use `claude mcp list` to verify.

### Connected:
- **Playwright** (`@playwright/mcp`) — Browser automation, page spinning, visual testing, 25+ tools
- **GitHub** (`@modelcontextprotocol/server-github`) — PR management, issue tracking, repo operations
- **n8n-MCP** (`n8n-mcp`) — Workflow creation, 1084+ nodes, 2709 templates, 20 tools
- **Sequential Thinking** (`@modelcontextprotocol/server-sequential-thinking`) — Step-by-step reasoning
- **Context7** (`@upstash/context7-mcp`) — Up-to-date framework/library documentation
- **PostgreSQL** (`@modelcontextprotocol/server-postgres`) — Direct database access

### Pending Setup:
- **Supabase** — Needs `npx supabase login` first
- **Firecrawl** — Deferred until API key obtained (~$0.004/page)
- **Composio** — 850+ SaaS integrations, deferred until needed
- **BrowserMCP** — Real browser profile automation, deferred

## Skills & Frameworks Installed

### everything-claude-code (ECC) — 82 skills, 43 commands, 14 rules
Source: affaan-m/everything-claude-code (72K stars)

### get-shit-done (GSD) — 32 commands
Source: gsd-build/get-shit-done (28K stars)

### ruflo — 30 skills, 99 agents, 10 commands
Source: ruvnet/ruflo (20K stars)

## Development Workflow
1. Plan with GSD phases (`/gsd:new-project` or `/gsd:plan-phase`)
2. Execute with parallel agents
3. Test with Playwright (`npm test`)
4. Commit wins to GitHub
5. Deploy workflows via n8n-MCP

## Code Style
- Keep files small and focused
- Prefer TypeScript for new code
- Use descriptive variable names
- No console.log in production code — use proper logging

## Git Conventions
- Branch per feature: `feature/<name>`
- Commit messages: `type: description` (feat, fix, test, docs, refactor)
- Always run tests before pushing
