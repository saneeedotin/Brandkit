# Website editing guide

For anyone changing www.saneee.in. The site is Next.js (App Router) in `Z:\saneee.in\website`, and it deploys to Vercel.

## Where things live

| What | File |
|---|---|
| Colours, fonts, type scale, all styles | `src/app/globals.css` (tokens at the top) |
| Fonts loaded, site title, description, icons | `src/app/layout.tsx` |
| Site URL | `src/data/site.ts` |
| Services text | `src/data/services.ts` |
| Case studies | `src/data/projects.ts` |
| Team | `src/data/team.ts` (photos in `public/img/team-*.webp`) |
| Logo and favicons | `public/img/` (`logo-black.svg`, `logo-white.svg`, `favicon.*`) |
| Brand font | `public/fonts/saneee-brand-regular.woff2` |
| Sane pages | `src/app/(sane)/…` |
| Insane pages | `src/app/insane/…` |

Most content edits are in `src/data/`. You rarely need to touch components to change text.

## Tokens

These are the only colour and type values to use. They're in `globals.css` and in [tokens.css](tokens.css).

```css
--ink: #080808;   --paper: #f6f6ef;   --lime: #c7ff2e;   --grey: #5f5f5a;
--gutter: clamp(16px, 3vw, 48px);
--font-brand: "Saneee Brand";  --font-editorial: Instrument Serif;  --font-body: Instrument Sans;
--text-h1 … --text-h4, --text-body-lg, --text-body, --text-label
```

Don't type raw hex codes or font names in new CSS. Use `var(--…)`.

## Classes to reuse

| Class | Gives you |
|---|---|
| `.sane` / `.insane` | The world: paper ground or lime ground |
| `.label` | Brand caps eyebrow, 13px, +0.08em |
| `.h1` `.h2` `.h3` `.h4` | Brand headings on the scale |
| `.h-editorial` | Big serif italic line |
| `.voice` | Serif italic voice line |
| `.lead`, `.body` | Intro sizes |
| `.switch` | Pill button (44px, 1.5px outline) |
| `.more-link` | Small "Know more →" link |
| `.vh` | Visually hidden text for screen readers and SEO |

## Rules for edits

- **Both worlds.** A page usually exists in `(sane)` and in `insane`. Change both, or check that the insane one still makes sense.
- **Lime text never goes on paper.** On insane pages, the selection flips to ink.
- **One `<h1>` per page.** The home hero's visible SANEEE is artwork. The real H1 is hidden text.
- **Metadata:** every page sets `title`, `description` and `alternates.canonical`. New pages must too.
- **Images:** WebP, real `alt` text, no stock.
- **Motion:** respect `prefers-reduced-motion`. The portal blob steps aside over text, so keep text as real text, not images.
- **Accessibility:** 44px minimum tap targets, visible focus (the outline is already set), body text 16px or more.

## Deploying

1. Work on a branch, then commit as `saneee <saneeedotin@gmail.com>`. Vercel only accepts that author.
2. Push to the `insane` remote's `main`: `git push insane <branch>:main`, from any folder inside the repo.
3. Vercel builds and publishes www.saneee.in.

Don't run `next build` in the main folder while `next dev` is running on :3000. It breaks the dev server.
