# Kairov

@docs/KAIROV_CLAUDE_OPERATING_SYSTEM_COMPACT.md
@package.json
@README.md

## Automated Testing Protocol (MANDATORY)

**Every code change MUST be followed by running tests.** No functionality should be lost as we progress.

Before ANY commit:
1. Run `npm test` to execute all Playwright tests
2. If tests fail, fix the regression before committing
3. Add new tests for any new feature or page added

When adding new pages/features:
1. Create the feature
2. Write a corresponding test in `tests/`
3. Run full test suite — only commit if all tests pass

Test commands:
- `npm test` — run all tests
- `npm run test:headed` — visual debugging
- `npm run test:report` — view HTML reports

## Dev Server

Port 3333 (`npm run dev`). Playwright config and server.js both default to this port.

## Git Conventions

- Branch per feature: `feature/<name>`
- Commit messages: `type: description` (feat, fix, test, docs, refactor)
- Always run tests before pushing

## Client Work

Client-specific context lives in `docs/clients/`. Load the relevant client file when scoping or building workflows for a specific client.

Current clients:
- `docs/clients/ag-risk-managers.md` — AG Risk Managers (insurance/agri-insurance)
