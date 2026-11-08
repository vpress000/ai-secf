# AI-SECF — AI Software Engineering Configuration Framework
**Version:** 1.1.0  
**Primary target:** Claude Code  
**Purpose:** Govern the discovery, design, generation, validation, optimization, and maintenance of project-level AI coding-assistant configuration.

## Mission
AI-SECF is a meta-configuration framework. It governs the configuration artifacts that help Claude Code understand and operate appropriately within a software repository. It does **not** prescribe the project's general software-development lifecycle, application architecture, coding standards, or business governance except where project facts are needed to configure Claude.

## What AI-SECF produces
A tailored, validated configuration package for a target repository. Depending on evidence and need, that package may include:
- `CLAUDE.md` instruction entry points and scoped instruction files
- `.claude/settings.json` and optional local settings guidance
- `.claude/rules/`, `.claude/agents/`, `.claude/skills/`, `.claude/commands/`
- hooks and MCP configuration where justified and approved
- project context maps, workflow guidance, and configuration-maintenance records
- a manifest, validation report, assumptions log, and human-decision register

Not every project needs every capability. The default is **minimum sufficient configuration**, not maximum file count.

## Core operating model
1. Detect whether the target is a new/empty project or an existing repository.
2. Discover project context, structure, technologies, workflows, and existing Claude configuration.
3. Build an evidence-backed project profile and inventory existing artifacts.
4. Determine the minimum sufficient Claude configuration for this project.
5. Design a dependency-aware configuration blueprint.
6. Reuse and preserve valid existing configuration; create or update only what is needed.
7. Generate safe, low-risk configuration artifacts automatically and stage consequential runtime changes for approval.
8. Validate syntax, references, scope, conflicts, compatibility, security, and ecosystem coherence.
9. Present a change report, unresolved decisions, and validation results.
10. Maintain configuration idempotently as the repository and Claude Code evolve.

## Authority and compatibility
AI-SECF requirements describe what a sound configuration system should achieve. Claude Code's current official documentation defines supported filenames, schemas, frontmatter, settings keys, hook events, and runtime behavior. Never invent native Claude Code capabilities. Check the official documentation before generating or changing platform-specific configuration.

Official references:
- Claude Code documentation: https://code.claude.com/docs/
- Memory and CLAUDE.md guidance: https://code.claude.com/docs/en/memory
- Settings and precedence: https://code.claude.com/docs/en/settings
- Subagents: https://code.claude.com/docs/en/sub-agents
- Skills: https://code.claude.com/docs/en/skills
- Hooks: https://code.claude.com/docs/en/hooks
- MCP: https://code.claude.com/docs/en/mcp
- Slash commands: https://code.claude.com/docs/en/slash-commands
- Permissions: https://code.claude.com/docs/en/permissions

Documentation URLs and platform capabilities can change. Record the date and Claude Code version used for compatibility checks.

## Package map
- `00-FRAMEWORK-GOVERNANCE/` — framework scope, principles, lifecycle, roles
- `01-DISCOVERY/` — repository discovery and evidence capture
- `02A-ORCHESTRATION/` — end-to-end generation workflow, reconciliation, idempotency, and ecosystem coherence
- `02-CONFIGURATION-ARCHITECTURE/` — instruction hierarchy and artifact selection
- `03-ARTIFACT-STANDARDS/` — standards for each Claude configuration artifact
- `04-GENERATION/` — generation method, templates, change safety
- `05-VALIDATION/` — quality gates and test approach
- `06-SECURITY/` — permission, secret, trust, and integration safeguards
- `07-MAINTENANCE/` — drift detection and lifecycle management
- `08-TEMPLATES/` — reusable templates and machine-readable schemas
- `09-EXECUTION/` — operator workflow and Claude Code bootstrap prompt
- `10-REFERENCE/` — terminology and compatibility references

## Start here
1. Read `00-FRAMEWORK-GOVERNANCE/scope-and-boundaries.md`.
2. Read `09-EXECUTION/project-bootstrap-workflow.md`.
3. Provide the framework directory to Claude Code.
4. Use `09-EXECUTION/bootstrap-prompt.md` to initiate a new project.
5. Review the blueprint and approvals before activating any settings, hooks, MCP servers, or permissions.
