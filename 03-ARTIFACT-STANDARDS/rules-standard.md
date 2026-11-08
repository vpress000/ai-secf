# Modular Rules Standard

Use rules for stable, reusable instructions with a distinct topic or scope.

Each rule file should:
- have one clear subject;
- state applicability explicitly;
- use supported Claude Code rule-file conventions and frontmatter;
- be short enough to scan and maintain;
- avoid copying the root instructions;
- link to canonical project docs for detailed facts;
- include concrete examples only where they clarify behavior.

For path-specific rules, use only documented path/frontmatter syntax. Validate glob patterns against actual repository paths. Do not assume a rule applies merely because its filename suggests a scope.
