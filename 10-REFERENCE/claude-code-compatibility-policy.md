# Claude Code Compatibility Policy

Claude Code evolves. AI-SECF does not freeze platform syntax.

Before generating platform-specific files:
1. Identify the installed Claude Code version where possible.
2. Consult the current official documentation for the relevant artifact.
3. Verify exact paths, filenames, frontmatter, JSON keys, hook event names, matcher syntax, and precedence.
4. Record the checked version/date in the project profile and manifest.
5. Prefer conservative, documented capabilities.
6. If documentation is ambiguous or a feature is version-dependent, mark it as conditional and ask before relying on it.

Do not assume older concepts remain separate features. For example, verify the current relationship between custom slash commands and skills before generating both. Do not assume every feature is available in every host, cloud session, or managed environment.

Official documentation entry point: https://code.claude.com/docs/
