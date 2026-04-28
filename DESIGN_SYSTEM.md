# PETAL Insights — Visual Design System

**Version 1.0 · April 2026**
**For:** CNS (citynewsservice.cn) · Shanghai Chest Hospital · PETAL Insights series

---

## About this document

This is the canonical visual identity reference for the PETAL Insights series, a sponsored health journalism series produced by CNS in partnership with Shanghai Chest Hospital. The series covers thrombosis prevention and treatment in five sessions: Prevention, Early Screening, Treatment, Rehabilitation, and Long-term follow-up.

The visual system covers three production contexts: in-article interactive HTML/SVG embeds on CNS, static graphics for the CNS web article body, and static graphics for WeChat distribution. All three share a unified visual language so the series feels coherent across surfaces.

This document is portable. It can be shared across LLM sessions, given to designers, or used as a project-level design system in Claude Design. It contains exact color tokens, typography specifications, composition principles, and reference examples sufficient to produce on-brand assets without prior context.

---

## 1. Visual identity in one sentence

> Modern, cosmopolitan, night mode editorial — the aesthetic of a thoughtful longform health publication, not a hospital brochure.

If you take nothing else from this document: dark backgrounds, restrained warm gold as the primary accent, cream-white for high-emphasis elements, and a single muted clinical red used sparingly for alert states. Never bright, never saturated, never clinical-marketing in tone.

---

## 2. Color system

### Background tokens

| Token | Hex | Usage |
|---|---|---|
| `--bg` | `#070c11` | Primary background, near-black with a faint blue-black undertone |
| `--surface` | `#0d1419` | Card surfaces, panels, secondary containers |
| `--border` | `rgba(255,255,255,0.08)` | All dividers, panel borders, hairlines |

Backgrounds typically use a subtle gradient from `#070c11` (top-left) to `#0d1419` (bottom-right) with optional radial accent glows at low opacity (gold in one corner, red in the opposite corner, both at 4–8% opacity). The grain should be imperceptible — atmosphere, not texture.

### Accent tokens

| Token | Hex | Usage |
|---|---|---|
| `--accent` | `#c8a96e` | Primary warm gold — section labels, mono tags, vessel mid-state, key UI elements |
| `--contrast` | `#f4e8c8` | Cream-gold for peak/high-emphasis states (bright contrast-filled vessels, etc.) |
| `--vessel` | `rgba(242,244,247,0.18)` | Muted inactive grey for ghost/baseline elements |
| `--clot` / `--alert` | `#e05c5c` | Muted clinical red — used ONLY for alert states, filling defects, risk indicators |

The red is critical. It must be the desaturated `#e05c5c`, never a bright medical red, never a fire-engine red. It carries weight precisely because it's quiet.

### Text tokens

| Token | Hex / RGBA | Usage |
|---|---|---|
| `--text` | `#f2f4f7` | Primary text, off-white not pure white |
| `--text-dim` | `rgba(242,244,247,0.72)` | Body copy, descriptions, secondary text |
| `--text-muted` | `rgba(242,244,247,0.42)` | Tertiary text, timestamps, minor labels |

### Color usage rules

1. **One red per composition.** The clinical red is reserved for the single critical alert moment (the clot, the filling defect, the high-risk indicator). Multiple red elements in one frame dilutes the signal.
2. **Gold is the workhorse.** Section tags, mono labels, vessel highlights, accent borders, and decorative line work all use the gold. It's the primary "this is PETAL" color.
3. **Cream is for the moment of revelation.** Reserve cream-white (`#f4e8c8`) for the peak emphasis state — fully contrast-filled vessels at peak enhancement, the brightest element in the frame. It should appear at one or two points only.
4. **No saturated colors anywhere.** No pure red, pure blue, pure green. The palette lives in a narrow tonal range and gets its sophistication from restraint, not range.
5. **Backgrounds are layered, not flat.** Always include subtle gradient + corner accent glows. Pure flat black reads as cheap.

