# Configuration Drift Management

Review configuration when:
- languages, frameworks, package managers, or build tools change;
- scripts or canonical commands change;
- repository directories are moved or split;
- services or packages are added or removed;
- team workflows or review practices change;
- Claude Code introduces or deprecates configuration mechanisms;
- permissions, hooks, MCP integrations, or security requirements change.

Drift checks:
- broken paths and links;
- stale commands;
- rules matching no files or too many files;
- duplicated or contradictory instructions;
- unused agents/skills/commands;
- unsupported settings or frontmatter;
- integrations no longer used;
- root instructions that have grown excessively.

Update the manifest and validation report after each maintenance cycle.
