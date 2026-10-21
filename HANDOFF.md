# D&J Construction — handoff at ~60%

**Live:** https://10elizabethbell.github.io/djConstruction/ · **Repo:** https://github.com/10elizabethbell/djConstruction · **Built:** 2026-10-20 from Muse brief (run 2026-10-21, Facebook group "Essex County Contractor Referrals") · **Call Sheet:** site set

## What's built
- One page, calm band style: paper header (round D&J badge + name, tap-to-call 519-818-8755 top right) → photo hero → "Your home, treated like ours" (their three flyer promises + big Facebook row) → services on slate (8 rows, Bathrooms marked "Our specialty") → How it works (3 steps, deep slate with the line texture) → quote form → close ("Let's build something great together." + big number) → footer (badge, phone, email, Facebook).
- Palette from their badge and flyer: deep slate `#2e373c` (the logo's own ground), mid slate `#3a4751`, cool paper `#f3f5f7`, sand accent `#d6b48e` (the flyer's brush stroke) as a fill only, `#7a5432` when it has to be text on light, slate-blue `#2d5c85` for form hover/focus outlines.
- Hero: a **generated** bathroom photo (see Images) under a slate overlay; separate phone crop (shower glass + vanity). White text measured at 5.8:1 worst case on phone, 7.8:1 on desktop.
- Motion: hero H1 letter bounce-in, `.rise` fade-up below the first screen, floating text circle (shows after the hero, hides at the form). Reduced motion and no-JS show everything at once (checked).
- Contact: "Get a quote" → form; "Text us" + floating circle → `sms:+15198188755` with "Hi D&J, I found your website. I'm thinking about a renovation: ". Tapping a service row pre-selects its chip. The form composes "Hi D&J, this is <name>. Project: <job>. <message>. Town: <town>." and shows a call fallback.
- Favicon / home-screen icon: crop of the badge's centre (hammers + D&J). OG image 1200x630 (`og.jpg`).

## Assumptions I made
- **Phone and email come from their own flyer**, not the brief: the brief says "no phone published" because Muse's OCR was garbled, but the flyer clearly shows **519 818 8755** and **Djconstruction@mail.com**. Worth telling Muse.
- **The number takes texts** (inferred: 519 cell numbers usually do; brief says "unknown"). If it's a landline, change the hero "Text us" to something else and set `CONFIG.FLOAT=false`.
- Services and their sub-lines are the flyer's words (Kitchens, Bathrooms, Basements, Drywall & Painting, Trim & Doors, Flooring, Decks/Fences/Pergolas, And more). The Facebook page description backs decks, fences, pergolas, tile, flooring.
- Voice is "we" (their posts: "We are new to this group", "We specialize in…").
- Hero promise and trust paragraph are written by me from their slogans ("Your vision. Our expertise.", "Quality renovations built to last."); "We keep you in the loop, finish what we start" and step 2's "a quote before any work starts" are inferred, not stated by them.
- Service area: only "Located in Leamington" is known; the close says "Not sure we cover your area? Call and ask."

## Placeholders and gaps
- **No photos of their own work.** The flyer's room photos are of unknown origin (they look stock/generated), so they are not on the site. The work section is the Facebook row only. Their post promises photos soon: swap them in as work cards (calm kit's 4:5 photo cards) and, ideally, replace the hero.
- No owner name, hours, reviews, prices, years in business, insurance, Instagram, Google Maps listing.

## Images
| File | Source | Notes |
|---|---|---|
| `img/hero.webp`, `img/hero-phone.webp` | Generated with gpt-image-1, 2026-10-20 (`genimg`, `src-assets/gen/hero-1.png`) | Prompt: "Professional real-estate photograph of a newly renovated bathroom in an ordinary Ontario family home: large walk-in shower with light grey porcelain wall tile and a glass panel, a warm wood double vanity with a white quartz top and brushed brass faucets…". An example of the service, **not a D&J job**; no caption claims it is. |
| `img/badge.webp`, `favicon.png`, `apple-touch-icon.png` | D&J Facebook profile image (og:image), 2026-10-20 | Their logo. |
| `og.jpg` | Rendered from the hero photo + logo | |

## Questions for the owner
1. Does 519-818-8755 take texts?
2. Can we have 6–10 photos of finished jobs (bathrooms first), and any before/after pairs?
3. Owner names (the D and the J?) — a first-person "We're D… and J…" line would beat the generic trust copy.
4. Which towns do you cover (Kingsville, Wheatley, Essex, Ruthven…)?
5. Hours, insurance/WSIB, years renovating, any reviews you'd like quoted?
6. Is a quote visit free? (Not claimed on the site.)

## Ideas not built (yours to pick)
- **Signature motion (opt-in):** runner-up worlds from the trade: (1) tile being laid — grout lines drawing in across the hero as a grid that settles; (2) a drywall knife skimming a smooth finish across a band divider; (3) paint roller pass revealing the hero photo; (4) a level bubble that settles as you scroll. Best fit: **tile laying**, since bathrooms are the specialty.
- Before/after sliders under Bathrooms once pairs exist.
- Work photo cards + "Click to see our work on Facebook." row under them.
- A short "Who we are" with the owners' names and a photo.
<!-- impeccable conflicts and not-applied findings are appended below -->

## Not verified
- Real-device tap/SMS handoff on iOS and Android, and inside Facebook's in-app browser (tested in headless Chromium and WebKit only).
- Whether `sms:` opens in Facebook's in-app browser on Android.
- Frame rate of the bounce-in on old phones.
