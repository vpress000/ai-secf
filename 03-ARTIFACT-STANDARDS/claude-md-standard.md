# CLAUDE.md Standard

## Purpose
Provide Claude with the smallest set of high-value project instructions that should be available by default.

## Recommended sections
1. Project identity and purpose.
2. Repository map (only useful landmarks).
3. Canonical commands, verified from repository sources.
4. Essential conventions and constraints.
5. How to discover detailed instructions.
6. Important safety/approval boundaries.
7. Links to authoritative documentation.

## Quality rules
- Be concise, specific, and imperative where appropriate.
- Separate mandatory instructions from suggestions.
- Do not restate obvious code or lengthy documentation.
- Do not include secrets, credentials, personal data, or machine-specific paths.
- Do not claim tools or commands exist unless verified.
- Do not include contradictory or speculative rules.
- Keep detailed domain or path-specific rules elsewhere.
- Use relative links/paths that work for collaborators.
- Check whether nested instruction files already cover a topic before adding it at root.

## Maintenance
Review when project purpose, top-level structure, commands, tooling, or major conventions change. Remove stale guidance promptly.
