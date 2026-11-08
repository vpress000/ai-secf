# Context Inventory Standard

For each useful context item, record:
- topic and concise summary;
- authoritative source path;
- confidence and last-verified date;
- intended Claude tasks;
- scope (whole repository, package, directory, file type);
- whether the source is stable or likely to change;
- whether Claude needs the full content or only a pointer.

Prioritize context that is difficult to infer from code and materially improves decisions:
- project purpose and boundaries;
- repository map and package relationships;
- canonical development commands;
- architectural conventions already adopted;
- domain vocabulary;
- data and API contracts;
- known generated/vendor directories;
- contribution and review workflow;
- constraints that are not obvious from code.

Do not duplicate long documentation into CLAUDE.md. Prefer a concise pointer to the canonical source.
