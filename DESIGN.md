---
name: KMD Windows and Doors
description: The front of a South Jersey house on a cool morning, seen through glass they installed.
colors:
  paper: "#f4f6f7"
  ink: "#15213b"
  muted: "#4a5670"
  navy: "#12306c"
  navy-deep: "#0d2453"
  navy-night: "#0a1c42"
  vinyl: "#fcfbf8"
  siding-tint: "#efe8da"
  line: "#d9dee4"
  field-stroke: "#cdc5b6"
  on-navy-text: "#dbe4f4"
  brass: "#b06f26"
  error: "#a3261b"
  white: "#ffffff"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.2rem, 10.4vw, 4.6rem)"
    fontWeight: 850
    lineHeight: 0.97
    letterSpacing: "-0.015em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(1.85rem, 7.6vw, 2.9rem)"
    fontWeight: 850
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(1.25rem, 5.4vw, 1.6rem)"
    fontWeight: 750
    lineHeight: 1.25
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(1.0625rem, 4.6vw, 1.25rem)"
    fontWeight: 400
    lineHeight: 1.45
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1rem"
    fontWeight: 750
    lineHeight: 1.2
  small:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 400
    lineHeight: 1.55
rounded:
  trim: "2px"
  frame: "4px"
  control: "10px"
  card: "14px"
  round: "50%"
spacing:
  gutter-phone: "16px"
  gutter: "32px"
  section-phone: "60px"
  section: "80px"
  field: "18px"
  chip-gap: "8px"
  container: "1120px"
components:
  button-primary:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.white}"
    typography: "{typography.label}"
    rounded: "{rounded.control}"
    padding: "0 16px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.navy-deep}"
    textColor: "{colors.white}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.navy}"
    typography: "{typography.label}"
    rounded: "{rounded.control}"
    padding: "0 16px"
    height: "56px"
  input:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.control}"
    padding: "12px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "0 16px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.white}"
  service-row:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    padding: "10px 2px"
    height: "70px"
  service-row-arrow:
    backgroundColor: "#e3e7ec"
    textColor: "{colors.navy}"
    rounded: "{rounded.round}"
    size: "44px"
  form-card:
    backgroundColor: "{colors.vinyl}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
    padding: "22px 18px 24px"
  photo-frame:
    backgroundColor: "{colors.vinyl}"
    rounded: "{rounded.frame}"
    padding: "10px"
---

# Design System: KMD Windows and Doors

## Overview

**Creative North Star: "The Front of the House"**

