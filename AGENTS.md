# AGENTS.md — working rules for this repository

## Context

This repository belongs to a design test assignment: the header and hero section of
a dental clinic website called "Belaya Liniya" (White Line). The site is built in
Tilda; there is no site code here. The repository stores documentation, assets and
screenshots.

## Source of truth

- `docs/brief.md` — positioning, audience, tone of voice.
- `docs/copy.md` — all copy. Any wording change starts here.
- `docs/design-system.md` — palette, fonts, sizes, states, breakpoints.

Do not introduce new colors, fonts, sizes or copy without updating the matching
document. Any discrepancy between `docs/` and the Tilda build is a bug.

## Scope

- Only the header and the hero section. Do not add other sections, a footer, extra
  pages or "bonus" blocks unless explicitly asked.
- Do not use ready-made Tilda templates.
- Figma is not used: no mockups for three breakpoints.
- Responsive breakpoints follow Tilda: 1200 / 960 / 640 / 480.

## Tilda

- Never invent block IDs or settings: verify in the editor or ask.
- Zero Block: separate Desktop and Mobile artboards; tablet is fixed with targeted CSS.
- Custom CSS goes into the site HEAD. Selectors must be scoped to the block record ID
  (`#rec...`), otherwise other blocks break.
- CSS is a last resort for things settings cannot do: hover states, shadows, form
  field styling, fractional sizes. Do not break the layout of standard blocks globally.

## Assets

- Photos: free stock cleared for commercial use (Unsplash, Pexels). Record the source
  and license next to each file.
- Weight: hero up to ~300 KB, webp, max width 1920 px.
- Logo and icons: SVG.

## Git

Read-only access. Never run `add`, `commit`, `push`, `checkout`, `reset`, `stash` or
similar. When a change needs to be recorded, show the user the exact commands.

## Communication

- Reply in Russian, keep it short and concrete.
- No restating the obvious, no design theory unless asked.
- Flag debatable decisions explicitly, with an alternative and its time cost.
