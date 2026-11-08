# Nested Context Standard

Nested instruction files are justified only when a subtree has distinct conventions or context that Claude cannot reliably infer from the root instructions.

Rules:
- Keep scope local and avoid re-stating global rules.
- Prefer the narrowest correct scope.
- Ensure instructions remain valid for every file matched.
- Check for accidental gaps and overlapping globs.
- Record nested instruction files in the configuration manifest.
- Reassess after directory moves, renames, package splits, or merges.
