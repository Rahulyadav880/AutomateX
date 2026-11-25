# `@repo/typescript-config`

Shared TypeScript compiler presets for the AutomateX workspace. Extend these JSON configs from an app or package `tsconfig.json` to reuse common strict compiler options.

## Presets

| Config | Use |
|---|---|
| `base.json` | Common strict TypeScript options for workspace code |
| `react-library.json` | Base options with the React JSX transform |
| `nextjs.json` | Base options tailored for Next.js projects |

These are configuration files only; this package does not provide runtime code or its own build command.
