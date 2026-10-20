# KMD Windows and Doors — handoff at ~60%

**Live:** https://10elizabethbell.github.io/kmdWindowsAndDoors/ · **Repo:** https://github.com/10elizabethbell/kmdWindowsAndDoors · **Built:** 2026-10-19 from Muse brief (run 2026-10-19, NJ Small Business Network group post)

## What's built
- One page, `index.html` (single file, ~600KB with three embedded photos), phone first.
- **World:** the front of their customer's house: lap siding, a white vinyl double-hung window, navy louvered shutters (logo navy and the shutters in their own job photo), brass only on hover/focus.
- **Signature element:** the hero window's glass is fogged. It wipes itself in slow strokes until someone touches it; a finger (any direction, page doesn't scroll) or the mouse wipes it clear to show their real install behind. Condensation beads form, swell, and run down leaving clear trails; the fog creeps back over a few seconds. It lives in the hero only: a second fogged pane behind the estimate form read as specks on navy and was cut in review (the `Pane` code still supports a photo-less pane via `base`/`avoid` options if Ellie wants it back somewhere).
- Sections: header (real logo, phone top-right) → hero (their job photo behind the copy under a navy overlay, per Ellie's 2026-10-19 photo-hero rule; LET THE LIGHT BACK IN. in white, promise, Free estimate / See our work) → What we do (4 rows, each preselects the form) → Back for more (the repeat-customer story, two crops of the job photo, Facebook button) → How it works (3 steps) → Get a free estimate (form composes a text to 609-374-0679, with a copy-message fallback) → footer (name, phone, email, Facebook).
- Tunables are named at the top of the fog script (`FOG.REGROW`, `PHANTOM_IDLE`, `PHANTOM_SPEED`, `BRUSH_FRAC`, `RUN_CHANCE`...).

## Assumptions I made
- **Name:** page uses "KMD Windows and Doors" (their Facebook page name); header shows the actual logo, which reads "KMD Installations".
- **Email** kmfrank613@gmail.com: brief marked it OCR-only, but it's printed on their own yard sign in the job photo, so I treated it as verified. Footer only.
- **Voice:** "we" (caption says "Send us a message"; crew size unknown).
- **The photo is the repeat customer's house:** inferred, because the photo is in the same post as the story.
- **Services:** "Window installation", "Front doors", "Shutters", "Home improvements": from their yard sign (Window installation · Doors · Home improvements) and the caption (front door, shutters).
- **How it works step 2:** "We come out, measure, and give you a price": standard for the trade, not stated by them.
- **Promise and story lines** ("the same care we'd want in our own", "We treat every house like the one we come home to") are my copy in their voice, built on their "Back for More, Built on Trust" post. Owner should approve.
- **Text handoff:** the form texts 609-374-0679, but whether that number takes texts is unknown. The form has a copy-message fallback; calling is the header number and the footer (the in-form call line was cut so two call links weren't on one screen).
- **Audience:** not treated as 40+ (brief doesn't say); full motion is on. If Ellie thinks their buyers skew older, freeze the glass (see `older-audience.md`).
- **Area:** only "Proudly serving South Jersey and surrounding areas" (verbatim). Sewell, NJ left off; the brief says verify first.
- **Colors:** navy #12306c sampled from the logo; ground #f4f6f7 cool vinyl white; brass #b06f26 from the door hardware.

## Placeholders and gaps
- Only one job photo exists; it's used four ways (behind the hero copy under a navy overlay, behind the fog, full house, door-and-shutters crop). White hero text samples at 6.4:1 or better at 360, 390 and 1440px. Fit check (Ellie's 2026-10-19 condition): the photo is portrait (960x1280) but the hero box is 390x342 on a phone and 702x820 on desktop (copy column only, not a wide band), so `object-fit:cover` keeps the whole two-storey front: windows, shutters, door. It's drawn at 1.22x on a 3x phone and 0.73x on desktop, so it isn't soft. Kept. More photos wanted, especially before/afters.
- No reviews, hours, owner name, licence/insurance, years in business: none shown.
- Favicon is "KMD" lettering on navy (the full logo can't be read at 16px); iPhone home-screen icon is the full logo.
- Messenger (their stated preference) isn't wired; the form texts instead (Ellie's rule). An `m.me` link would need their page username.

## Questions for the owner
- Can 609-374-0679 receive texts?
- Owner's name, and is it a one-person shop or a crew? (I vs we)
- Which towns do you cover? Is Sewell home base?
- More job photos, and before/after pairs?
- Licensed/insured in NJ (HIC number)? Years in business?
- Do you do storm doors, patio/sliding doors, siding, or anything else under "home improvements"?
- Any customer reviews we can quote word for word?

## Ideas not built (yours to pick)
- **Runner-up world:** drafts. Autumn leaves blowing in through a leaky old frame and stopping dead at a sealed new window, pushed around by the finger.
- Write "FREE ESTIMATE" in the fog with a finger (pre-wiped lettering) on the close pane.
- Before/after slider once they send a pair (old fogged-seal window vs new).
- A "what's wrong with your windows?" picker (drafty, foggy between panes, won't open, high bills) that pre-fills the text.
- A sun-angle easter egg: light through the cleared glass casting a warm patch on the siding.
- Atkinson Hyperlegible or a geometric face closer to the logo, if Ellie wants off the system stack.

## Impeccable pass
- Detector: clean. Ignores (in `.impeccable/config.json`, all with reasons): broken-image (lazy base64 photos), repeating-stripes (siding/louvers are the material), dark-glow (eave shadow), overused-font Roboto (system stack is the house rule), cramped-padding (divider rows). Cream-palette was fixed by moving the ground to cool vinyl white #f4f6f7.
- Finish reviewer: applied straight drip trails, removed close-section fog, removed in-form call line and duplicate footer area line, cut the story's last sentence, aligned desktop left edges. Kept the cool ground (reviewer suggested warming it; I changed the contract instead: cool trim vs warm siding is the real look). Concept roll / seed key skipped (unattended build).
- Other modes, done in-thread: audit/adapt (Chromium + WebKit at 360/390/430: no overflow, 44px targets, 16px inputs, first screen OK, vertical touch wipe), harden (empty-field errors, copy fallback, reduced motion = pre-wiped still glass), optimize (600KB; recompressing photos saved only ~10% at visible quality cost, kept), clarify/distill (duplicate lines cut). Not run: live (needs Ellie), onboard (no first-run flow), bolder/quieter/overdrive (no finding called for them).

## Not verified
- Real-device touch on iPhone/Android and inside Facebook's in-app browser (Chromium and WebKit emulation passed).
- The real SMS handoff on iOS/Android (body checked in code; `sms:+1…?&body=` format).
- Frame rate on older phones (fog canvas is capped at 1.5x DPR, drops at 2x).
- Top-level headless screenshots don't show the wipe (a canvas capture quirk); iframe captures and pixel reads confirm it works.
