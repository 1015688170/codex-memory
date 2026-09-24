# Current State

Updated: 2026-09-24

- The Playwright project is `/new_docker/e2e-test`; supporting test-case documents are in `/new_docker/e2e-test-report`. The test project directory is not itself a Git checkout.
- Functional tests use `playwright.config.ts` and `specs/new/`. `config/case-status.ts` currently registers 13 completed combined cases and one pending combined case. These are registry states, not a claim that the latest run passed.
- Performance tests use `playwright.performance.config.ts` and currently contain `P-02-001` and `P-02-002` under `specs/performance/`.
- AOCI is initialized in the test project. Its managed-scope policy is aligned and excludes generated `reports/` content. The current scope stage is `authoring_required`, with zero authored index entries.
- The project-level `.codex/config.toml` registers the AOCI MCP server. A newly opened Codex chat rooted at `/new_docker/e2e-test` reported AOCI tools in its tool list, but no AOCI MCP call had been made at the end of this conversation; service operation is not yet verified.
