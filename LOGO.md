# Logo

saneee.in has two marks. Both come from the same idea: **a cursor arrow sitting where the dot of the i would be**. We build for screens, and the arrow says so.

## 1. The wordmark

Lowercase `saneee.in`, drawn in the Saneee Brand letterforms. It has a cursor arrow over the i and a small ® after it.

- Use it wherever there's room: site header, proposals, the end card of a reel, ad end frames, letterheads.
- **Minimum width:** 96px on screen, 25mm in print. Below that, use the sigil.

## 2. The sigil

The **S** from the wordmark with the cursor arrow at its top right. It's a square mark for small and social spaces.

- Use it for the favicon, app icon, Instagram profile picture, story highlight covers, stickers, watermarks and the corner of a slide.
- **Minimum size:** 16px (the favicon). Keep at least 25% padding inside a square tile.
- The **green version** (ink sigil on a lime square) is the Instagram profile picture and the cover for launch or campaign posts.

## Colourways

| Version | Files | Use for |
|---|---|---|
| Paper on ink | `logo/saneee-wordmark-paper.svg`, `sigil/saneee-sigil-on-ink.svg` | **Default.** Website, dark slides, reels, most posts |
| Ink on paper | `logo/saneee-wordmark-ink.svg`, `sigil/saneee-sigil-on-paper.svg` | Print, proposals, invoices, light slides |
| Ink on lime | `logo/saneee-wordmark-on-lime.svg`, `sigil/saneee-sigil-on-lime.svg` | Insane world: profile picture, launches, campaign covers |
| Lime on ink | `logo/saneee-wordmark-lime.svg`, `sigil/saneee-sigil-lime.svg` | Rare accent moments: the website footer, a single hero frame |

Never put the logo in lime on paper, or in grey on anything. Both are too low in contrast.

## Files

```
assets/logo/
  saneee-wordmark-ink.svg        transparent, ink
  saneee-wordmark-paper.svg      transparent, paper
  saneee-wordmark-lime.svg       transparent, lime
  saneee-wordmark-on-ink.svg     with ink background
  saneee-wordmark-on-paper.svg   with paper background
  saneee-wordmark-on-lime.svg    with lime background
assets/sigil/
  saneee-sigil-ink.svg / -paper.svg / -lime.svg     transparent
  saneee-sigil-on-lime.svg / -on-ink.svg / -on-paper.svg   square tiles
assets/png/
  saneee-sigil-on-lime-1080.png     Instagram profile picture
  saneee-sigil-on-{param,teesha,hardik,smit}-1080.png   each member's accent tile, for their own profiles and posts
  saneee-sigil-on-lime-512.png      small avatars (WhatsApp, Google)
  saneee-sigil-on-ink-1080.png, saneee-sigil-on-paper-1080.png
  saneee-sigil-*-transparent-1024.png
  saneee-wordmark-on-*-2048.png, saneee-wordmark-*-transparent-2048.png
```

Use the SVGs wherever the tool accepts them (Figma, Canva, the website). Use the PNGs for Instagram, WhatsApp, Meta Ads Manager and anywhere else that only takes images.

## Clear space

Leave at least the **height of the lowercase e** empty on every side of the wordmark. For the sigil, leave the width of the arrow. Give it more room when the layout allows.

## Placement

- **Posts and slides:** bottom-left or bottom-centre, at about 12–18% of the frame width. The sigil goes in a corner at about 6–8% of the frame width.
- **Reels:** the full wordmark on the end card only. Inside the video, use a small sigil in a top corner, clear of Instagram's interface (see [SOCIAL.md](SOCIAL.md)).
- **Website header:** the wordmark, 28–40px tall.

## Don't

- Don't retype the logo in any font, not even Saneee Brand. Always use the artwork.
- Don't stretch, squash, skew, rotate or letter-space it.
- Don't move, resize or remove the arrow. Don't swap it for an emoji or an icon.
- Don't add shadows, glows, outlines, gradients or 3D effects.
- Don't recolour single letters, or use any colour outside the palette.
- Don't place it over a busy photo. If you must, put it on a solid ink or paper panel.
- Don't lock it up with other words, except for the tagline below it with the clear space kept.

## Motion

The site's hero morphs the word SANEEE into the sigil, with the arrow landing last. For reels and intros, use the same move: the type settles, then the cursor clicks into place. Keep it to 1.5–3 seconds. The original animation files are in `Z:\saneee.in\logo\` (`animatedLOGO*.mp4`).
