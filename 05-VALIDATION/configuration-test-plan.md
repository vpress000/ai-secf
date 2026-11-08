# Configuration Test Plan

Test representative Claude tasks rather than merely checking that files exist.

Suggested tests:
1. Start Claude at repository root and confirm project identity and essential commands are understood.
2. Ask a task scoped to a directory with special rules; confirm the correct scoped guidance is applied.
3. Ask for a task that should trigger a skill; verify discovery and output quality.
4. Verify that an agent is used only for its intended bounded role.
5. Confirm settings are loaded using documented diagnostics.
6. Confirm hooks run only on intended events and fail safely.
7. Confirm MCP integrations expose only approved tools and expected data.
8. Test a conflicting or ambiguous instruction and confirm Claude surfaces the conflict rather than silently choosing.
9. Check that user-local configuration is not tracked.
10. Re-run after a representative directory or manifest change to assess maintenance behavior.

Record environment, Claude Code version, test prompt, expected result, observed result, and limitations.
