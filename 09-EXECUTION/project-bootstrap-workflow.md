# Project Bootstrap Workflow

## Inputs
- Path to the AI-SECF framework.
- Target repository root.
- Permission to inspect repository files.
- Optional project-owner answers to material unknowns.

## Operator procedure
1. Start Claude Code at the target repository root.
2. Provide the framework path and bootstrap prompt.
3. Ask Claude to perform read-only discovery first.
4. Review the project profile and evidence.
5. Review the proposed blueprint before generation.
6. Approve or reject each high-impact decision.
7. Generate files in a branch or recoverable working tree.
8. Inspect the diff and run validation.
9. Approve settings, permissions, hooks, MCP, and plugin changes separately.
10. Run representative Claude tasks and record results.

## Completion criteria
A bootstrap is complete when:
- the profile, blueprint, and manifest exist;
- only justified artifacts were generated, and valid existing artifacts were reused;
- existing configuration was preserved or intentionally migrated;
- validation report is complete;
- unresolved decisions are visible;
- risky behavior has not been activated without approval;
- maintainers know how to maintain the configuration.
