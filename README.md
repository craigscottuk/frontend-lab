# Frontend Lab

Experiments in frontend development, UI component libraries, responsive design, and accessibility, with documented comparisons and learning notes.

The first experiment compares two independent foundations for a future mobile-first personal organiser. The finished organiser will be developed in a separate production repository.

| Prototype | Stack |
| --- | --- |
| A | Next.js, React, TypeScript, Tailwind CSS, shadcn/ui (Base UI), assistant-ui |
| B | Next.js, React, TypeScript, Tailwind CSS, DaisyUI 5 |

## Structure

```text
experiments/personal-organizer/
  shadcn/   # Prototype A; independent npm application
  daisyui/  # Prototype B; independent npm application
docs/       # Documentation approach and cross-experiment notes
AGENTS.md   # Guidance for future development sessions
```

There is no root package or shared runtime dependency. Each application has its own `package.json` and lockfile.

## Run locally

Use Node.js 20.9 or newer and npm. In separate terminals:

```bash
cd experiments/personal-organizer/shadcn
npm ci
npm run dev
```

```bash
cd experiments/personal-organizer/daisyui
npm ci
npm run dev -- --port 3001
```

Open `http://localhost:3000` and `http://localhost:3001` respectively. Run `npx tsc --noEmit`, `npm run lint`, and `npm run build` from each application directory when changing its setup or code.

## Scope

Phase 0 establishes the toolchains and library configuration only. Both applications retain the Next.js starter screen. Later phases will compare general UI components, responsive behaviour, accessibility, and AI chat components. No organiser UI, chat functionality, backend, or model provider is implemented yet.

Record experiment-specific findings near the relevant application and broader comparisons under [`docs/`](docs/README.md).

## Dependency advisory

`npm audit` currently reports an upstream `braces` advisory, primarily through development and shadcn CLI tooling. Our review found no compatible patched version. We are not applying npm's incompatible major-version downgrade suggestions and will review upstream fixes periodically.
