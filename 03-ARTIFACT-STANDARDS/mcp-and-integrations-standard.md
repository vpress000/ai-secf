# MCP and External Integrations Standard

Treat every MCP server, plugin, marketplace, and external integration as a trust boundary.

Before proposing one, document:
- the concrete workflow gap it addresses;
- provider and source authenticity;
- tools and data it exposes;
- authentication and credential storage model;
- data sent outside the repository;
- permissions and side effects;
- versioning and update policy;
- fallback if unavailable.

Do not invent server names, package identifiers, endpoints, or configuration keys. Do not embed credentials in tracked files. Require explicit human approval before adding or enabling an integration.
