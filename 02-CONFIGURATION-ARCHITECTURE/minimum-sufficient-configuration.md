# Minimum Sufficient Configuration

Start from a minimal baseline:
- one concise root `CLAUDE.md`;
- a configuration manifest and validation report maintained by the framework (these may live under `docs/ai-config/` if preferred);
- shared `.claude/settings.json` only when a specific shared setting is justified.

Add other artifacts only when a decision record explains:
1. the problem it solves;
2. the Claude task or scope it supports;
3. why a simpler existing artifact is insufficient;
4. the maintenance cost;
5. any security or compatibility implications.

A project with many technologies does not automatically need many rule files. A large repository does not automatically need agents. An available integration does not imply it should be enabled.
