# Morgan Carr

**AI/LLM & TypeScript engineer** — I build LLM integrations, MCP tooling, and static-analysis / developer tools, and I ship focused, tested fixes upstream in the libraries I use.

Night-time coder. My work lands as small, well-tested pull requests in real projects — **40+ merged into external open-source repos**, including the official OpenAI Node SDK, promptfoo, txtai, kysely, react-jsonschema-form, ast-grep, protobuf.js, and meriyah.

**Focus areas**
- **AI / LLM** — OpenAI/Anthropic SDKs, structured outputs, streaming, tool/function calling, RAG, and MCP (Model Context Protocol) servers
- **TypeScript / Node** — SDK & API work, type-level correctness, parsers/ASTs
- **Static analysis & tooling** — ESLint plugins, linting, package analysis, and the edge-case fixes that get merged into major libraries
- **Backend reliability** — REST APIs, Postgres/Prisma, webhooks, idempotency

## Projects

- **[ast-lens-mcp](https://github.com/morgan-coded/ast-lens-mcp)** — MCP server for AST-based code intelligence on TypeScript/JavaScript codebases ([npm](https://www.npmjs.com/package/ast-lens-mcp)).
- **[mcp-source-lint](https://github.com/morgan-coded/mcp-source-lint)** — static checks for MCP server source that catch stdio corruption and missing handler input schemas.
- **[agent-bisect](https://github.com/morgan-coded/agent-bisect)** — git-bisect for agent runs: deterministically localizes the first breaking step in an agent transcript, and abstains when it can't.
- **[chrome-review](https://github.com/morgan-coded/chrome-review)** — TypeScript static analyzer for Chrome MV3 extensions.

## Recent upstream contributions

- [openai/openai-node #1985](https://github.com/openai/openai-node/pull/1985) · [#1987](https://github.com/openai/openai-node/pull/1987) — Zod v4-mini schema support + stream rehydration in the official OpenAI SDK
- [promptfoo/promptfoo #9994](https://github.com/promptfoo/promptfoo/pull/9994) — RAG grader variable precedence
- [neuml/txtai #1130](https://github.com/neuml/txtai/pull/1130) — new dense ANN index backend
- [kysely-org/kysely #1919](https://github.com/kysely-org/kysely/pull/1919) — Postgres session-level advisory locking for exclusive migrations
- [cline/cline #12023](https://github.com/cline/cline/pull/12023) — crash fix in structured run-command history export
- [rjsf-team/react-jsonschema-form #5152](https://github.com/rjsf-team/react-jsonschema-form/pull/5152) — option-description rendering across 12 widgets
- [meriyah/meriyah #576](https://github.com/meriyah/meriyah/pull/576) — parser fix for class fields named `get`/`set`
- [protobufjs/protobuf.js #2358](https://github.com/protobufjs/protobuf.js/pull/2358) — parser hardening against malformed input
- [ast-grep/ast-grep #2787](https://github.com/ast-grep/ast-grep/pull/2787) — bounded-channel backpressure

…plus merged fixes across the ESLint plugin ecosystem (eslint-plugin-n, -regexp, -yml, -playwright, -import-x, eslint-stylistic, and more).

## Tech

TypeScript · Node.js · Python · React/Remix · Postgres/Prisma · Vitest · Playwright · MCP · OpenAI/Anthropic SDKs
