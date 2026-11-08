# Core Principles

1. **Purpose before artifact:** Create a file only to meet a defined Claude-use need.
2. **Minimum sufficient configuration:** Prefer the smallest complete configuration that improves reliable task performance.
3. **Evidence before instruction:** Do not turn guesses into authoritative project instructions.
4. **One source of truth:** Each fact or rule should have one authoritative home; link to it rather than copying it.
5. **Layered context:** Put universally applicable project guidance at the root; specialized guidance near the relevant scope.
6. **Explicit scope:** Every instruction must make clear when and where it applies.
7. **Actionable language:** Prefer observable instructions over vague aspirations.
8. **No hidden authority:** Distinguish mandatory rules, recommendations, assumptions, and examples.
9. **Native compatibility:** Use only documented Claude Code mechanisms and valid schemas.
10. **Least privilege:** Grant only the minimum permissions required; prefer prompting over broad standing approval.
11. **Human control:** Require review for consequential permissions, hooks, external integrations, and destructive automation.
12. **Low duplication:** Avoid repeated or contradictory instructions.
13. **Context efficiency:** Keep frequently loaded instructions concise; load detail conditionally where supported.
14. **Maintainability:** Configuration must evolve with project structure, tools, and workflows.
15. **Reversibility:** Generation should be reviewable and changes should be easy to diff, revert, and explain.
16. **Portability:** Separate universal framework logic from project-specific facts and Claude-specific syntax.
17. **Honest validation:** Report what was checked, what was not checked, and any unresolved uncertainty.
