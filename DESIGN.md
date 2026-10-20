---
name: KMD Windows and Doors
description: Calm full-bleed bands in the logo's navy, with the oak of the front door they installed as the one warm accent.
colors:
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  ink: "#0f2147"
  body: "#2a3550"
  soft: "#4b5670"
  navy: "#12306c"
  deep: "#0a1c42"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c9d7ea"
  oak: "#eab04a"
  oak-2: "#f2c26c"
  oak-ink: "#87561a"
  line: "rgba(15,33,71,.12)"
  focus: "#12306c"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 76px)"
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
    fontSize: "clamp(22px, 6vw, 28px)"
    fontWeight: 400
    lineHeight: 1.15
  label:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  eyebrow:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: "0.02em"
  small:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.7
rounded:
  card: "24px"
  facebook-row: "20px"
  ready-box: "16px"
  field: "10px"
  focus: "6px"
  pill: "999px"
  circle: "50%"
spacing:
  gutter-phone: "20px"
  gutter: "40px"
  section-phone: "64px"
  section: "96px"
  column-gap: "64px"
  form-gap: "20px"
  chip-gap: "10px"
  container: "1160px"
components:
  button-primary:
    backgroundColor: "{colors.oak}"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.oak-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-copy:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "48px"
  eyebrow:
    backgroundColor: "rgba(15,33,71,.06)"
    textColor: "{colors.ink}"
    typography: "{typography.eyebrow}"
    rounded: "{rounded.pill}"
    padding: "9px 14px"
  eyebrow-on-dark:
    backgroundColor: "rgba(255,255,255,.12)"
    textColor: "{colors.on-dark}"
  service-row:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    padding: "12px 2px"
    height: "76px"
  service-row-arrow:
    backgroundColor: "rgba(15,33,71,.07)"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "44px"
  service-row-arrow-hover:
    backgroundColor: "{colors.oak}"
    textColor: "{colors.ink}"
  facebook-row:
    backgroundColor: "{colors.card}"
    textColor: "{colors.ink}"
    rounded: "{rounded.facebook-row}"
    padding: "14px 16px 14px 22px"
    height: "76px"
  step-number:
    backgroundColor: "{colors.oak}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "48px"
  work-photo:
    rounded: "{rounded.card}"
    width: "100%"
  form-card:
    backgroundColor: "{colors.card}"
    textColor: "{colors.body}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  input:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  ready-box:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.ready-box}"
    padding: "16px"
  floating-circle:
    backgroundColor: "{colors.oak}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "60px"
---

# Design System: KMD Windows and Doors

## Overview

**Creative North Star: "The Calm Front Door"**

This is Ellie's house calm band style, coloured from KMD's own job. The page is a stack of full-bleed bands that swap between light and dark, so every new section is obvious on a phone: off-white paper, the KMD logo's navy, and a deeper navy carrying a faint diagonal line texture. The one warm colour is the oak of the front door KMD installed. It shows up as a fill on the things you can press or follow (the estimate button, step numbers, the text circle), and as a small dot on each eyebrow.

The mood is calm, open and friendly. Headings are set in Cal Sans: soft geometric shapes at a single weight, sitting on a quiet system body at 16/1.7. Shapes are soft and borderless: 24px cards, pill buttons, tinted fields with no stroke. There is almost no shadow. Depth comes from band contrast and tonal fills, so a white card sits on navy and a pale blue field sits on the white card. The hero is KMD's own house photo under a navy overlay, so the first screen shows their real work.

Motion is short and happens once. The hero headline bounces in letter by letter. Content below the first screen rises 12px as it arrives. A single oak text circle slides up once the hero has gone. Without JS, or with reduced motion, all of it is switched off and the page is complete as it stands.