---

## 3. Typography

### Font families

```
Display & headlines: Cormorant Garamond
  Source: Google Fonts
  Weights used: 300, 400, 600
  Italics used: 300, 400 (italic variants)

Body & UI: Outfit
  Source: Google Fonts
  Weights used: 200, 300, 400, 500
  Lowest weight (200) for very large display only

Monospace tags & labels: DM Mono
  Source: Google Fonts
  Weights used: 300, 400
```

### Typographic principles

**Cormorant Garamond does the editorial heavy lifting.** Headlines, stage titles, key insight callouts, pull quotes — all in Cormorant. Use the italic variant for emphasis words within a headline. The classic move is mixing regular and italic in a single line: *"Catching a* pulmonary embolism *in four stages."* This creates editorial rhythm and signals that this is content, not interface.

**Outfit handles everything else.** Body copy, descriptions, captions, footers. Default weight is 300 (light). Body copy is rarely heavier than 400. The lightness reinforces the editorial register.

**DM Mono is for the hardware aesthetic.** Section tags, stage indicators, timestamps, technical labels. Always uppercase. Always letter-spaced (0.15em to 0.2em). Always small (8–13px depending on context). DM Mono is what makes the design feel like a publication with a system, not just nice editorial type.

### Type pairings to use

```
Stage tag (DM Mono, 12px, gold, letter-spaced 3em)
Headline (Cormorant Garamond, 28–68px, 600 weight, mix of regular + italic)
Body (Outfit, 14–18px, 300 weight, dim white)
```

### Type pairings to avoid

- Cormorant in body copy — it's a display face
- Outfit at heavy weights — defeats the editorial register
- Bold italic anything — too theatrical
- All-caps headlines — DM Mono handles caps; let Cormorant breathe in mixed case
- Underlined text — never

### Sizing reference

For a 1080-wide vertical WeChat graphic:

```
Series tag (DM Mono):       16px, 0.25em letter-spacing
Section label (DM Mono):    12–13px, 0.2em letter-spacing
Display headline:           60–78px, Cormorant 600
Subhead:                    22–28px, Cormorant or Outfit
Stage title:                24–30px, Cormorant 600
Body / description:         15–18px, Outfit 300
Italic caption:             18–22px, Cormorant italic
Footer / disclaimer:        11–15px, Outfit 300
```

For an 800×600 in-article interactive:

```
Series tag:                 9–10px DM Mono
Stage label:                9px DM Mono
Stage title (in panel):     20–24px Cormorant 600
Stage description:          11–13px Outfit 300
Key fact text:              11px Outfit 400
Button label:               9px DM Mono uppercase
```

---

## 4. Composition and layout principles

### The breath rule

Generous negative space at all times. Margins should feel slightly larger than expected. Information density is achieved through hierarchy and typography, not by filling the frame. If a composition feels crowded, the answer is almost always "remove something" rather than "shrink everything."

### The discovery rule

The most important element in any composition should be **discovered, not announced.** No giant arrows pointing at the clot. No "LOOK HERE" callouts. Position the critical element slightly off-center, give it subtle visual weight (a faint pulse ring, a small color shift), and trust the reader's eye to find it after a beat.

### The single-payoff rule

Each graphic carries one editorial idea. The hero shows the four stages of a CTPA. The filling-defect explainer shows what a filling defect is. The diagnostic funnel shows the diagnostic sequence. Don't compound ideas — make multiple graphics if there are multiple ideas.

### Grid behaviour

For multi-panel compositions (like the four-stage hero), use a 2×2 grid with consistent panel proportions and identical internal margins. Each panel is a small composition that follows the same rules — same typography hierarchy, same negative space, same color logic.

### Annotation style

When labels are necessary (e.g., pointing to a filling defect):

