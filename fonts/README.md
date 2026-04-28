# Fonts

The PETAL Insights design system uses three Google Fonts. They are loaded via Google Fonts CDN rather than self-hosted, so this directory does not contain font files.

## The three families

### Cormorant Garamond
- **Role:** Display, headlines, editorial emphasis, key insight statements
- **Source:** [Google Fonts — Cormorant Garamond](https://fonts.google.com/specimen/Cormorant+Garamond)
- **Designer:** Christian Thalmann (Catharsis Fonts)
- **License:** [SIL Open Font License 1.1](https://scripts.sil.org/OFL)
- **Weights used:** 300, 400, 600 (regular and italic)

### Outfit
- **Role:** Body copy, descriptions, UI text
- **Source:** [Google Fonts — Outfit](https://fonts.google.com/specimen/Outfit)
- **Designer:** Smith Gilliam, Rodrigo Fuenzalida
- **License:** [SIL Open Font License 1.1](https://scripts.sil.org/OFL)
- **Weights used:** 200, 300, 400, 500

### DM Mono
- **Role:** Small caps tags, section labels, technical annotations
- **Source:** [Google Fonts — DM Mono](https://fonts.google.com/specimen/DM+Mono)
- **Designer:** Colophon Foundry, Jonny Pinhorn
- **License:** [SIL Open Font License 1.1](https://scripts.sil.org/OFL)
- **Weights used:** 300, 400

All three are open source under the SIL Open Font License, free for commercial use.

## Loading them

### Single import URL (recommended)

```html
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=DM+Mono:wght@300;400&family=Outfit:wght@200;300;400;500&display=swap" rel="stylesheet">
```

Or in CSS:

```css
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=DM+Mono:wght@300;400&family=Outfit:wght@200;300;400;500&display=swap');
```

This URL is also stored as a token in `tokens/typography.json` under `font.google-fonts-import-url`.

### Self-hosting

If self-hosting is required (CDN-blocked environment, offline use, performance optimisation), download the WOFF2 files from [google-webfonts-helper](https://gwfh.mranftl.com/fonts) and reference them locally:

```css
@font-face {
  font-family: 'Cormorant Garamond';
  font-weight: 600;
  font-style: normal;
  src: url('/fonts/cormorant-garamond-600.woff2') format('woff2');
  font-display: swap;
}
/* repeat for each weight/style combination used */
```

The license permits self-hosting and redistribution under SIL OFL terms.

## Why these three

The pairing was chosen for editorial register, not technical optimisation. Cormorant Garamond carries the longform-magazine authority of a Garamond revival without the dryness of older serif faces. Outfit is geometric enough to feel modern but not so geometric that it reads as tech-startup. DM Mono provides the editorial-system signal — the publication-with-a-system look — without the heaviness of older monospaced faces like Courier.

The combination is intentionally restrained. Most PETAL compositions use only two of the three at a time (Cormorant + DM Mono for static graphics; Outfit + DM Mono for interactive UIs; Cormorant + Outfit for long-form layouts).

If extending this system to new contexts, stay within these three. Adding a fourth family weakens the system signature.
