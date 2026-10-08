# Current State

Updated: 2026-10-08

- The Playwright project is `/new_docker/e2e-test`; supporting test-case documents are in `/new_docker/e2e-test-report`. The test project directory is not itself a Git checkout.
- Functional tests use `playwright.config.ts` and `specs/new/`. The completed scope currently selects 20 combined business tests plus one preflight test; the pending scope selects one combined business test plus preflight. These are selectable-case counts, not a claim that the entire suite recently passed.
- Performance tests use `playwright.performance.config.ts` and currently contain four cases under `specs/performance/`: `P-02-001`, `P-02-002`, `P-02-003`, and `P-03-001`.
- AOCI is initialized in the test project. Its managed-scope policy excludes generated `reports/` content; the code index is still an unpopulated scaffold. The project-level `.codex/config.toml` registers its MCP server, but tool availability depends on the Codex chat's project root.
