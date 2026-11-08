# End-to-End Configuration Orchestration

## Objective
AI-SECF is intended to be introduced into a new or existing repository and used by Claude Code to produce a coherent, project-tailored configuration ecosystem. This document defines the end-to-end orchestration, not the software project's development process.

## Required workflow
1. **Locate and identify:** Confirm repository root, framework location/version, Claude Code environment/version, and whether this is a new or existing project.
2. **Discover:** Inspect relevant project context, structure, manifests, scripts, documentation, and existing Claude configuration.
3. **Inventory:** Enumerate existing configuration artifacts and classify ownership, scope, purpose, validity, and current use.
4. **Analyze:** Identify what Claude needs to know and do in this repository, including recurring tasks and contextual boundaries.
5. **Decide:** Select required artifacts using the artifact-selection matrix and minimum-sufficient-configuration principle.
6. **Blueprint:** Build a dependency-aware plan with exact paths, rationale, content outline, and risk/approval classification.
7. **Reconcile:** Reuse valid existing artifacts, update stale or incomplete artifacts, create missing artifacts, and propose removal only when justified.
8. **Generate:** Create or update safe artifacts automatically, preserving unrelated content.
9. **Validate:** Check each artifact and the configuration ecosystem as a whole.
10. **Report:** Summarize changes, preserved artifacts, omissions, unresolved decisions, validation, and next steps.

## New project mode
A new or empty repository has little or no project-specific context. Generate a minimal starter configuration using confirmed information only. Use clearly marked TODOs for unknown project facts; do not fabricate stack choices, commands, conventions, or workflows. Re-run discovery and update configuration as the project takes shape.

## Existing project mode
Existing project configuration is input to be assessed, not disposable material. Determine whether each artifact is valid, useful, redundant, conflicting, stale, or unsupported. Preserve useful user-authored content. Prefer focused edits over replacement. If ownership or intent is unclear, retain the artifact and ask before making a destructive change.

## Automatic generation principle
The normal outcome of initialization is actual file generation, not merely a recommendation report. Generate all justified, low-risk project configuration artifacts after discovery and blueprinting. Do not require the user to approve routine creation of a concise CLAUDE.md, manifest, profile, or ordinary documentation/rule files when their contents are evidence-backed and do not alter runtime permissions or execute code.

## Approval-gated changes
Do not silently activate or widen:
- tool permissions or permission modes;
- hooks or executable automation;
- MCP servers, plugins, marketplaces, or external integrations;
- credentials, secret access, network access, or data transmission;
- destructive commands, publishing, deployment, or external side effects.

For these, automatically prepare a proposal and configuration draft where safe, but wait for explicit approval before activation.

## Completion
Initialization is complete when the generated and retained artifacts form a coherent, validated configuration system and the report clearly states any blocked or approval-gated items.
