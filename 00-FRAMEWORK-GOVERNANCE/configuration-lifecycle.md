# Configuration Lifecycle

## Stage 0 — Prepare
- Identify repository root and whether it is trusted.
- Identify the framework version and Claude Code version.
- Establish whether existing Claude configuration must be preserved.
- Work in a branch or create a recoverable backup before substantial changes.

## Stage 1 — Discover
- Inspect repository structure, README files, manifests, build scripts, CI definitions, existing instructions, and relevant docs.
- Identify languages, frameworks, tools, package managers, test commands, monorepo boundaries, and developer workflows.
- Do not inspect secrets or private user data unnecessarily.
- Record evidence paths and confidence.

## Stage 2 — Profile
- Create a project profile describing observed facts, inferred facts, unknowns, and stakeholder decisions.
- Identify likely Claude task types and recurring workflows.
- Identify context boundaries: root, packages, services, directories, file types.

## Stage 3 — Design
- Create a configuration blueprint before writing files.
- For each proposed artifact record purpose, audience, scope, trigger, source facts, dependencies, risk, and rationale.
- Mark each item required, recommended, optional, or not applicable.
- Resolve high-impact unknowns with the user.

## Stage 4 — Generate
- Generate using native Claude Code file formats and current documented syntax.
- Preserve existing user-authored content unless explicitly authorized to change it.
- Avoid changing application source files during configuration generation.
- Do not activate risky behavior as a side effect of drafting configuration.

## Stage 5 — Validate
- Parse structured files.
- Check names, paths, references, frontmatter, schemas, and duplicate/conflicting instructions.
- Review permissions, hooks, MCP, and executable content separately.
- Test representative instruction discovery and configuration loading where possible.

## Stage 6 — Review and activate
- Present a file-by-file summary and diff.
- Obtain approval for permissions, hooks, MCP servers, plugins, executable scripts, and any destructive or networked behavior.
- Activate only approved changes.

## Stage 7 — Maintain
- Reassess after structural, stack, workflow, or team changes.
- Detect stale paths, obsolete commands, duplicated rules, and unsupported settings.
- Update manifest and validation report with every material change.
