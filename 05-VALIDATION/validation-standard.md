# Configuration Validation Standard

Validate in layers.

## 1. Structural
- Required files exist.
- File and directory names are valid.
- No accidental empty files or placeholder artifacts remain.
- Relative references resolve.

## 2. Syntax and native compatibility
- JSON parses strictly.
- YAML/frontmatter parses.
- Required fields and supported values are present.
- Hook event names, matcher shapes, settings keys, and file locations match current Claude Code documentation.
- No undocumented fields are assumed valid.

## 3. Semantic quality
- Each artifact has a clear purpose and scope.
- Instructions are actionable and non-contradictory.
- Root instructions are concise.
- No unnecessary duplication.
- Commands and scripts match the repository.
- Rules' path patterns match intended files.

## 4. Security
- No credentials or sensitive data.
- Permissions follow least privilege.
- Hooks and integrations have explicit approval.
- No unexpected network or destructive side effects.

## 5. Runtime checks
Where available and approved, use Claude Code diagnostics such as `/status`, `/doctor`, `claude doctor`, and `/mcp` to confirm what loaded and identify errors. Exact commands and diagnostics may evolve; verify current documentation.

## 6. Reporting
Report passed, failed, not-run, and blocked checks separately. Never label an untested configuration as fully validated.
