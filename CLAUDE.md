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

## MCP Servers (Installed)
Use `claude mcp list` to verify. The following MCPs power the Kairov workflow stack:

### Core MCPs:
- **Playwright MCP** — Browser automation, page spinning, visual testing
- **GitHub MCP** — PR management, issue tracking, repo operations
- **n8n-MCP** — Workflow creation, 1084+ node access, template deployment
- **Firecrawl MCP** — Web scraping, data extraction for workflow inputs
- **Sequential Thinking** — Complex multi-step reasoning for workflow design

## Skills & Tools (Installed)
- **everything-claude-code** — 65 skills, 40+ commands, 16 agents, 20+ hooks
- **get-shit-done (GSD)** — Phase-based planning, parallel task execution, atomic commits
- **ruflo** — 60+ specialized agents, multi-agent swarms, self-learning orchestration

## Development Workflow
1. Plan with GSD phases (`/gsd:init` or `/gsd:plan`)
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
