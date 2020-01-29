idea: look for all `system.write` and `sys.write` calls? that's the IO boundary for all printed messages

this might be useful: https://github.com/microsoft/TypeScript/commit/7106a587cc206f6f7dd3c8306f3e42eee218508b


The issue to reference for the RFC: https://github.com/microsoft/TypeScript/issues/30433 (where `--formatter json` comes from)


this is a similar CLI option: https://github.com/microsoft/TypeScript/commit/caf0041f8a9b2eb11405e303533d805105b6a1d7 (`--listFilesOnly` doesn't make sense in build mode)


is this useful? `emitFilesAndReportErrors`

use `yarn gulp watch-tsc` to build tsc, then run `node built/local/tsc.js --formatter json --project your_tsconfig.json` to verify
