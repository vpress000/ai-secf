# Idempotency and Incremental Generation

AI-SECF generation must be idempotent: rerunning initialization against an unchanged repository should not create duplicate files, repeatedly rewrite content, or produce unnecessary diffs.

## Requirements
- Read current state before writing.
- Compare intended output with existing content.
- Write only when content or configuration meaningfully needs to change.
- Preserve manually maintained sections.
- Use stable paths and deterministic naming.
- Track AI-SECF-managed artifacts in the manifest.
- Mark generated content clearly only where such markers do not conflict with native file formats or user readability.
- Never assume a file is framework-managed merely because it resembles a template.
- Keep a change log of material updates.

## Incremental behavior
When project context changes, recalculate the affected artifact set. Do not regenerate the entire configuration tree for a local change. For example, a new package may require a scoped rule and manifest update, not replacement of root instructions and unrelated skills.

## Safe write strategy
Prefer branch-based changes or backups. Produce a diff before finalizing. If a write would destroy user-authored content, stop and request direction.
