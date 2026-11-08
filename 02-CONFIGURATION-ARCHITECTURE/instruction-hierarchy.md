# Instruction and Configuration Hierarchy

## Design layers
1. **Organization/managed policy:** Settings delivered and enforced by the organization, outside the project generator's authority.
2. **User-level preferences:** Personal configuration outside the repository; do not generate or overwrite it during project bootstrap.
3. **Shared project configuration:** Version-controlled project instructions and settings intended for collaborators.
4. **Scoped instructions:** Rules that apply only to particular paths or work areas.
5. **Task-specific context:** Skills, agents, commands, and referenced documents loaded when relevant.
6. **Session-specific choices:** Temporary runtime choices; do not persist unless the user requests it.

This is a design model, not a substitute for Claude Code's actual precedence and loading rules. Verify current platform behavior for each artifact.

## Instruction conflict rules
- Never assume all instruction sources have equal precedence.
- Avoid conflicting instructions rather than relying on precedence to resolve them.
- If conflict remains, identify both sources and ask for a decision when impact is material.
- More specific rules may refine general rules but must not silently reverse them.
- Security restrictions and organization-managed policies must not be weakened by project-generated content.

## Root instruction file
Root `CLAUDE.md` is the concise entry point: project identity, essential workflow, high-value constraints, and pointers to scoped material. It is not a dump of all project knowledge.
