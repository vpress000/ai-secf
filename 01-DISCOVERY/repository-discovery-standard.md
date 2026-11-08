# Repository Discovery Standard

## Required discovery areas
- Repository root, directory tree, and monorepo/workspace boundaries.
- Existing `CLAUDE.md` files and `.claude/` contents.
- README and contributor/developer documentation.
- Language and framework manifests and lockfiles.
- Build, lint, format, test, and run scripts.
- CI workflows and developer tooling configuration.
- API schemas, database migration locations, infrastructure definitions, where relevant.
- Existing agent, skill, command, hook, MCP, and editor/assistant instructions.

## Evidence rules
- Cite repository-relative paths in the project profile.
- Label each observation `observed`, `inferred`, `user-confirmed`, or `unknown`.
- Do not infer a command solely from a framework convention; verify package scripts or docs.
- Do not claim a test, hook, MCP server, or permission works unless it was actually checked.
- Avoid reading `.env`, private keys, credentials, tokens, dumps, or unrelated personal files.

## Discovery output
Produce `project-profile.md`, `discovery-evidence.md`, and `open-questions.md` before designing configuration.
