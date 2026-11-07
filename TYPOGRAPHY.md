# Typography

**One custom face, one serif.** Make variety through size, line breaks and space, not by adding fonts.

## The fonts

| Role | Font | Where it's used | Get it |
|---|---|---|---|
| **Brand** | **Saneee Brand** Regular | Headlines, nav, buttons, labels, numbers, section titles | `assets/fonts/saneee-brand-regular.otf` (install on desktop, Figma, Canva) and `.woff2` (web) |
| **Voice** | **Instrument Serif** Italic | Taglines, service voice lines, pull quotes, one-line editorial moments | [Google Fonts](https://fonts.google.com/specimen/Instrument+Serif) |
| **Text** | **Instrument Sans** 400 / 500 | Paragraphs, forms, long captions inside designs | [Google Fonts](https://fonts.google.com/specimen/Instrument+Sans) |

Notes:
- Saneee Brand has **one weight (Regular)**. Never fake bold with strokes or a "bold" button. To add emphasis, use size, lime, or a switch to the serif.
- Instrument Serif is a stand-in for **Voyage**, the planned licensed serif. When Voyage arrives, it replaces Instrument Serif in the same roles.
- Instrument Sans is temporary, until Saneee Brand has a text weight. Keep it out of headlines.
- In Canva, upload the `.otf` as a brand font (Canva Pro: Brand Kit → Fonts → Upload).

## Characters Saneee Brand has

```
A–Z  a–z  0–9
! " # % & ' ( ) + , - . / : ; ? @
– — ‘ ’ “ ”  ← → ↗
```

**It does not have:** `₹ $ € * = < > [ ] _ · • ™ ©` or accented letters.
- Set prices like **₹18,000** with the ₹ in Instrument Sans, or write "Rs" or "INR".
- Use `/` or `—` as separators in Saneee Brand. Only use `·` in serif or sans text.
- The ® in the logo is part of the artwork, not the font.

## Scale

The website scale. The first number in each range is for phones, the last for large screens.

| Token | Size | Leading | Font | Use |
|---|---|---|---|---|
| `display-lg` | 48 → 112px | 1.0 | Brand | Hero statements |
| `h1` | 44 → 88px | 1.12 | Brand | Page titles |
| `h2` | 34 → 64px | 1.12 | Brand | Section titles |
| `h3` | 26 → 44px | 1.12 | Brand | Sub-sections, card titles |
| `h4` | 20 → 28px | 1.12 | Brand | Small headings |
| `voice` | 21 → 27px | 1.2 | Serif italic | Voice lines |
| `editorial` | 38 → 96px | 1.02, −0.015em | Serif italic | Big editorial line |
| `body-lg` | 18 → 20px | 1.65 | Sans | Intros |
| `body` | 17px | 1.65 | Sans | Paragraphs (never under 16px) |
| `label` | 13px | 1.4, +0.08em, CAPS | Brand | Eyebrows, metadata |

### For 1080px social frames

| Element | Size | Font |
|---|---|---|
| Headline | 96–160px, leading 1.0 | Brand |
| Voice line | 56–80px | Serif italic |
| Body | 34–40px, max 3 lines | Sans |
| Label / tag / page number | 26–30px caps, +0.08em | Brand |
| Smallest text allowed | 26px | |

## Pairing

Use one serif phrase, then one brand phrase:

> *Ideas that* **move.**
> *Sanely built.* **Insanely good.**

- Change font at the phrase level, never word by word in a sentence.
- One serif moment per frame or section. If everything is italic, nothing is.
- The serif carries feeling. The brand face carries facts and actions.

## Rules

- Headlines are short (2–8 words) and set in **sentence case** with a full stop: "Tell us what you need."
- Use caps only for labels and tags.
- Keep body text to about 60 characters per line.
- Balance headline line breaks by hand. Don't leave one word alone on the last line.
- No outlines, shadows, gradients on text, or warped text.