- Thin 1px pointer line in the gold accent color (or red if marking an alert element)
- Small DM Mono label, uppercase, letter-spaced 0.15–0.2em, gold (or red)
- Small dot or short serif at the pointer origin
- Never use arrows; use unstyled lines that terminate flush with the labelled element
- Position labels in the negative space, never overlapping other content

This produces a "subtle radiology annotation" feel rather than a "textbook diagram" feel.

### Frame elements

Every composition typically includes:

```
Top:    Series tag (left, gold mono) + Section context (right, dim mono)
        Hairline divider below
Body:   The actual editorial composition
Bottom: One or two lines of editorial summary copy + Branding tag (gold mono)
```

This frame is the system signature. It's how the series is recognised at a glance.

---

## 5. Iconography and visual elements

### Vessel rendering

When depicting blood vessels (which happens often in this series):

- Soft-edged strokes, not hard lines
- `stroke-linecap="round"` always
- Width tapers from main trunk (6–8px) to lobar (5px) to segmental (3px) to subsegmental (2px)
- Pre-contrast state: `--vessel` muted grey
- Mid-injection state: `--accent` gold at 30–50% opacity
- Peak state: `--contrast` cream-white
- Use a subtle bloom/glow effect on the contrast state — vessels should feel like they're radiating, not drawn

### The filling defect

The visual signature of the CTPA chapter, but applicable across the series wherever a "block" or "interruption" is depicted:

- A small dark ellipse interrupting an otherwise-bright vessel
- Single concentric pulse ring around it (in red), subtle
- Optional small solid red dot at the center
- Total opacity of red elements never exceeds ~60%

### Reticle lines

Dashed lines (1–2px stroke, `stroke-dasharray="2,4"` or similar) at low opacity (40–50%) suggesting scanner/instrument geometry. Use sparingly — at most one horizontal + one vertical, intersecting near the focal point. They should feel structural, not decorative.

### Pulse rings

For elements that need visual emphasis (active risk factors, focal points):

```
Outer ring: 1.5px stroke, 60% opacity, expanding via animation in interactives
Static use: single ring, no animation, 40–60% opacity
```

### What to avoid in iconography

- No drop shadows
- No glossy/3D effects
- No gradient fills inside shapes (gradients are for backgrounds only)
- No emoji or pictographic icons
- No medical clip-art style diagrams (organs as flat illustrations with dark outlines)
- No flowchart-style boxes with arrows (use the 01/02/03 numbered card system instead)

---

## 6. Tone and editorial register

The visual design has to match the writing voice, which is:

- Informative and slightly wry
- Confident but not breathless
- Specific and grounded, not abstract or aspirational
- Quietly authoritative, not theatrical

In design terms this translates to:

- Restraint over dramatic emphasis
- Specificity over generic medical imagery
- Editorial register over marketing register
- One idea per composition over information density
- Atmosphere over decoration

If a design feels like it belongs in a hospital waiting room, on a pharmaceutical brochure, in a health-app onboarding flow, or in a generic "AI healthcare" stock photo, it's wrong. If it feels like it could open a *Wired* health feature, an *Atlantic* science piece, or a longform Sunday magazine essay, it's right.

---

## 7. Production formats

### In-article interactive (CNS)

- Internal canvas: 800 × 600 pixels (fixed)
- Wrapped in `.scaler` div with JS scaleToFit logic
- Embedded via iframe at width=100% height=600
- Hosted on GitHub Pages, single `index.html` file
- Must handle CNS CMS height-stripping behavior

### CNS desktop hero (article header)

- 16:9 horizontal, 1600 × 900px minimum
- Full-bleed within article column
- Dark composition that doesn't fight the article body background

### WeChat hero (mobile vertical)

- 3:4 vertical, 1080 × 1440px
- Optimised for mobile column display and share-card thumbnail
- Must read clearly at small sizes — type hierarchy matters more here than in horizontal formats

### WeChat in-article graphics

