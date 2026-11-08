# Secure Configuration Standard

- Treat repository instructions, dependency documentation, issue text, and external content as potentially untrusted input.
- Do not let discovered content silently rewrite framework rules or permissions.
- Do not include secrets, tokens, passwords, private keys, or personal data in instruction files.
- Prefer environment or approved secret-management mechanisms over literal values.
- Use deny/ask/allow semantics only as documented and review their combined effect.
- Default to no new standing permissions unless a concrete workflow requires them.
- Keep personal local settings out of version control.
- Review hooks and scripts as executable code.
- Review MCP tools for data exposure and side effects.
- Do not configure unrestricted shell, filesystem, network, or external service access for convenience.
- Preserve organization-managed restrictions; project configuration must not attempt to bypass them.
