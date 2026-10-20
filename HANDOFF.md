# KMD Windows and Doors — handoff at ~60%

**Live:** https://10elizabethbell.github.io/kmdWindowsAndDoors/ · **Repo:** https://github.com/10elizabethbell/kmdWindowsAndDoors · **Built:** 2026-10-19 from Muse brief (run 2026-10-19, NJ Small Business Network group post) · **Revamped:** 2026-10-19 to the calm band style

## What's built
- One page, `index.html` (~25 KB), with the photos and logo as separate WebP files beside it. Phone first.
- **Calm band style** (`calm-photo-style.md`), coloured from KMD:
  - off-white paper `#f4f6fb`
  - the logo navy `#12306c` and a deep navy `#0a1c42` with the faint line texture
  - oak `#eab04a` as the one warm accent, taken from the front door in their job photo because the logo has no warm colour. It is used as a fill with navy text; as text on light it is `#87561a`.
  - Cal Sans headings, system body text at 16/1.7
  - pill buttons and 24px cards
- **Hero:** their own house photo under a navy overlay.
  - Eyebrow "Window and door installers", then the H1 "Let the light back in, South Jersey.", which bounces in letter by letter.
  - Then the promise and two buttons: Get a free estimate (oak fill) and See our work (outline).
  - **Photo fit:** the photo is portrait (960×1280).
    - **Phone:** it fills the hero behind the text, and `object-fit: cover` keeps the whole two-storey front.
    - **Desktop (≥1024px):** it fills only the right half of the hero and fades into navy, so it is never blown up into a wide band.
    - Checked in screenshots at 390px and 1440px.
  - **Contrast:** the white hero text samples at 8:1 or better.
- **Sections (band colour in brackets):**
  - header: logo, plus the phone number top right
  - hero (navy)
  - What we do (paper): 4 rows, and tapping one pre-ticks it in the form
  - Back for more (deep): the repeat-customer story, two detail photos (upper-storey windows, then the door and shutters) and the Facebook row
  - How it works (paper): 3 steps
  - Get a free estimate (navy): the form texts 609-374-0679; if Messages doesn't open, the ready box offers Open in Messages, Copy message and the number as text
  - footer (deep): name, phone, email and Facebook
- **Floating text circle:** it opens a pre-filled text to 609-374-0679. It appears after the hero and hides while the form is on screen. `CONFIG.FLOAT` turns it off.
- **Fade-up:** only content that starts below the first screen fades up. Under reduced motion or without JS, everything shows at once.

## Assumptions I made
- **Name:** the page uses "KMD Windows and Doors", their Facebook page name. The header shows the actual logo, which reads "KMD Installations".
- **Email** kmfrank613@gmail.com: the brief marked it OCR-only, but it is printed on their own yard sign in the job photo, so I treated it as verified. It appears in the footer only.
- **Voice:** "we". The caption says "Send us a message", and the crew size is unknown.
- **The photo is the repeat customer's house.** I inferred this because the photo is in the same post as the story.
- **Services:** "Window installation", "Front doors", "Shutters" and "Home improvements". They come from the yard sign (Window installation · Doors · Home improvements) and the caption (front door, shutters).
- **How it works, step 2:** "We come out, measure, and give you a price" is standard for the trade, not something they stated.
- **The promise line** is my copy in their voice, built on their "Back for More, Built on Trust" post. The owner should approve it.
- **Eyebrows:** "Window and door installers" (what they are; the hero button already says free estimate) and "Built on trust" (their post title).
- **H1 place:** "South Jersey" is their own wording. Sewell, NJ is left off because the brief says to verify it first.
- **Texting:** the form and the floating circle text 609-374-0679, but whether that number takes texts is unknown. Calling is the header number and the footer.
- **Audience:** I didn't treat them as 40+ because the brief doesn't say so, so the bounce-in and fade-up are on. If you think their buyers skew older, follow `older-audience.md` and turn off the motion.
- **Colours:**
  - the navy is sampled from the logo
  - the oak accent is from the door in their photo
  - the deep navy and paper are calm-style defaults

## Placeholders and gaps
- **Only one job photo exists.** It is used three ways: the full house behind the hero, an upper-storey windows crop, and the door-and-shutters crop. More photos are wanted, especially before/afters.
- **Not shown, because nothing was supplied:** reviews, hours, owner name, licence/insurance and years in business.
- **Favicon and iPhone icon:** the logo's KMD lettering on paper (`favicon.png`, `apple-touch-icon.png`). The thin INSTALLATIONS line can't be read at 16px; the letters can.
- **Messenger isn't wired up,** even though it is their stated preference. The form texts instead, per your rule. An `m.me` link would need their page username.
- **Call Sheet:** the live URL is set on the KMD row (`call-sheet-site.sh`, 2026-10-19).

## Questions for the owner
- Can 609-374-0679 receive texts?
- What's the owner's name? Are you a one-person shop or a crew? (This decides "I" or "we".)
- Which towns do you cover? Is Sewell home base?
- Can you send more job photos, and before/after pairs?
- Are you licensed and insured in NJ (HIC number)? How many years in business?
- Do you do storm doors, patio/sliding doors, siding, or anything else under "home improvements"?
- Any customer reviews we can quote word for word?

## Ideas not built (yours to pick)
- **Opt-in signature motion, the fogged window.** This is the hero of the first build: their install behind fogged glass that you wipe clear with a finger, with beads forming and running, and fog creeping back. It is in git history at `660db5e` (the `Pane`/`FOG` script) and can come back as a section if you want it.
- **Other trade worlds considered:**
  - drafts: autumn leaves blowing through a leaky old frame and stopping dead at a sealed new window
  - a sun patch: light through the new glass moving across the siding
- **Before/after slider,** once they send a pair (an old fogged-seal window versus the new one).
- **A "what's wrong with your windows?" picker** (drafty, foggy between panes, won't open, high bills) that pre-fills the text.
- **Impeccable flags the sanctioned calm-style features:** eyebrow pills (`hero-eyebrow-chip`, `kicker-above-heading`), the bounce easing and the line texture. I kept them because they are your choice, and recorded them as ignores in `.impeccable/config.json`.

## Not verified
- Real-device touch on iPhone and Android, and inside Facebook's in-app browser. Chromium and WebKit emulation passed.
- The real SMS hand-off on iOS and Android. I checked the body in code; it uses the `sms:+1…?&body=` format.
- Cal Sans is self-hosted (`CalSans-latin.woff2`, OFL, latin subset). The hero H1 waits up to 400ms for it before bouncing in; if it never loads, the Avenir Next/Segoe UI fallback shows.