**Key Characteristics:**
- Full-bleed bands in a fixed order: navy photo hero, paper, deep navy with lines, paper, navy, deep navy footer.
- Oak is a fill with ink text; oak-ink is the only way oak appears as text on a light ground.
- Cal Sans 400 for every heading, button, row title and label; system sans 16/1.7 for reading.
- Soft and borderless: 24px cards, 999px pills, 10px tinted fields, 44px circles.
- Flat, apart from one shadow on the floating circle.
- Three motions (letter bounce-in, 12px rise, circle slide), each one-shot, each off under reduced motion and without JS.

## Colors

Paper, two navies taken from the logo, and one warm oak used as a fill.

### Primary
- **KMD Logo Navy** (navy): The logo's navy. Hero ground under the photo, and the estimate band. It is also the focus colour (focus) for outlines and input borders on light surfaces, so focus never reads as the oak fill.
- **Night Navy** (deep): The darker band, always with the line texture. Used for the work band and the footer.

### Secondary
- **Front Door Oak** (oak): The one warm accent, taken from the installed door. Fills only: the primary button, step numbers, the floating text circle, a hovered or focused service arrow, the eyebrow dot and text selection. Text on oak is always ink (8.1:1). On navy and deep bands, oak is also used as text for a heading's closing phrase (6.5:1 on navy) and as the focus ring.
- **Lit Oak** (oak-2): Hover fill for the primary button. Nothing else uses it.
- **Oak Ink** (oak-ink): Oak used as text or icon on light grounds. The closing phrase of a heading on paper, the header's phone icon, and the phone link on hover (5.75:1 on paper).

### Neutral
- **Cool Paper** (paper): Page ground, header, light bands, the ready box inside the form card, and the browser theme colour.
- **Card White** (card): The estimate form card and the Facebook row.
- **Pale Field** (field): Text inputs and unselected chips on the white card.
- **Navy Ink** (ink): Headings on light, text on oak fills, form labels, selected chip fill.
- **Body Slate** (body): Running text on light (11.3:1 on paper).
- **Soft Slate** (soft): Secondary text: ledes, step descriptions, hints, placeholders, the note under the submit button (6.8:1 on paper).
- **On Dark** (on-dark): Headings, promise text and links on navy and deep.
- **On Dark Soft** (on-dark-soft): Running text on navy (8.6:1) and deep (11.4:1).
- **Hairline** (line): 1px rules above and between service rows.
- **Error Red** (error): Inline validation text and the invalid input border.

### Named Rules
**The Oak Fill Rule.** Oak is a fill with ink text on it. On a light ground, oak used as text or icon is always oak-ink. White on oak and oak on paper are never used.

**The Two Navies Rule.** Navy is for hero and estimate, deep is for work and footer, and deep always carries the line texture. New dark surfaces pick one of the two; there is no third navy.

## Typography

