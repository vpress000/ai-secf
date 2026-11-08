# Configuration Generation Method

## Required sequence
1. Read the AI-SECF framework version and target Claude Code documentation.
2. Discover the repository without modifying it.
3. Inventory existing assistant configuration and classify each item as user-owned, project-owned, generated, or unknown.
4. Build project profile and context inventory with evidence.
5. Create a proposed configuration blueprint.
6. Identify decisions requiring the user.
7. Generate only approved artifacts.
8. Validate and produce a diff/report.

## Generation constraints
- Never overwrite existing files without comparing and preserving their intent.
- If a target file exists and ownership is unclear, stop and ask.
- Use placeholders only when clearly marked and never make them appear operational.
- Do not invent commands, scripts, endpoints, tools, MCP servers, or platform settings.
- Do not change application source code as part of configuration setup.
- Do not activate hooks or integrations while merely drafting a proposal.
- Prefer incremental changes over wholesale regeneration.
