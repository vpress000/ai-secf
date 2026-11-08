# Context Budget and Instruction Efficiency

- Keep root instructions short and high-signal.
- Load specialized guidance only when its scope or task requires it.
- Prefer pointers to canonical docs over copying entire documents.
- Remove duplicated instructions and redundant examples.
- Avoid large directory dumps and generated-file inventories in default context.
- Do not create a rule for information Claude can reliably infer from nearby code.
- Use skills or referenced supporting docs for long workflows.
- Review whether each instruction changes Claude's behavior; if not, remove or relocate it.
- Do not optimize solely for token count at the expense of clarity or safety.
