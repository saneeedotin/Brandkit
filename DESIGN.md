# Design

How saneee.in things look: colour, layout, components, imagery and motion. This applies to the website, posts, decks, ads and print.

## Colour

| Name | HEX | RGB | Token | Role |
|---|---|---|---|---|
| **Ink** | `#080808` | 8 8 8 | `--ink` | Hero, footer, nav, dark posts. All text on light grounds. |
| **Paper** | `#F6F6EF` | 246 246 239 | `--paper` | Ground of the sane world. Text on ink. |
| **Lime** | `#C7FF2E` | 199 255 46 | `--lime` | The accent and the insane world: cursor, selection, footer word, CTAs, launch posts. |
| **Grey** | `#5F5F5A` | 95 95 90 | `--grey` | Captions, metadata, secondary text. |

That is the whole studio palette. Make tints only by changing opacity: 1px lines are ink or paper at 14–16% opacity.

### Team accents

Each team member has a personal accent. Lime belongs to the studio, and it's also Param's.

| Member | Colour | HEX | Token | Ink on it |
|---|---|---|---|---|
| Param Mehta | Lime | `#C7FF2E` | `--param` | 16.9 : 1 |
| Teesha Wala | Pink | `#FF80EC` | `--teesha` | 9.1 : 1 |
| Hardik Solanki | Orange | `#FB6F2B` | `--hardik` | 7.1 : 1 |
| Smit Chauhan | Yellow | `#FFDC69` | `--smit` | 15.0 : 1 |

**Use a member accent** in place of lime on things that person owns or signs: their own posts and reels, team cards and profile pictures, decks and proposals they present, and their email signature. Their sigil tiles are in `assets/sigil/saneee-sigil-on-<name>.svg` and `assets/png/saneee-sigil-on-<name>-1080.png`.

**Keep lime** for the logo colourways, the website's two worlds, and studio-wide posts, ads and campaigns.

Rules:
- One accent per piece. Never mix two members' colours, except on a team post where each person's card wears their own.
- The accent follows the same rules as lime: ink text on top, used as punctuation or a full ground, never as text on paper.
- Grey fails contrast on pink (2.9 : 1) and orange (2.3 : 1). Use ink at 72% opacity for small text on those grounds.
- In the visual brand kit (`index.html`), the dots in the nav switch the whole kit to each member's accent.

### Contrast (WCAG)

| Pair | Ratio | OK for |
|---|---|---|
| Ink on paper | 18.5 : 1 | Everything |
| Paper on ink | 18.5 : 1 | Everything |
| Ink on lime | 16.9 : 1 | Everything |
| Lime on ink | 16.9 : 1 | Everything |
| Grey on paper | 5.9 : 1 | Body text and captions |
| Grey on lime | 5.4 : 1 | Body text and captions |
| Lime on paper | ~1.1 : 1 | **Never.** It disappears. |

### How much lime

- **Sane pieces** (most things): ink and paper do the work. Lime appears once, as a highlighted word, a pill, the cursor or a small tag.
- **Insane pieces** (launches, covers, ad hooks): a full lime ground with ink type. Plain and loud. Keep the grain (see Texture).
- Never use lime and paper together without ink in between.

## Layout

- **Type is the image.** Most frames are a big headline and a lot of space. Add photos only when they show real work or real people.
- **Gutter:** 3vw on the website, from 16px to 48px. On a 1080px post, keep 72–96px from every edge.
- **Grid:** a simple column grid. Align to the left edge. Use centred layouts only for single-line moments, such as the sigil on a cover.
- **Section labels:** `01 / Services`, in Saneee Brand caps at small size. The number is the real order. Don't number things that aren't a sequence.
- **Rules:** 1px lines at 14–16% opacity separate list rows and sections. Don't use boxes inside boxes.
- **Space is a feature.** When in doubt, make the headline bigger and the copy shorter.

## Components

| Element | Spec |
|---|---|
| **Button / tag (pill)** | Full radius (999px), 1.5px outline in the text colour, min height 44px, 18px side padding, Saneee Brand. The main action is filled in ink. |
| **Panel / image** | 4px corners, no shadow. On paper, a 1px inner line at 14% ink. |
| **List row** | 1px top rule, 10–20px vertical padding. |
| **Label** | Saneee Brand, 13px, caps, +0.08em tracking. |
| **Link arrow** | `→` after the text, as in "Know more →" or "All the work →". Saneee Brand has `→` and `↗`. |
| **Cursor** | The logo's arrow in lime with an ink outline. On the site it's the mouse pointer. In graphics it can point at the thing that matters. |
| **Selection** | Lime highlight, ink text. Flipped on lime. |

## Texture

Lime surfaces carry a **fine grain** (fractal noise at about 9% black), so flat lime doesn't look cheap or digital. Do the same in posts: a light noise layer on lime grounds only.

## Imagery

- **Client work:** show real screenshots in a device or a clean 4px frame on ink or paper. The client's own colours stay inside the frame.
- **People:** the team photos (`team-*.webp` on the site) are natural, close crops. Use real people, never stock.
- **Black and white** works for mood photos so lime and type lead. Client work stays in colour.
- **Never:** stock photos of handshakes or laptops, 3D blobs, gradient meshes, emoji as icons, or AI-generated "office" scenes.

## Motion

The site is calm by default, with one strong moment per page.

- **Hero:** the type morphs into the sigil. The arrow arrives last.
- **Portal blob:** the cursor tears a hole into the other world. It steps aside when it is over text.
- **Menu:** a liquid bubble opens from the top-right corner, in the other world's colours.
- **Easing:** `cubic-bezier(0.22, 1, 0.36, 1)` (a fast start and a soft landing). 0.3–0.6s for UI.
- Respect reduced-motion settings on the web. In reels, cut on the beat and keep text on screen long enough to read twice.

## Checklist before you ship anything

- [ ] Only Ink, Paper, Lime and Grey (client work excepted)
- [ ] No lime text on paper
- [ ] The logo or sigil comes from `assets/`, untouched
- [ ] Saneee Brand plus the serif italic only
- [ ] One main message per frame
- [ ] It works at phone size