Every surface is a piece of the front of a South Jersey house on a cool morning: the page ground is the window trim in daylight, the warm bands are beige lap siding, the dark blocks are the navy shutters (the logo's navy, and the shutters in the job photo), and the single warm accent is the brass on the front door. Nothing is decoration borrowed from elsewhere; if a colour or material does not exist on that house, it does not exist on the page.

The system is plain-spoken and dense with fact, built phone-first for a Facebook in-app browser. Type is heavy, upright and navy; content sits in simple stacked bands that widen into two columns on desktop. Depth is physical and only where a real object casts it: the window casing, the shutters, the sill, the photo prints in their vinyl frames, the estimate card lifted off the navy close. Flat UI everywhere else.

The signature is the fogged double-hung window: a photograph of a real install behind glass the visitor wipes clear, with condensation beads that form and run and fog that creeps back. It is the one piece of motion in the system, and it carries the story; everything around it stays still.

**Key Characteristics:**
- Cool vinyl-white ground, warm siding bands, navy shutters and close; brass appears only on hover and focus.
- Heavy uppercase navy headlines (weight 850), tight leading, balanced wrapping.
- Ten-pixel rounded controls with 2px strokes; large touch targets (44px minimum, 56px primary).
- Physical, warm-tinted shadows on real objects only; everything else flat.
- One interactive material moment (fogged glass) per page; no other ambient motion.

## Colors

A house-front palette: one cool white, one warm beige, a three-step navy, and a brass that only answers to touch.

### Primary
- **Shutter Navy** (navy): The logo navy. Headlines, the phone link, primary button fill and stroke, selected chips, step numerals, the arrow glyph in service rows, the shutters themselves.
- **Deep Shutter Navy** (navy-deep): Primary button hover fill and the top of the estimate section's gradient (it runs down to a slightly lighter navy, #112c62).
- **Night Navy** (navy-night): Footer ground only.

### Secondary
- **Door Brass** (brass): The one accent. Focus rings (3px, 3px offset), hover border on buttons, inputs and chips, hover fill of the service-row arrow, phone-link hover colour. Never a resting fill, never text at rest. On the navy footer a lighter brass (#f0c58f) takes the link hover so it stays legible on dark.

### Neutral
- **Vinyl Trim White** (paper): Page ground; also the browser theme colour.
- **Window Frame White** (vinyl): Surfaces that are physically "frame": window casing, rail and sill, photo frames, the estimate card.
- **Lap Siding Beige** (siding-tint): The work section's ground; the warm band that interrupts the cool page. The hero wall uses a darker banded siding gradient (#ece4d2 to #bfb092) drawn from the same hue.
- **Navy-Charcoal Ink** (ink): Body text and service-row titles.
- **Slate** (muted): Secondary copy: step descriptions, hints, notes, "(optional)" tags.
- **Trim Line** (line): 1px rules between service rows.
- **Field Stroke** (field-stroke): The warm grey 2px border on inputs and unselected chips.
- **Pale Sky** (on-navy-text): Body text on navy (service-area line, footer).
- **Error Red** (error): Inline validation text and invalid input border only.

### Named Rules
**The Hardware Rule.** Brass is door hardware: it appears only when the visitor touches something (hover, focus, focus-visible). A screen at rest shows no brass.

**The Real House Rule.** A colour earns its place by existing on the house in the job photo. New surfaces pick from trim white, siding beige, shutter navy and brass, not from a new hue.

## Typography

**Display Font:** System sans stack (-apple-system, Segoe UI, Roboto, Helvetica Neue, Arial)
**Body Font:** Same stack
**Label/Mono Font:** None distinct

**Character:** One family carried by weight: 850 uppercase for headlines, 750 for interactive labels and service titles, 400 for reading. See the note under Named Rules on the display face.

### Hierarchy
- **Display** (850, clamp(2.2rem, 10.4vw, 4.6rem), 0.97, uppercase, -0.015em): The hero headline only, one per page, white on the photo hero.
- **Headline** (850, clamp(1.85rem, 7.6vw, 2.9rem), 1.02, uppercase, -0.01em): Section headings; navy on light grounds, white on the navy close. Always `text-wrap: balance`.
- **Title** (750, clamp(1.25rem, 5.4vw, 1.6rem)): Service rows. Step headings use 1.25rem at default bold with 1.25 leading.
- **Numeral** (850, 2.6rem, 0.9): The 1-2-3 step numbers, navy, set in a 44px column beside the step.
- **Lead** (400, clamp(1.0625rem, 4.6vw, 1.25rem), 1.45): The hero promise, max 30ch (34ch on desktop). Section story text runs 1.125rem at 58ch.
- **Body** (400, 1.0625rem, 1.55): All running copy; descriptions cap at 42ch.
- **Label** (750 on buttons, 700 on form labels, 1rem): Buttons, form labels and legends. Chip text sits at 650.
- **Small** (0.9375rem): Hints, form notes, validation messages (600, error red). Footer fine print drops to 0.875rem.

### Named Rules
**The Weight Ladder Rule.** Hierarchy comes from weight and case, not from extra families: 850 uppercase speaks, 750 acts, 400 reads.

**Display face is the system sans stack by house rule.** Ellie's pitch-site style mandates the system font stack (fast on cellular, worked on earlier builds); it overrides Impeccable's craft-floor ban on system display faces. The role is heavy, uppercase, navy. Swap the face only if Ellie asks.

## Layout

Single column, phone first, in full-bleed bands: header, hero, services, work (siding band), how it works, estimate (navy band), footer. Content sits in a 1120px max container; the header runs slightly wider (1184px).

- **Phone (<700px):** sections pad 60px vertical, 16px gutters. Hero stacks copy over the window wall. The hero copy sits on their own job photo (the house shot cropped to sky and upper floor) under a navy overlay, rgba(10,28,66) at .66 to .84, with white text; sampled worst-case contrast is 6.4:1. Buttons on it are a white fill with navy text and a white outline. Primary actions sit side by side in a two-column grid (max 440px wide).
- **Tablet (>=700px):** sections pad 80px / 32px. Photo frames go two-up at 3fr / 4fr. Steps go three across. Footer becomes three columns (1.2fr 1fr 1fr).
- **Desktop (>=1024px):** hero splits copy and wall side by side (1fr / 1.05fr), up to 860px tall, copy aligned to the container's left edge. Services run heading beside list (1fr / 1.4fr). Work puts the tall house photo in the left column spanning the intro, close-up and Facebook link. The estimate pairs heading with a form card capped at 500px.

Rhythm: 8-10px between sibling controls, 18px between form fields, 20-24px under headings and intro copy, 26-28px between steps, 48-64px column gaps on desktop.

## Elevation & Depth

Hybrid: the interface is flat, the house is physical. Shadows appear only on things that are real objects on a real wall, and they are warm-tinted (brown, not black) because they fall on beige siding. Flat UI (buttons, rows, chips, inputs) never takes a shadow.

### Shadow Vocabulary
- **Casing** (`box-shadow: 0 12px 18px -8px rgba(70,48,15,.4), 0 2px 3px rgba(70,48,15,.2)`): The window frame standing off the siding.
- **Shutter** (`box-shadow: 0 10px 14px -6px rgba(70,48,15,.45), inset 0 0 0 1px rgba(0,0,0,.18)`): Shutters hung beside the window.
- **Photo print** (`box-shadow: 0 16px 26px -14px rgba(40,35,20,.45), 0 2px 4px rgba(40,35,20,.14)`): Framed job photos on the siding band.
- **Lifted card** (`box-shadow: 0 26px 44px -20px rgba(0,0,0,.55)`): The estimate form card on navy; the only neutral-black shadow, because it sits on navy rather than siding.
- **Recessed glass** (`box-shadow: inset 0 3px 8px rgba(0,0,0,.3)`): Inner shadow at the top of the window pane.

### Named Rules
**The Object Rule.** If it would cast a shadow on the actual house front, it may have one here; if it is interface, it stays flat.

## Shapes

Gently rounded and practical. Interactive controls share one radius (10px); the estimate card is a step softer (14px); physical window parts are nearly square (2-3px) and photo frames 4px, because vinyl trim is milled, not pillowy. The service-row arrow is the only circle. Strokes are 2px on controls (navy on buttons, warm grey on fields and chips) and 1px hairlines between rows. Photos are always matted in a 10px vinyl-white frame.

## Components

### Buttons
Solid, tall and blunt: built to be hit with a thumb.
- **Shape:** gently rounded (10px), 2px navy stroke, min height 56px (48px inside the post-submit panel).
- **Primary:** navy fill, white 750 label, 16px side padding.
- **Hover / Focus:** fill deepens to deep navy and the stroke turns brass; focus-visible adds a 3px brass ring at 3px offset. Transitions 0.2s on colour only; nothing moves.
- **Outline:** transparent with navy stroke and navy label; hover turns the stroke brass.
- **Facebook link:** a full-width primary-style bar (60px) with an inline SVG Facebook mark.

### Chips
- **Style:** white fill, 2px warm-grey stroke, 10px radius, 48px tall, 650 label; a hidden checkbox drives it.
- **State:** checked becomes navy fill, navy stroke, white text, with an inline SVG check mark revealed. Hover and focus turn the stroke brass; focus-visible adds a 2px brass ring.

### Cards / Containers
- **Corner Style:** 14px for the estimate card; 4px for photo frames.
- **Background:** window frame white.
- **Shadow Strategy:** lifted card on navy; photo print on siding (see Elevation).
- **Internal Padding:** 22px 18px 24px for the card; 10px matte for frames.

### Inputs / Fields
- **Style:** white fill, 2px warm-grey stroke, 10px radius, 52px min height (textarea 104px), body size text, slate placeholder (#6b7488). Labels sit above in 700.
- **Focus:** stroke turns brass plus a 2px brass outline at 2px offset; hover turns the stroke brass. Transitions 0.15s.
- **Error:** stroke turns error red; message below in 0.9375rem / 600 error red, written as a reason ("so we know who we're texting back").

### Navigation
No menu. The header is the logo (44px tall, 52px on desktop) left and the phone number right as a navy 750 link with an inline SVG handset, 44px min target; hover turns it brass. The footer on night navy repeats phone, email and Facebook as 44px-tall white links.

### Service Rows
A ruled list rather than cards: each service is a full-width link 70px tall with a title-weight label and a 44px circular arrow (pale grey fill, navy SVG arrow) at the right, separated by 1px trim lines. Hover and focus fill the arrow brass with a white arrow; the focus ring moves to the arrow. Each row deep-links to the estimate form and pre-checks the matching chip.

### Fogged Window (signature)
A CSS-built double-hung window on a banded lap-siding wall: navy louvred shutters (repeating navy gradient, center rail), vinyl casing, meeting rail and sill, and a pane holding the job photo under two canvases. The fog is a blurred copy of the photo under a cool veil and fine condensation; the pointer or finger wipes it clear with a soft round brush, beads grow and run, and the cleared area fogs back about 5% every ~0.2s. After 6s idle it wipes itself on a slow Lissajous path so the photo is never hidden for long. Reduced motion pre-clears a wave through the glass and stops the animation. A hint line under the actions tells phone users to wipe and mouse users to hover.

## Do's and Don'ts

### Do:
- **Do** keep brass to hover, focus and focus-visible states (3px ring, 3px offset on buttons and links; 2px on fields and chips).
- **Do** set section headings in 850 uppercase navy with balanced wrapping, white on the navy close.
- **Do** give every tap target at least 44px, and primary actions 56px.
- **Do** frame photographs of real jobs in a 10px vinyl-white matte with the warm photo-print shadow.
- **Do** keep shadows warm-tinted (rgba(70,48,15) / rgba(40,35,20)) on the siding and reserve them for physical objects.
- **Do** use inline SVG for every icon (phone, arrow, check, Facebook).
- **Do** alternate cool paper bands with the warm siding band and close on navy.

### Don't:
- **Don't** use brass as a resting fill, a text colour at rest, or a decorative stripe.
- **Don't** introduce colours that are not on the house: no new accent hues, no gradients beyond the siding and the navy close.
- **Don't** put shadows on buttons, chips, inputs or rows.
- **Don't** add a second ambient animation; the fogged glass is the only moving thing on the page.
- **Don't** add small uppercase labels above headings; headings stand on their own.
