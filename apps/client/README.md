# AutomateX Client

The client is the React and Vite frontend for AutomateX. It provides the workflow canvas, authentication screens, dashboard, workflow editor, and execution history.

## Requirements

- Bun (for installing the monorepo dependencies)
- Node.js 18 or newer

## Run locally

Install dependencies once from the repository root:

```bash
bun install
```

Start the Vite development server:

```bash
cd apps/client
bun run dev
```

Open the local URL printed by Vite (normally `http://localhost:5173`). From the repository root, `bun run dev` starts the configured app development tasks together.

## Other scripts

Run these commands from `apps/client`:

| Command | Purpose |
|---|---|
| `bun run build` | Type-check and create a production Vite build |
| `bun run lint` | Run ESLint |
| `bun run preview` | Preview the production build locally |

The API client currently uses the deployed backend URL configured in `src/lib/api.ts`.
