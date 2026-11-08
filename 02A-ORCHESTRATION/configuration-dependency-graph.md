# Configuration Dependency and Coherence Model

Treat the generated configuration as an ecosystem, not a pile of independent files.

## Dependency relationships
Examples:
- Root `CLAUDE.md` points to relevant scoped rules and canonical project documents.
- A rule's path scope must match actual repository paths.
- An agent's description and tools must match the task it is delegated.
- A skill's trigger and instructions must not conflict with root or scoped instructions.
- A command should invoke verified scripts or a clearly described workflow.
- A hook must reference an existing executable and documented event.
- Settings must reference supported keys and intended project behavior.
- MCP configuration must match an approved, real server and its actual tools.

## Coherence checks
- No broken references.
- No duplicate or contradictory instructions.
- No orphaned agents, skills, commands, scripts, or configuration files.
- No path patterns that accidentally cover unrelated areas.
- No artifact that assumes a missing prerequisite.
- No settings that undermine documented safety boundaries.
- No stale manifest entries.
- No two artifacts claiming conflicting authority over the same behavior.

## Configuration graph
Maintain a simple manifest of artifacts and their relationships. A full graph database is unnecessary; a YAML manifest or table is sufficient for most projects.
