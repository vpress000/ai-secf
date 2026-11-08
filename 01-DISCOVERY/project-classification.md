# Project Classification Guide

Classify only dimensions that affect Claude configuration.

| Dimension | Examples | Configuration impact |
|---|---|---|
| Repository shape | single package, monorepo, multi-repo | instruction scopes and path-specific rules |
| Main technologies | Python, TypeScript, Go, Java, Rust | language/tool rules where useful |
| Product shape | library, CLI, web app, mobile app, service, data project | task context and workflow instructions |
| Maturity | prototype, active product, legacy | discovery depth and caution |
| Work patterns | tests, migrations, API changes, docs, release | skills/commands only for recurring workflows |
| Integration needs | MCP, issue tracker, cloud platform | integration proposal and approval |
| Team context | solo, shared repository, organization-managed | shared vs local configuration guidance |

Classification is descriptive, not prescriptive. Do not create a rule file for every detected technology. Create it only when specialized, recurring instructions are needed.
