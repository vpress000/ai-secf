# Permission Design Guidance

Permission configuration is behaviorally significant and must be conservative.

For each proposed permission, record:
- tool or command covered;
- exact scope/pattern;
- task that requires it;
- why interactive approval is insufficient;
- potential impact if misused;
- whether the permission is shared or personal;
- test and rollback approach.

Prefer narrow command patterns and limited paths. Avoid broad wildcards, unrestricted shell access, broad write permissions, or blanket approval modes. Never generate a bypass or elevated permission mode as a default. Verify current permission syntax and precedence from official documentation.
