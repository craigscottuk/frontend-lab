# Personal organiser: shadcn/ui foundation

This is an independent Next.js App Router, TypeScript, and Tailwind CSS application. Phase 0 configures shadcn/ui with the Base UI `base-nova` style and installs the `@assistant-ui/react` core package. The screen is still the Next.js starter.

Run `npm ci` and `npm run dev` from this directory. Verify changes with `npx tsc --noEmit`, `npm run lint`, and `npm run build`.

`components.json` contains the shadcn aliases, CSS variable setup, and assistant-ui's style-aware registry. The registry resolves Base UI versions because the shadcn style is `base-nova`. For Phase 1, the official command to add the initial chat pieces is:

```bash
npx shadcn@latest add @assistant-ui/thread @assistant-ui/thread-list
```

Add other components only when needed. Any chat runtime, backend, and provider setup belongs to a later phase. See the [assistant-ui installation guide](https://www.assistant-ui.com/docs/installation) and [CLI guide](https://www.assistant-ui.com/docs/cli).
