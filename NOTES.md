# /arken/packages/seer/NOTES.md

## Analysis snapshot (2026-02-17)

`seer` is a wrapper repo with code split into nested submodules:
- `packages/protocol` (`arkenrealms/seer-protocol`)
- `packages/node` (`arkenrealms/seer-node`)

### Current status
- Submodule container checked out and healthy.
- Nested repos are not yet initialized in this pass.

### Next protocol-focused work
1. Initialize nested protocol/node submodules.
2. Audit websocket/tRPC wrappers and use-case coverage.
3. Add missing tests around malformed payloads, timeout lifecycles, and dispatch edge-cases.
4. Add/update concise `README.md` + maintainer `NOTES.md` in touched folders.
