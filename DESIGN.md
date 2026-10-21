---
name: D&J Construction
description: Calm slate-and-sand bands for a Leamington bathroom renovation crew.
colors:
  paper: "#f3f5f7"
  card: "#ffffff"
  field: "#e2e6eb"
  ink: "#232a2f"
  body: "#323b41"
  soft: "#566069"
  navy: "#3a4751"
  deep: "#2e373c"
  on-dark: "#f6f4f0"
  on-dark-soft: "#d3d8dc"
  sand: "#d6b48e"
  sand-2: "#e2c6a5"
  sand-ink: "#7a5432"
  line: "rgba(35,42,47,.12)"
  focus: "#2d5c85"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(20px, 5.6vw, 26px)"
    fontWeight: 400
    lineHeight: 1.15
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(18px, 4.6vw, 20px)"
    fontWeight: 400
    lineHeight: 1.5
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "12px"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "0.06em"
  eyebrow:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: "0.02em"
rounded:
  field: "10px"
  card: "24px"
  pill: "999px"
spacing:
  gutter-phone: "20px"
  gutter-desktop: "40px"
  section-phone: "64px"
  section-desktop: "96px"
  container: "1160px"
components:
  button-primary:
    backgroundColor: "{colors.sand}"
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.sand-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  input-text:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  eyebrow:
    textColor: "{colors.ink}"
    typography: "{typography.eyebrow}"
    rounded: "{rounded.pill}"
    padding: "9px 14px"
  step-number:
    backgroundColor: "{colors.sand}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "48px"
  float-circle:
    backgroundColor: "{colors.sand}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "60px"
---

# Design System: D&J Construction

## Overview

**Creative North Star: "The Slate Badge, Laid Out Flat"**

The system takes the D&J badge (white on charcoal slate) and the flyer's warm sand and spreads them across full-bleed bands that alternate light and dark, so every new section reads as a new room. It is an instance of Ellie's calm band house default (pitch-site, 2026-10-19): cool paper, two slates, one warm accent used as a fill, a single display webfont, soft borderless shapes, and motion limited to a hero headline bounce-in, a quiet fade-up, and a floating text circle.

Density is low and phone-first. One column on phones, two at 1024px and up; headlines are short and set large; lists are hairline-divided rows rather than card grids. Depth comes from band contrast and a faint diagonal line texture on the darkest slate, not from stacked shadows. The hero is a photograph of a finished bathroom under a slate overlay, so the photo reads as slate-toned and the copy sits on it at full contrast.

The page speaks as the crew, plainly. The visual system matches: no ornament beyond the texture and the sand accents, every control is a big rounded shape, and the accent appears where an action or a landing word is.

**Key Characteristics:**
- Full-bleed bands: paper, mid slate, deep slate with diagonal texture, alternating.
- One accent, sand, as a fill; a darker sand-ink when it must be text on light.
- Cal Sans for every heading, button label and list title; system sans for running text.
- Pills and circles for every control; 24px card, 10px field, no borders at rest.
- Each heading ends on an accent phrase.
- Motion: H1 letter bounce-in, a 12px fade-up below the fold, a floating text circle.

## Colors

Cool, quiet slates carry the page; a single warm sand does all the signalling.

### Primary
- **Flyer Sand** (sand): the one accent. Fills only: primary buttons, step-number discs, the floating text circle, service-row arrows on hover, the eyebrow dot, text selection. On dark bands it is also the colour of the accent phrase and the row tag (4.9:1 on mid slate, 6.2:1 on deep slate). Text on sand is always ink (7.5:1).
- **Warm Sand Lift** (sand-2): primary button hover only.
- **Sand Ink** (sand-ink): sand as text or line icon on light grounds: accent phrases on paper, claim icons, the header phone glyph, header number hover (6.1:1 on paper).

