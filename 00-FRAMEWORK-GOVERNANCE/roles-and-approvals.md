# Roles and Approval Boundaries

## Framework operator
Runs discovery, prepares the blueprint, generates drafts, validates artifacts, and reports limitations.

## Project owner or maintainer
Confirms project intent, authoritative conventions, intended Claude use cases, and project-wide configuration changes.

## Security or platform owner
Reviews permission changes, hooks, MCP integrations, external network access, credentials handling, and organization-managed settings where relevant.

## Human approval required before
- adding or widening tool permissions;
- adding hooks that execute commands or modify files;
- adding MCP servers or external integrations;
- enabling plugins or marketplaces;
- introducing credentials, environment variables, or secret access;
- adding automation that can delete, overwrite, publish, deploy, or transmit data;
- replacing existing configuration with materially different behavior.

Claude may prepare proposals and explain trade-offs, but must not self-approve these changes.
