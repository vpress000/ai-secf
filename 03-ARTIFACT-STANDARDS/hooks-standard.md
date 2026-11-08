# Hooks Standard

Hooks are executable automation and therefore high-risk configuration.

Only propose a hook when:
- the triggering event and desired deterministic action are clear;
- the action is idempotent where practical;
- failure behavior is understood;
- output and error handling are predictable;
- runtime and platform compatibility are checked;
- the user has explicitly approved the behavior.

For every hook document:
- event and matcher;
- command or handler;
- files/processes affected;
- network access, if any;
- timeout and failure behavior;
- approval owner;
- test procedure and rollback.

Never silently install hooks that modify source files, delete data, publish content, deploy, or transmit repository content.
