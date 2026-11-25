# `@repo/eslint-config`

Shared ESLint flat configurations for workspace packages and apps.

## Available configurations

| Import path | Export | Intended use |
|---|---|---|
| `@repo/eslint-config/base` | `config` | Base JavaScript and TypeScript rules |
| `@repo/eslint-config/react-internal` | `config` | React and React Hooks rules |
| `@repo/eslint-config/next-js` | `nextJsConfig` | Next.js rules |

Import the configuration needed by an app's `eslint.config.js` and include it in that app's flat config. The React and Next.js configurations build on the shared base rules.
