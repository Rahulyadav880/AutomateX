# `db`

Shared MongoDB models for AutomateX. The package uses Mongoose and is consumed by the backend API.

## Exports

Import the database connection helper and models from `db/client`:

```ts
import { ExecutionModel, NodesModel, UserModel, WorkflowModel, connectDB } from "db/client";
```

`connectDB(uri)` connects Mongoose to the supplied MongoDB URI. The exported models represent users, workflows, workflow node definitions, and workflow executions.

## Development

Install dependencies from the repository root with `bun install`. The package is linked into the workspace and does not run as a standalone service.
