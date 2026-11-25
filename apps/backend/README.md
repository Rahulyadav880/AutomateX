# AutomateX Backend

The backend is an Express API that handles authentication and workflow operations. It uses MongoDB through the shared `db` package and validates authentication and workflow input with schemas from `common`.

## Requirements

- Bun (the repository's package manager and backend runtime)
- A reachable MongoDB instance

## Configuration

Create `apps/backend/.env` with:

```env
MONGO_URL=mongodb://localhost:27017/automatex
JWT_SECERTE=replace-with-a-long-random-secret
PORT=3000
```

`MONGO_URL` and `JWT_SECERTE` are required by the current server implementation. `PORT` is optional and defaults to `3000`.

## Run

Install dependencies once from the repository root:

```bash
bun install
```

Then start the backend:

```bash
cd apps/backend
bun run dev
```

Use `bun run start` to run without hot reload, or `bun run build` to type-check and emit the TypeScript build.

## API

- `POST /signup` and `POST /signin` provide account registration and authentication.
- Authenticated workflow routes create, list, retrieve, update, and inspect executions.
- `GET /nodes` lists the available workflow node definitions.

Protected routes expect a bearer token in the `Authorization` header. The root README contains the endpoint table and request examples.
