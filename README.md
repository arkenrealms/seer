# Arken Seer

Meta-repo for Seer runtime surfaces.

## Structure
- `packages/protocol` → `arkenrealms/seer-protocol` (submodule)
- `packages/node` → `arkenrealms/seer-node` (submodule)

## Notes
- Submodules are configured in `.gitmodules` to track `main`.
- Repo-level formatting/lint policy comes from `.editorconfig`, `.prettierrc`, and `.eslintrc` and currently favors migration-friendly (permissive) lint behavior.
- `.gitignore` includes private-key and secret-file patterns (`id_ed25519*`, `secrets.json`) plus generated/runtime artifacts (`coverage/`, logs, build outputs).
- Most implementation lives in the submodules; this repo mainly coordinates pointers and high-level docs.
