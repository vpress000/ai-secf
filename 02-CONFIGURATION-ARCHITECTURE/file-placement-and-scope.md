# File Placement and Scope Standard

- Put project-wide, always-relevant guidance in the root `CLAUDE.md`.
- Put genuinely directory-specific guidance in nested `CLAUDE.md` files or path-scoped rules, choosing the native mechanism best supported by current Claude Code documentation.
- Put modular topic guidance in `.claude/rules/` when it has a distinct purpose, scope, or maintenance owner.
- Put reusable task procedures in skills when on-demand loading is appropriate.
- Put delegated specialist behavior in agents only when delegation has a clear benefit.
- Put shared project settings in `.claude/settings.json` only when team-wide behavior is intended.
- Never generate personal settings or credentials into the repository.
- Keep generated scripts in a clearly named and reviewed location; do not hide executable logic inside opaque configuration.
- Use stable, descriptive filenames. Avoid ambiguous names such as `misc.md`, `general2.md`, or `new-rules.md`.
- Do not create empty placeholder directories or files merely to match an example tree.
