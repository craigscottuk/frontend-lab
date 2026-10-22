# Frontend Lab guidance

- This repository tests frontend technologies through small, understandable experiments. The two personal-organiser applications in `experiments/personal-organizer/shadcn` and `experiments/personal-organizer/daisyui` are independent npm projects; keep their dependencies, components, and imports separate.
- Both use Next.js App Router, React, TypeScript, and Tailwind CSS. The shadcn app uses shadcn/ui with Base UI and prepares assistant-ui; the DaisyUI app uses DaisyUI 5 alone.
- Prefer official documentation and current library conventions. Build responsive, accessible interfaces when UI development is requested.
- Avoid unnecessary dependencies, abstractions, and complexity. Keep learning notes and technical decisions concise, preferably close to the relevant experiment.
- Run relevant TypeScript, lint, and build checks after changes. Do not add a backend, AI API, model provider, or authentication unless explicitly requested.
- Git operations are managed by the user through GitHub Desktop. Do not stage files, create commits, switch branches, push changes, or modify repository history unless explicitly instructed in a future task.
