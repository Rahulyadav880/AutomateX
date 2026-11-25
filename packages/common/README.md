# `common`

Shared validation schemas and trading metadata used by the AutomateX apps. Keeping these definitions in one workspace package helps the frontend and backend agree on workflow and authentication payload shapes.

## Exports

Import API schemas from the package's exported `types` subpath:

```ts
import { CreateWorkflowSchema, userSignInSchema, userSignUpSchema } from "common/types";
```

The schemas validate signup and signin payloads and workflow node/edge data. The package source also defines shared trading metadata, supported assets, and trigger metadata types.

## Development

Install dependencies from the repository root with `bun install`. This package is linked into the workspace and consumed directly by the backend and client.
