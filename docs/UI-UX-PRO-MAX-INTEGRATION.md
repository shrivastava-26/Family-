# UI UX Pro Max integration

Family Connect is adopting the official [UI UX Pro Max skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) as its design-research and UI implementation workflow.

## Install in the repository checkout

Run from the Family Connect repository root:

```bash
npx ui-ux-pro-max-cli init --ai codex
```

Use another supported `--ai` target if the repository is worked on by a different assistant. The official CLI generates the full assistant-specific skill assets; avoid copying an old, incomplete template by hand.

The UI UX Pro Max search scripts require Python 3.x. Once installed, use its search workflow for the relevant product domain, visual style, typography, palette, component stack, and UX/accessibility guidelines before significant UI work.

## Project-specific rules

- Follow `DESIGN.md` and `design-system/Family-Connect/MASTER.md`.
- Keep Material UI and the established Next.js/TypeScript architecture.
- Add page-specific guidance under `design-system/Family-Connect/pages/` for major screens.
- Validate responsive behavior, contrast, keyboard focus, reduced motion, and loading/empty/error states.
- Do not call the skill installed until the generated skill files exist in the working checkout.

## Repository/deployment status

These integration and design-system files are repository configuration only. They do not themselves install the external CLI, verify a production build, or create a Vercel deployment.