### Secondary
- **Badge Slate** (deep): the logo's charcoal. Hero ground under the photo, the How it works band and the footer, always carrying the diagonal texture.
- **Mid Slate** (navy): the services band and the closing call band. Flat, no texture.

### Neutral
- **Cool Paper** (paper): page ground, header, and the light bands. Never replaced by black or warm cream.
- **Card White** (card): the quote form card and the Facebook row.
- **Field Grey** (field): input and unselected chip fill on the white card.
- **Slate Ink** (ink): headings, labels, text on sand, selected chip fill.
- **Body Slate** (body): running text on light (10.5:1).
- **Soft Slate** (soft): ledes, help text and the brand subline on light (5.9:1).
- **Warm Off-White** (on-dark): headings, row titles and link text on slate bands.
- **Mist** (on-dark-soft): running text on slate bands (6.7:1 on mid slate).
- **Hairline** (line): 1px dividers between claim rows on paper. On slate bands the divider is white at 12%.
- **Focus Blue** (focus): hover and focus outline for form controls and the focus ring on light grounds; caret colour. Deliberately not sand, so focus never reads as a filled button.
- **Error Red** (error): inline error text and the error border.

### Named Rules
**The Sand Is a Fill Rule.** Sand never sets text on a light ground (1.8:1 on paper). On light, use sand-ink; on sand, use ink.

