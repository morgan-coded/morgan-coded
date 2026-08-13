# Morgan Carr

TypeScript/Node engineer working on AI infrastructure, SDKs, parsers, and static analysis.
Below are five upstream contributions I can explain end to end, followed by original projects with setup instructions, tests, and documented limitations.

## Selected upstream work

| Problem | Contribution | Outcome |
|---|---|---|
| [txtai #1164](https://github.com/neuml/txtai/pull/1164) needed a fixed-dimensional LEMUR path; its training path then needed to move out of pooling in [#1172](https://github.com/neuml/txtai/pull/1172). | Added the encoder and trainer, measured matched-size exact retrieval, then moved training and validation selection into `LemurTrainer` with progress reporting. | Both changes merged. At the matched 2,048-dimensional budget, LEMUR-MLP lifted NDCG@10 by 49.4–61.9% across the three datasets; the trainer move kept config and all seven tensors byte-identical under a fixed seed. |
| [openai-node #2021](https://github.com/openai/openai-node/pull/2021) could lose server error metadata before `response.created`, while delayed async iteration could finish without rejecting. | Converted error frames before accumulation and generic event emission, then reused `EventStream.events()` failure retention for iteration. | `HAYDEN-OAI` added final test polish and merged the change into the official SDK. |
| [meriyah #612](https://github.com/meriyah/meriyah/pull/612) routed decorators through general member/call parsing, accepting forms outside the decorator grammar and producing incorrect computed-field shapes. | Implemented the decorator grammar directly and added fail cases, AST-shape assertions, and controls for valid forms. | The fix merged. The maintainers then invited me as a collaborator and asked that changes continue through PRs, including small fixes. |
| [kysely #1919](https://github.com/kysely-org/kysely/pull/1919) could release migration locks too early when migrations ran without a surrounding transaction. | Implemented PostgreSQL session-level locking and serialization with a real concurrent-migrator regression. | The maintainer added the acquisition timeout and MSSQL session-lock path, fixed the flaky test, and merged the result. |
| OpenLIT's trace-analysis dimensions were wired across separate paths, making focused extensions touch several surfaces. | Added the registry foundation in [#1354](https://github.com/openlit/openlit/pull/1354), then extended it with prompt-injection observability in [#1376](https://github.com/openlit/openlit/pull/1376) and tool-misuse evidence in [#1394](https://github.com/openlit/openlit/pull/1394). | Maintainers approved and merged each stage, preserving one registry path for later dimensions. |

## Own projects

- **[ast-lens-mcp](https://github.com/morgan-coded/ast-lens-mcp)** — a TypeScript MCP server exposing read-only tools for structural code queries, with syntactic limits documented explicitly.
- **[agent-bisect](https://github.com/morgan-coded/agent-bisect)** — a deterministic CLI for locating the first visible breaking step in an agent run and abstaining when the evidence is insufficient.
- **[script-sentinel](https://github.com/morgan-coded/script-sentinel)** — a read-only Shopify Plus migration-risk app with the workflow, architecture, and product boundaries documented.
- **[chrome-review](https://github.com/morgan-coded/chrome-review)** — a static-only Chrome MV3 extension analyzer with no extension-code execution or telemetry.
