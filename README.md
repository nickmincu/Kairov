# Kairov

AI-powered workflow automation that eliminates manual work.

## What is Kairov?

Kairov is an AI automation company that builds automated workflows for businesses to reduce manual workload and cut out time waste. We specialize in intake automation, document processing, approval orchestration, and system synchronization for workflow-heavy industries.

## Tech Stack

- **AI Development:** Claude Code with MCP ecosystem
- **Workflow Engine:** n8n (1,084+ automation nodes)
- **Testing:** Playwright (browser automation + visual regression)
- **Database:** PostgreSQL
- **Runtime:** Node.js 20+

## Getting Started

```bash
# Install dependencies
npm install

# Start dev server
npm run dev

# Run tests
npm test
```

## Project Structure

```
├── docs/                 # Operating system, client files, specs
│   ├── clients/          # Client-specific context (one file per client)
│   └── KAIROV_CLAUDE_OPERATING_SYSTEM_COMPACT.md
├── public/               # Static web assets
├── src/                  # Application source code
├── tests/                # Playwright test suites
├── .claude/              # Claude Code agents, skills, commands
├── CLAUDE.md             # Claude Code project instructions
└── playwright.config.ts  # Test configuration
```

## Development

All code changes must pass Playwright tests before committing. See `CLAUDE.md` for the full testing protocol.

## License

ISC
