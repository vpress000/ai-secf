# Configuration Quality Gates

A configuration package is ready for activation only when:

- [ ] Project profile is evidence-backed.
- [ ] Blueprint explains why each artifact exists.
- [ ] Existing configuration has been preserved or migration approved.
- [ ] Root `CLAUDE.md` is concise and points to relevant detail.
- [ ] Every rule has an appropriate scope.
- [ ] All settings use documented keys and valid JSON.
- [ ] Agents and skills have distinct responsibilities.
- [ ] Hooks, MCP, plugins, and permission changes have explicit approval.
- [ ] Secrets and sensitive values are absent.
- [ ] References and paths resolve.
- [ ] Conflicts and duplicated instructions have been reviewed.
- [ ] Validation report distinguishes tested from untested behavior.
- [ ] A rollback path exists for material runtime changes.