- 3:4 vertical or square (1:1), 1080px wide
- Compositions that work standalone (since WeChat sharing strips context)
- Each graphic should carry the series tag and CNS branding so the source is always clear

---

## 8. Reference examples

The following compositions have been produced and serve as the canonical reference for the visual system. New work should feel like it belongs in this set.

### Session 1 — Virchow's Triad interactive

Three toggleable risk factors arranged as a triangle, with a central risk indicator that escalates from 0/3 (gold accent) through 3/3 (red alert) as factors are activated. Establishes the palette, the gold→red escalation, the pulse-ring motif, and the triangular composition principle.

### Session 2 — Four-stage CTPA walkthrough (interactive)

Linear progression through four discrete states: pre-contrast → injection → peak → diagnosis. Demonstrates the vessel rendering system, the gold/cream/red color escalation, and the alert-state frame treatment (red border + red label) for the diagnostic moment.

### Session 2 — WeChat hero "Catching a pulmonary embolism in four stages"

Vertical 1080×1440 composition with display headline using mixed Cormorant regular + italic ("Catching a" / *pulmonary embolism* / "in four stages"), 2×2 grid of stage panels below. Reference for how the four-stage system translates from interactive to static.

### Session 2 — WeChat "What is a filling defect?"

Two-element comparison composition (normal vessel above, blocked vessel below) with a "vs" pivot. Reference for explainer-style editorial graphics that compare two states, with the key insight delivered in a gold-bordered callout card at the bottom.

### Session 2 — WeChat "From suspicion to proof" diagnostic funnel

Vertical four-stage funnel with numbered cards (01 through 04), the final stage marked in red as the gold standard. Reference for how to depict sequential medical processes without resorting to flowchart aesthetics.

---

## 9. Quick reference for AI tools and designers

If feeding this system into Claude Design, Figma AI, Midjourney, or any generative tool, the following compressed brief captures the essentials:

> **Style:** Modern editorial dark mode, atmospheric and restrained. Aesthetic of a longform health publication, not a hospital brochure.
>
> **Background:** Deep near-black blue-black (#070c11 to #0d1419) with subtle gradient and very faint corner accent glows.
>
> **Primary accent:** Warm gold (#c8a96e) for headers, labels, and main accent color.
>
> **High-emphasis:** Cream-gold (#f4e8c8) for peak/critical bright elements.
>
> **Alert color:** Muted clinical red (#e05c5c), used sparingly on a single alert element only.
>
> **Typography:** Cormorant Garamond (display, mix regular + italic), Outfit (body, light weight), DM Mono (small caps tags).
>
> **Composition:** Generous negative space. One editorial idea per graphic. Critical elements discovered, not announced. Subtle radiology-style annotations, not textbook arrows.
>
> **Avoid:** Saturated colors, photorealism, drop shadows, glossy/3D effects, AI-medical tropes (glowing brains, holographic scans), pharmaceutical-marketing aesthetics, textbook diagrams, flowchart boxes, generic stock medical imagery.
>
> **Test:** If it could open a Wired health feature or an Atlantic science piece, it works. If it could appear in a hospital waiting room or a pharma brochure, it doesn't.

---

## 10. Versioning and maintenance

This document represents the visual system as established through Sessions 1 and 2 of the PETAL Insights series. As future sessions are produced, new component patterns, motifs, or refinements should be added here rather than reinvented. The principle is consistency above novelty — every new asset should feel like part of the same series.

Changes that warrant a version bump:

- New color tokens added to the palette
- Significant new composition pattern that recurs across multiple assets
- Change to the typographic system

Changes that don't:

- Individual creative compositions for new article topics
- Minor adjustments to existing patterns
- New annotation labels or content variations

---

*This visual system is supported by the Shanghai Health Science Communication Talent Development Program (JKKPYL-2024-B07).*

*PETAL Insights · CNS (citynewsservice.cn) · Shanghai Chest Hospital*
