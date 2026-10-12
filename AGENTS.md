# Family Connect — Agent Instructions

## UI/UX work: use UI UX Pro Max

For any interface, visual-design, accessibility, or interaction task, use the **UI UX Pro Max** design workflow before changing components.

Official project: https://github.com/nextlevelbuilder/ui-ux-pro-max-skill

Install the official skill in this repository with the current CLI:
```bash
npx ui-ux-pro-max-cli init --ai codex
```
The official installer generates assistant-specific files and the full skill assets. Do not replace it with a hand-written imitation. The search script requires Python 3.x.

## Family Connect design constraints

- Product feeling: warm, trustworthy, premium, calm, private family space — not a generic SaaS admin panel.
- Stack: Next.js 14 + TypeScript + Material UI. Respect existing app patterns; do not introduce another component system without a clear need.
- Dark foundation: background `#080B14`, elevated surface `#101522`, glass surface `rgba(255,255,255,0.07)`, stronger glass `rgba(255,255,255,0.11)`, border `rgba(255,255,255,0.12)`.
- Accent: primary `#8B7CFF`; success `#5EE6B2`; warning `#FFC857`; danger `#FF6B81`; info `#62B7FF`.
- Typography: Inter or system sans. Use a deliberate type scale and avoid tiny low-contrast text.
- Mobile-first: 44px minimum touch targets, thumb-friendly bottom navigation, responsive layouts, safe-area awareness.
- Accessibility: visible keyboard focus, semantic controls, WCAG AA contrast, reduced-motion support, accessible names, and useful empty/loading/error states.
- Use glassmorphism sparingly; preserve legibility and performance. Avoid excessive blur, gradients, decorative cards, and generic AI-dashboard patterns.
- Keep family, relationship, event, chat, and memory experiences emotionally clear and privacy-conscious.
- Reuse established design tokens/components and preserve behavior while improving visuals.

## Required UI workflow

1. Read `DESIGN.md` and `design-system/Family-Connect/MASTER.md` before styling.
2. Use UI UX Pro Max to research the relevant product/domain, style, typography, color, and UX guidance.
3. Create or update page-specific guidance under `design-system/Family-Connect/pages/` for significant screens.
4. Inspect responsive states (mobile and desktop), keyboard/focus states, empty/loading/error states, and reduced motion.
5. Run available lint, typecheck, unit, and build checks; state clearly what was and was not executed.
6. Do not claim the official skill is installed unless the generated assistant-specific skill files are present in the checkout.
