# arken/packages/seer/packages/ANALYSIS.md

## Folder
`arken/packages/seer/packages`

## Purpose
- Container for Seer package submodules (`node`, `protocol`).

## Key files
- `README.md`
- child submodules: `node/`, `protocol/`

## Current status
- Submodules initialized in this run.
- Deepest-first protocol analysis chunks completed in `protocol/src/modules/oasis`, `protocol/src/modules/isles`, `protocol/src/modules/infinite`, and `protocol/src/modules/evolution`, summarized upward into `protocol/src` and `protocol` docs.
- Follow-up source analysis completed for protocol root files (`protocol/src/index.ts`, `protocol/src/router.ts`, `protocol/src/types.ts`) to merge leaf findings upward.
- Initial leaf-first source analysis completed for `node/src`, extended with `node/src/data` legacy-payment artifact docs (`node/src/data/{README.md,ANALYSIS.md}`).

## Risks
- Protocol/interface drift risk remains high due to permissive contracts in several reviewed modules (including `evolution`).
- Isles and Infinite modules currently show likely router/service wiring errors and weak schema boundaries.
- Evolution module concentrates reward/payment logic in a large service surface with limited protocol test guardrails.

## Next test/protocol checks
- Move from leaf analysis to protocol-hardening test plans in reviewed modules (`evolution`, `isles`, `infinite`, `oasis`).
- Mirror the same doc + analysis pass in `node/` submodule folders.
- Run package tests/typecheck once targeted protocol changes are introduced.