**The One Warm Colour Rule.** Sand is the only warm hue in the system. Everything else is a cool slate or neutral. A second accent breaks the badge.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** system sans (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** Cal Sans is rounded, wide and friendly, the voice of a crew that answers its phone; the system body keeps running text native and fast on phones inside Facebook's in-app browser.

### Hierarchy
- **Display** (400, clamp 42-80px, 1.02): hero H1 only, white, max 11ch, light text-shadow over the photo.
- **Headline** (400, clamp 30-48px, 1.08, -0.005em, balanced wrap): section H2s.
- **Title** (400, clamp 20-26px, 1.15): claim rows, service row names, step titles, the Facebook row label. Also the button and header-number face at 18-20px.
- **Big number** (400, clamp 30-52px, 1): the closing band's tap-to-call number only.
- **Lede** (400, clamp 18-20px, 1.5): one sentence under a section heading, max 40ch; the hero promise at max 34ch.
- **Body** (400, 16px, 1.7): everything else. Inputs are 16px so iOS does not zoom.
- **Label** (600, 12px, 0.06em, uppercase): the brand subline and the "Our specialty" row tag. Nowhere else.
- **Eyebrow** (500, 14px, 0.02em, sentence case): eyebrow pills only (see Components).

### Named Rules
**The Display Does the Talking Rule.** Cal Sans sets every heading, every button label, every list title and every phone number. The system face never sets a heading; Cal Sans never sets a paragraph.

**The Accent Phrase Rule.** Every H1 and H2 ends on its last word or phrase in the accent: sand on slate and over the hero, sand-ink on paper. The build applies it on light bands too, which widens the house default (dark bands only).

## Layout

A single centred container (max 1160px) with a 20px gutter on phones and 40px from 760px. Bands are full-bleed; content inside them is not. Section padding is 64px on phones and 96px from 760px.

- **Phones (default):** one column. Hero buttons stack full width. The hero photo crops to a portrait source with the subject right of centre.
- **760px:** larger header (80px tall, 52px badge), wider gutter, taller hero (120px top, 136px bottom padding), hero buttons side by side at min 220px, hero overlay switches from a vertical wash to a left-to-right fade that clears the right of the photo.
- **1024px:** two-column splits (copy left, list right, 64px column gap); service rows go two-up (56px gap); the form sits beside a sticky heading block (1fr / 1.2fr); steps go three-up; the closing band puts the big number on the right, bottom-aligned.
- Small-phone tweaks at 429px and 374px shrink the wordmark and hide the subline and phone glyph rather than wrapping.

Headings sit in a left-aligned block (max 640px, 16px internal gap). Nothing is centred. Lists are separated by hairlines, not gaps between cards. Every tap target is 44px or larger; buttons are 56px, chips 48px.

**The Bands Alternate Rule.** Adjacent sections never share a ground. Order in the build: hero (deep), paper, mid slate, deep (textured), paper, mid slate, footer (deep, textured).

## Elevation & Depth

Depth comes from band contrast and texture. Shadows exist only as soft, low-opacity ambient lift on the few white objects that sit on paper, and on the floating circle that sits over everything.

### Shadow Vocabulary
- **Card lift** (`box-shadow: 0 10px 30px rgba(35,42,47,.06)`, and `0 8px 24px rgba(35,42,47,.07)` on the Facebook row): white objects on paper.
- **Float lift** (`box-shadow: 0 10px 28px rgba(20,26,30,.3)`): the floating text circle only, because it overlaps content.

### Texture
- **Diagonal band texture** (`repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`): on deep-slate bands and the footer only, never on the mid slate or on light grounds. Kept at 3.5% white so it never reads as lines through text.

### Named Rules
**The Texture Lives on Deep Slate Rule.** The diagonal lines belong to the badge's charcoal and nowhere else. Never raise its opacity above about 4%.

**The Ambient Only Rule.** Shadows are wide, soft and slate-tinted. No hard or offset shadows; no shadows on buttons, chips, rows or eyebrows.

## Shapes

Soft and borderless. Three radii: 24px for cards (the form; the Facebook row uses 20px), 10px for fields, and full pill or circle for every control, disc and badge. Borders are absent at rest; a 2px transparent border is reserved on buttons, inputs and chips so hover and focus can colour it without layout shift. The round badge, the step discs, the arrow circles and the floating circle make the circle a recurring motif.

## Components

### Buttons
Big, round, unmistakable.
- **Shape:** full pill (999px), 56px tall, 26px side padding, Cal Sans 18px, optional 20px line icon before the label.
- **Primary:** sand fill, ink text. Used for "Get a quote" and the form submit (full width in the form).
- **Ghost:** transparent with a 2px warm off-white border at 75%; only on slate or over the hero. Hover: solid white border and a 10% white wash.
- **Hover / Focus:** primary lifts to sand-2. Press scales to 0.98 over 120ms. Hover styles apply only under `(hover:hover)`. Focus is a 3px outline offset 3px: focus blue on light, sand on slate.
- At most two buttons together (hero only): one primary, one ghost.

### Chips
- **Style:** pill, 48px tall, field-grey fill, ink text, 16px system face. They are visually hidden radio inputs with labels.
- **State:** selected is an ink fill with white text. Hover colours the reserved border focus blue; keyboard focus is an outline with a 2px offset so it stays visible on the ink fill.
- Tapping a service row pre-selects the matching chip.

### Cards / Containers
- **Corner Style:** 24px.
- **Background:** card white on paper.
- **Shadow Strategy:** card lift (see Elevation).
- **Border:** none.
- **Internal Padding:** clamp(20px, 5vw, 32px), 22px between fields.
- Only the quote form is a card. Lists are rows, not cards.

### Inputs / Fields
- **Style:** field-grey fill, no visible border at rest, 10px radius, 52px tall (textarea 120px, vertical resize), 16px system face, ink text. Labels and legends are Cal Sans 18px in ink; "(optional)" is 14px soft.
- **Focus:** the 2px border turns focus blue; hover does the same on pointer devices.
- **Error:** a plain-sentence error line in error red below the field, and an error-red border that holds through focus.

### Navigation
- **Header:** paper, wordmark left (round badge, Cal Sans name, uppercase label subline), tap-to-call number right in Cal Sans with a sand-ink phone glyph. No menu. Not sticky.
- **Footer:** deep slate with texture; badge, name, area, phone, email and Facebook as 44px-tall links in warm off-white, hovering to sand.

### Service Rows
Each row is the whole link: Cal Sans title, a 16px Mist description, and a 44px arrow circle at 10% white. Only the arrow changes on hover or focus, filling with sand. Rows are divided by 12% white hairlines. One row may carry an uppercase sand label tag ("Our specialty").

### Claim Rows
On paper: a 40px sand-ink line icon (stroke 2.4, round caps) beside a Cal Sans title, divided by hairlines. Not links, no arrows.

### Numbered Steps
A 48px sand disc with a Cal Sans counter, beside a title and a one-line body. Three-up from 1024px.

### Link Row (Facebook)
A white 20px-radius row on paper with a label and the same 44px arrow circle (7% ink), which fills with sand on hover.

### Eyebrow Pill (owner-approved exception)
A small label above the hero H1 and a few section headings, never every one (three in this build, out of six headings). 14px system face, sentence case, a 7px sand dot, and a pill at 6% ink on light or 12% white on slate. It is a label, not a heading and not a button: no arrow, no hover, no shadow, never a full sand fill. Ellie chose this deliberately on 2026-10-19 (calm band house default), knowing Impeccable's craft floor flags eyebrows; it is recorded here as her exception, not as a general licence for kickers.

### Floating Text Circle
One 60px sand circle, bottom right, with a chat glyph, opening a pre-filled `sms:`. It slides up from 120px below over 350ms (`cubic-bezier(.2,.8,.2,1)`) once the hero has scrolled away, and hides while the quote form is on screen. When hidden it is removed from the tab order and from the accessibility tree. One circle only; never a bottom bar.

### Hero
A finished-bathroom photo (`object-fit: cover`) under a slate overlay (80-92% on phones top to bottom; 92% left fading to 20% right from 760px). It holds an eyebrow, the H1, one promise line and at most two buttons. No call button in the hero; the number lives in the header.

### Motion
- **H1 bounce-in:** hero H1 only. JS splits it into letters inside no-wrap word spans; each letter enters from 50px right and transparent over 1s on `cubic-bezier(.34,1.56,.64,1)` (the overshoot is the bounce), 20ms apart. It waits for Cal Sans (max 600ms), then restores the plain heading on the last `animationend`. Skipped without JS and under reduced motion.
- **Fade-up:** elements marked to rise that start below the first screen move up 12px and fade in over 400ms ease-out on entry. Everything is visible at rest, without JS, and under reduced motion.
- **State transitions:** 150-200ms colour and border changes; 120ms press scale.

## Do's and Don'ts

### Do:
- **Do** alternate full-bleed bands so neighbouring sections never share a ground.
- **Do** use sand only as a fill, with ink text on it; switch to sand-ink for sand-coloured text on light.
- **Do** end each H1 and H2 on an accent phrase (sand on slate, sand-ink on paper).
- **Do** set every heading, button label, list title and phone number in Cal Sans 400; keep running text in the system face at 16px / 1.7.
- **Do** make every control a pill or circle, at least 44px tall (buttons 56px, chips 48px).
- **Do** use focus blue for form hover and focus, and sand for focus rings on slate.
- **Do** keep the fade-up content visible at rest and honour reduced motion everywhere.
- **Do** make a list row the whole link and let only its arrow circle change.

### Don't:
- **Don't** set sand text on paper or white (1.8:1).
- **Don't** add a second accent colour or warm the neutrals.
- **Don't** put the diagonal texture on the mid slate or on light bands, or push it above about 4% white.
- **Don't** apply the letter bounce-in to any heading other than the hero H1.
- **Don't** give an eyebrow pill a hover state, arrow, shadow or solid sand fill, or put one above every heading.
- **Don't** use hard or offset shadows, or shadows on buttons, chips and rows.
- **Don't** replace the floating circle with a bottom bar or show it alongside the form.
- **Don't** rely on the field-grey fill alone to outline a field on white (1.25:1); the label and, on interaction, the focus-blue border carry it.
