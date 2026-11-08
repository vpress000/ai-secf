# AI-SECF Project Bootstrap Prompt

You are initializing or reconciling Claude Code's project-level configuration for this repository using AI-SECF at: [PROVIDE FRAMEWORK PATH].

Your objective is to generate a coherent, project-tailored Claude configuration ecosystem. You are NOT being asked to redesign the software project or impose general software engineering standards.

Read the AI-SECF framework, including its orchestration, discovery, architecture, artifact standards, generation, validation, and security documents. Check current official Claude Code documentation for all native configuration syntax and capabilities.

## Phase 1 — Identify mode and discover
Determine whether this is a new/empty project or an existing repository. Inspect repository structure, context, technology stack, manifests, scripts, relevant documentation, and existing Claude configuration. Avoid secrets and private data. Do not modify files during discovery.

Create or update:
- `docs/ai-config/project-profile.md`
- `docs/ai-config/discovery-evidence.md`
- `docs/ai-config/open-questions.md`

Label facts as observed, inferred, user-confirmed, or unknown.

## Phase 2 — Inventory and design
Inventory existing Claude artifacts, including ownership and purpose. Reuse valid existing configuration. Create `docs/ai-config/configuration-blueprint.md` and `docs/ai-config/configuration-manifest.yaml`.

Select the minimum sufficient artifact set. For every proposed artifact, record path, purpose, scope, rationale, evidence, dependencies, and approval status. Identify conflicts and material unknowns.

## Phase 3 — Generate automatically
After discovery and blueprinting, automatically create or update all justified, low-risk configuration files. This normally includes a concise root `CLAUDE.md` and any necessary rules or supporting configuration documentation.

For an existing project, preserve and reconcile useful configuration; make minimal diffs and do not replace files wholesale. For a new project, use confirmed facts and clearly marked TODOs for unknowns. Do not invent project details, commands, conventions, tools, or workflows.

Do not modify application source code. Do not write user-level settings or credentials. Do not create optional artifacts merely because the platform supports them.

## Phase 4 — Approval-gated runtime configuration
You may prepare a proposal or draft for permissions, hooks, executable automation, MCP servers, plugins, external integrations, credentials, network/data access, or destructive/external side effects. Do not activate or broaden these capabilities without explicit human approval.

If an existing file has unclear ownership or a proposed edit could destroy user-authored intent, preserve it and ask before changing it.

## Phase 5 — Validate the ecosystem
Validate syntax, native compatibility, paths, references, instruction scope, duplication, conflicts, dependencies, security, and manifest consistency. Where available and approved, use documented Claude Code diagnostics and representative task tests.

Create or update `docs/ai-config/validation-report.md`. Distinguish passed, failed, not-run, and blocked checks. Do not claim runtime behavior was verified unless it was tested.

## Phase 6 — Report
Summarize:
1. files created, updated, retained, consolidated, or deliberately not created;
2. why each artifact is needed and how the files work together;
3. validation results and untested areas;
4. approvals still required;
5. assumptions and open questions;
6. maintenance triggers.

Rerunning this process without material repository changes should produce no unnecessary changes.
