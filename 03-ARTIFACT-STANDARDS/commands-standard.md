# Commands Standard

Before generating custom commands, verify the current Claude Code command mechanism and its relationship to skills. Do not create duplicate mechanisms for the same workflow.

A command should:
- represent a stable, repeatable user-invoked action;
- have a clear name, purpose, inputs, and expected output;
- avoid hidden destructive behavior;
- state whether it reads, writes, executes, or contacts external systems;
- request confirmation before consequential operations;
- reuse existing project scripts rather than reimplementing them.

If a skill is the better supported or more maintainable mechanism, use a skill instead.
