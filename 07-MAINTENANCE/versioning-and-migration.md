# Versioning and Migration

Track separately:
- AI-SECF framework version;
- generated configuration package version or revision;
- Claude Code version used for compatibility validation.

For framework upgrades:
1. Read the changelog and migration notes.
2. Compare current manifest against new requirements.
3. Generate a migration plan.
4. Preserve local/user-owned content.
5. Apply changes incrementally.
6. validate syntax, scope, security, and runtime behavior.
7. Record deprecated mechanisms and migration status.

Do not automatically rewrite all project configuration when a framework version changes. Apply only relevant, justified migrations.
