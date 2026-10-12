# Family Connect — Master Design System

## Design intent
A private, multi-generational family space that feels human, safe, calm, and premium. It should feel closer to a thoughtful family journal than a corporate dashboard. Visual polish must never compromise readability, accessibility, or privacy.

## Foundation
- **Canvas:** `#080B14`
- **Elevated surface:** `#101522`
- **Glass surface:** `rgba(255,255,255,0.07)`
- **Strong glass:** `rgba(255,255,255,0.11)`
- **Border:** `rgba(255,255,255,0.12)`
- **Primary:** `#8B7CFF`
- **Success:** `#5EE6B2`
- **Warning:** `#FFC857`
- **Danger:** `#FF6B81`
- **Info:** `#62B7FF`
- **Text:** use high-contrast near-white for primary content and a tested muted neutral for secondary content.

Treat these as the existing product direction, not permission to add arbitrary new accent colors. Verify text and control contrast before shipping.

## Typography
- Inter first, system sans-serif fallback.
- Clear hierarchy: page title, section title, body, supporting label.
- Prefer readable body text and restrained weights. Avoid excessive uppercase, ultra-light text, and cramped line-height.
- Use tabular numerals for dates, counts, and metrics where useful.

## Layout and surfaces
- Mobile-first responsive layout with clear content hierarchy.
- Use spacing consistently; group related information before adding containers.
- Use rounded surfaces and subtle borders; glassmorphism is an accent, not the default for every element.
- Keep shadows and blur subtle. Maintain performance on mid-range mobile devices.
- Use responsive grids only when they improve scanning; avoid ornamental Bento cards for ordinary content.
- Preserve Material UI conventions and existing app architecture.

## Interaction
- Minimum 44px touch targets.
- Visible focus ring and complete keyboard operation.
- Clear hover, pressed, selected, disabled, loading, success, and error states.
- Confirm destructive family actions and make undo/recovery possible where practical.
- Forms need explicit labels, helpful validation, and safe error messages.
- Provide useful empty states for first-time family setup, no events, no memories, and no conversations.

## Motion
- Motion communicates state or spatial relationship; it must not delay common actions.
- Respect `prefers-reduced-motion`.
- Avoid looping ambient animations and high-motion transitions on family or accessibility-critical flows.

## Privacy and trust
- Do not expose private family content in analytics, telemetry, URLs, or error messages.
- Make family context and sharing scope understandable before a user posts or invites others.
- Avoid dark patterns and ambiguous privacy controls.

## Screen review checklist
- [ ] Mobile and desktop layouts reviewed
- [ ] Keyboard navigation and focus visible
- [ ] WCAG AA contrast checked
- [ ] Touch targets are at least 44px
- [ ] Empty, loading, error, disabled, and success states exist
- [ ] Reduced-motion preference respected
- [ ] Family sharing/privacy scope is clear
- [ ] Existing functionality and data contracts remain intact