**Display Font:** Cal Sans (self-hosted latin subset, `CalSans-latin.woff2`, preloaded, `font-display: swap`), falling back to Avenir Next, Segoe UI, system-ui
**Body Font:** System sans (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** Cal Sans carries every voice that speaks or acts, from the H1 down to button text and form labels, always at its single 400 weight. The system stack carries everything you read, set generously at 16/1.7. Cal Sans is the house display face in the calm band style. It is self-hosted so the hero headline never waits on Google Fonts.

### Hierarchy
- **Display** (400, clamp(42px, 12vw, 76px), 1.02): The hero H1 only. White, max 12ch, and its closing phrase is in oak.
- **Headline** (400, clamp(30px, 7.6vw, 48px), 1.08): Section headings. Ink on paper, on-dark on navy and deep. All headings use `text-wrap: balance`.
- **Title** (400, clamp(22px, 6vw, 28px), 1.15): Service row labels. Sibling sizes on the same voice: Facebook row 19-22px, step headings 21px/1.2, footer business name 22px, step numerals 20px.
- **Label** (400, 18px, 1): Buttons and the header phone number (21px from 760px). Form labels and legends are 17px/1.2 on the same face.
- **Lead** (400, clamp(17px, 4.6vw, 19px), 1.7): Ledes (max 40ch) and the work story (max 46ch), `text-wrap: pretty`. The hero promise runs clamp(17px, 4.7vw, 20px) at 1.5, max 30ch.
- **Body** (400, 16px, 1.7): All running copy, and text inputs at 16px so iOS never zooms.
- **Eyebrow** (500, 14px, 1, 0.02em): Text inside the eyebrow pill. This is the only medium weight on the page.
- **Small** (400, 15px): Validation messages and the note under the submit button. Hints and the footer copyright are 14px.

### Named Rules
**The Single Display Weight Rule.** Cal Sans is only ever 400. Hierarchy comes from size and from colour on each band, never from bold display text.

**The Font-Ready Bounce Rule.** The H1 bounce never plays in the fallback face. The headline is hidden until Cal Sans loads, for at most 400ms, and then it animates.

## Layout

Single column and phone first, built from full-bleed bands. In order: paper header, navy photo hero, services on paper, work on deep, how it works on paper, estimate on navy, deep footer. Content sits in a 1160px container with a 20px gutter on phones and 40px from 760px.

- **Phone (<760px):** Sections pad 64px vertically. The hero copy pads 56px top and 64px bottom, and its portrait photo covers the whole hero (object-position 50% 30%) under a vertical navy overlay that darkens downward (rgba(10,28,66) at .74, then .84 at 45%, then .95 at 72%). The two hero buttons stack full width with a 12px gap. Below 380px, chip side padding drops to 14px.
- **Tablet (>=760px):** Sections pad 96px. The header grows to 80px and the logo from 44px to 52px. The hero pads 96px top and 112px bottom. The hero buttons sit side by side, each at least 230px wide. The Facebook row caps at 520px. Steps go three across with a 40px gap. The footer goes to two columns (1.3fr / 1fr).
- **Desktop (>=1024px):** The portrait photo fills only the right half of the hero. A horizontal overlay fades from solid navy at the seam to rgba(10,28,66,.2) at the far edge, and the copy sits on the left at max 520px, vertically centred in min(100svh - 80px, 720px). Services put the heading beside the rows (1fr / 1.4fr). Work puts the intro and Facebook row on the left and the two photos on the right. Estimate puts the heading beside the form (1fr / 1.2fr) with the heading sticky at 40px from the top. All desktop column gaps are 64px.

Rhythm: 16px inside section heads, 20px in the hero stack and between form fields, 24px between steps on phones, 28px between estimate head and form, 32px from a heading to its list or photos.

### Named Rules
**The Band Swap Rule.** A new section always changes band colour from the one before it. Two neighbouring sections never share a ground.

**The Photo Shape Rule.** The hero photo is portrait, so it covers the full hero only where the hero is tall (phones). On wide screens it gets the right half and is never stretched across the full width (`object-fit: cover` only).

## Elevation & Depth

Flat with tonal layering. There is one shadow in the whole system. Depth comes from band contrast (white card on navy), tinted fills nested inside surfaces (pale field on the white card, the paper ready box on the card), and the texture on deep bands. Nothing lifts on hover.

### Shadow Vocabulary
- **Floating lift** (`box-shadow: 0 10px 28px rgba(8,24,46,.3)`): The floating text circle only, because it floats over every band.

### Named Rules
**The One Shadow Rule.** Only the floating circle casts a shadow. Cards, buttons, rows, chips and photos stay flat.

**The Quiet Lines Rule.** Deep bands carry the diagonal line texture at 3.5% white (1px every 23px, 135deg), which never reads as lines through text. The hero carries it too, beneath the photo.

## Shapes

Soft and borderless. Containers are 24px (form card, work photos). The Facebook row is 20px. The ready box nested inside the card is 16px. Fields are 10px. Everything you press that isn't a field is a full pill (buttons, chips, eyebrows) or a circle (service arrows, step numbers, the text circle). Nothing at rest has a stroke, with three exceptions: the 1px hairlines on service rows, the 2px ghost and copy button outlines, and the 2px transparent field border that is held in reserve for hover, focus and error. Focus outlines round to a 6px corner.

## Components

### Buttons
Tall, round, Cal Sans: built for a thumb.
- **Shape:** full pill (999px), min height 56px, 26px side padding, 2px border, 18px Cal Sans label, optional 20px inline SVG icon at a 10px gap.
- **Primary:** oak fill and border with ink text. "Get a free estimate" in the hero, and "Text this to KMD" full width in the form.
- **Hover / Focus:** with a real pointer only, the primary fill lifts to oak-2. In the form, hover also adds the 3px navy focus outline. Focus-visible is a 3px outline at a 3px offset: oak on navy, deep and the hero, navy on light and on the card. Pressing scales to .98. Colour transitions take .2s.
- **Ghost:** transparent with a 2px rgba(244,247,251,.75) outline and on-dark text, for the hero's "See our work". On hover the outline goes solid white over a 10% white wash.
- **Copy:** transparent with an ink outline and ink text, 48px tall, inside the ready box ("Open in Messages", "Copy message").

### Eyebrow Pills
An intentional house feature of the calm band style, chosen by Ellie. A small label above the hero H1 and a few key section headings ("Window and door installers", "Built on trust"), never above every heading. It is a 14px/500 pill with 9px by 14px padding, a 7px oak dot and a faint tint: 6% ink on paper, 12% white on dark. It stays quiet so it can't be mistaken for a button: no arrow, no hover state, no shadow, never a full-strength fill.

### Chips
- **Style:** pill, 48px tall, 18px side padding, pale field fill, 2px transparent border, 16px system text in ink. A visually hidden checkbox drives each one.
- **State:** checked becomes an ink fill with white text. On hover the border turns navy. Keyboard focus puts a 3px navy outline on the label.

### Cards / Containers
- **Corner Style:** 24px for the form card. 16px for the ready box inside it.
- **Background:** card white on the navy band. The ready box is paper on the card.
- **Shadow Strategy:** none (see Elevation).
- **Border:** none.
- **Internal Padding:** clamp(20px, 5vw, 32px) on the card, with a 20px gap between fields. The ready box pads 16px with a 10px gap. The card caps at 600px.

### Inputs / Fields
- **Style:** pale field fill, 2px transparent border, 10px radius, 52px min height (textarea 110px, resizable), 16px system text in ink, soft slate placeholder, navy caret. Labels sit above in 17px Cal Sans. "(optional)" and "(pick any)" hints are 14px soft slate.
- **Focus:** the border turns navy and there is no outline. With a pointer, hover does the same. Transitions take .15s.
- **Error:** the border turns error red. A plain-sentence reason in 15px error red appears below ("Add your name so we know who we're texting back.").
- **Ready box:** after submit, a paper box shows the composed message in a readonly textarea (min 150px, grows with content up to 320px), the phone number, and two copy-style buttons.

### Navigation
No menu. The header sits on paper: the KMD logo on the left (44px tall, 52px from 760px) and the tap-to-call number on the right in 18px Cal Sans ink (21px from 760px), with an oak-ink inline SVG handset and a 44px target. On hover the number turns oak-ink. The header is flat and does not stick. The footer sits on deep with the line texture. It holds the business name in 22px Cal Sans, then phone, email and Facebook as 44px on-dark links that turn oak on hover, then a 14px copyright. Its bottom padding clears the floating circle and the safe area.

### Photo Hero (signature)
KMD's own house photo (portrait, 640w/960w srcset, preloaded, high fetch priority) under a navy overlay, laid over the navy ground with the line texture. On phones the photo fills the whole hero. From 1024px it fills only the right half, behind a horizontal navy fade (see Layout). The copy stack is the eyebrow, the bouncing H1, a one-line promise and at most two buttons (oak primary, ghost secondary). There is no Call button; the number lives in the header.

### Hero Headline Bounce-In (signature motion)
An intentional house feature. With JS on and reduced motion off, the H1 is split into letter spans, each inside a word wrapper that won't break mid-word. The oak accent span survives the split. Each letter slides in from 50px to the right with an overshoot (1s, cubic-bezier(.34,1.56,.64,1)), 20ms after the one before. The H1 is hidden until Cal Sans loads, for at most 400ms. While animating, it carries the full text as `aria-label` and the letters are `aria-hidden`. When the last letter lands, the plain heading HTML is restored so kerning and selection come back. Without JS, or with reduced motion, the plain heading shows at once.

### Service Rows
A ruled list, not cards. Each service is a full-width link, at least 76px tall, with a title-size Cal Sans label and a 44px arrow circle (7% ink tint, ink SVG arrow) on the right, separated by 1px hairlines. Only the arrow changes. With a pointer, hover fills it oak. Keyboard focus fills it oak and moves the 3px navy ring onto the arrow, and the row itself shows no outline, background or shadow. Each row links to the estimate form and pre-ticks the matching chip.

### Work Photos and Facebook Row
On the deep band, the two job photos are stacked full width at a 24px radius with a 16px gap. They have no frame and no caption. Below them sits a white 20px-radius row: the Facebook mark in Facebook blue, the line "Click to see more of our work." in Cal Sans, and the same 44px arrow circle, which is again the only part that changes on hover or focus.

### Numbered Steps
Three steps in an ordered list, numbered by a CSS counter. Each number is a 48px oak circle with a 20px Cal Sans ink numeral. The step heading is 21px Cal Sans ink and the description is soft slate body. They stack with a 24px gap on phones and go three across from 760px.

### Floating Text Circle
An intentional house feature, on by default (`CONFIG.FLOAT`). A 60px oak circle with an ink SVG chat icon sits 16px from the bottom-right corner, inside the safe area, and opens a pre-filled `sms:`. It slides up from 120px below (.35s, cubic-bezier(.2,.8,.2,1)) once the hero is less than 15% in view. It slides away while the estimate form is on screen, so two text controls are never in view together. While hidden it takes `tabIndex=-1` and `aria-hidden`. Without JS or IntersectionObserver it is removed. There is only ever one circle, never a bottom bar.

### Below-the-Fold Rise
Elements marked to rise only animate if they start below the first screen. They begin 12px low at opacity 0 and settle over .4s ease-out when they come 8% into view. Everything is visible at rest, without JS and under reduced motion.

## Do's and Don'ts

### Do:
- **Do** alternate full-bleed bands so neighbouring sections never share a ground, and put the line texture on every deep band.
- **Do** use oak as a fill with ink text, and oak-ink (#87561a) whenever oak has to be text or an icon on a light ground.
- **Do** set every heading, button, row title and form label in Cal Sans 400, and body text in the system stack at 16/1.7.
- **Do** keep cards at 24px, fields at 10px with a tinted fill and no visible border, and everything pressable as a pill or circle.
- **Do** put an eyebrow pill above the hero H1 and only a few key section headings. On dark bands, colour a heading's closing phrase oak.
- **Do** show focus as a 3px outline at a 3px offset: navy on light surfaces, oak on navy, deep and the hero.
- **Do** gate hover styles behind `(hover: hover)` so taps never leave them stuck on.
- **Do** keep every tap target at 44px or larger, with buttons at 56px.
- **Do** make sure all motion runs once, waits for content rather than hiding it, and is off under reduced motion and without JS.

### Don't:
- **Don't** put white text on oak, or oak text on paper or white.
- **Don't** add shadows to cards, buttons, rows, chips or photos; the floating circle is the only shadow.
- **Don't** change anything on a service or Facebook row on hover except the arrow circle.
- **Don't** give the eyebrow an arrow, a hover state, a shadow or a full oak fill.
- **Don't** use the bounce-in on any heading except the hero H1, and never let it play in the fallback face.
- **Don't** stretch the portrait hero photo across a wide hero; give it the right half from 1024px.
- **Don't** add a second floating control or a bottom bar.
- **Don't** introduce a third navy or a second warm accent.
