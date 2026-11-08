# Settings Standard

## Scope
Settings change Claude Code runtime behavior. They are not ordinary prose instructions.

## Rules
- Generate `.claude/settings.json` only for intentional, shared project behavior.
- Do not generate or commit `.claude/settings.local.json`; it is user-specific.
- Do not write to user-level settings or `~/.claude.json` during project bootstrap.
- Use strict valid JSON; no comments or trailing commas.
- Use only keys and values supported by the documented Claude Code version.
- Include a schema reference only when its validity and usefulness have been checked.
- Explain non-obvious settings in a companion note or manifest.
- Do not choose permissive defaults for convenience.
- Review setting scope and precedence; list-valued settings may merge differently from scalar settings.
- Validate using current documentation and Claude Code diagnostics where available.

Never assume a project-level setting can override organization-managed policy.
