# DESIGN.md - "Carolina Sky" (the new anchor, v2 · 26.08.2026)

Design read: owner-acquisition landing for affluent second-home owners in the US
Southeast, premium-consumer trust language, leaning toward a light, sky-anchored,
photography-led system. Dials: VARIANCE 7 · MOTION 5 · DENSITY 3.

## Principle
**The sky is the brand.** A company literally named Blue Sky gets a blue-anchored,
daylight-lit identity. UI stays cool, composed and quiet; ALL warmth comes from
photography (golden light in images, never gold chrome in the interface).

## Palette (one accent, locked)
- `--sky-950 #0C1F30` ink / dark band (never pure black)
- `--sky-800 #163A56` secondary ink
- `--sky-600 #1F66AE` THE accent (links, CTA, focus) - the only accent on the page
- `--sky-100 #E2EEF9` accent wash / tinted surfaces
- `--cloud    #F5F8FB` page background (cool off-white)
- `--white    #FEFEFE` cards/surfaces
- `--mist     #93A7B8` muted text on light, `#8FA9BE` on dark
- `--line     #D8E2EB` hairlines
- Feedback: success `#2E7D5B`, error `#B4532E`
- FORBIDDEN: gold/brass/beige chrome, purple, teal-dot decor, gradients as decoration
  (one exception: the dark closing band may fade `#0C1F30 -> #123049` vertically).

## Type
- Display: **Cabinet Grotesk** (Fontshare) 700/800, tracking -0.02em, leading 1.02.
- Body: **Satoshi** (Fontshare) 400/500/700, 1.0625rem/1.6.
- Numbers: Satoshi 700 tabular. No serif anywhere. No italic-descender risks.
- Scale: hero clamp(2.6rem,5.2vw,4.4rem); section H2 clamp(1.9rem,3.2vw,2.7rem);
  card H3 1.25rem; body 1.0625rem; small .92rem.

## Space & shape
- Container 1180px; section padding clamp(72px,10vh,128px); grid gap 24/48.
- Radius system (documented rule): interactive = pill; images & cards = 18px; inputs = 10px.
- Shadows: only on photography cards, tinted `rgba(12,31,48,.18)`, never pure black.

## Imagery (the image system)
- Real photography only. Golden-hour or soft morning light, believable Carolina lake
  country, lived-in, true color, no HDR. People implied (never posed portraits).
- Treatment: full-bleed or 18px-radius frames. NO caption chips/pills on photos;
  captions, when needed, sit under the image in muted text.
- Scrims allowed only under text on full-bleed photos: `linear-gradient(to top,
  rgba(12,31,48,.62), transparent 55%)`.
- Ratio system: hero 3:2, editorial pair 4:3 + 4:5, band 21:9, detail 4:5.

## Motion (MOTION 5, all behind prefers-reduced-motion)
- Entry: hero content fades/rises once (staggered 80ms).
- Scroll: IntersectionObserver reveals (opacity+12px rise), once per element.
- Hover: CTA lifts 1px, photo cards scale image 1.03 over 900ms.
- Nav: solid + hairline after hero, driven by an IO sentinel (no scroll listener).
- Nothing loops. No parallax. No scroll hijack.

## Voice
Plainspoken, honest, first-person plural. Short sentences. "We'll tell you honestly
if your home isn't a fit" stays. No filler verbs (elevate/seamless/unleash).

## Layout families for the page (>=5 distinct, no repeats)
1. Split hero: left content column on cloud, right 55% full-bleed photo (asymmetric).
2. Proof band: single hairline row of large numbers.
3. Bento: 5-cell asymmetric grid mixing photos and service facts.
4. Rail: 3 steps on one connected horizontal line.
5. Big-number split: pricing.
6. Dark photo band: testimonial over 21:9 landscape.
7. Two-column FAQ (no accordion chrome, plain <details>).
8. Dark closing: form card on gradient band.

## Rejected directions (for the record)
- "Twilight ledger": dark navy throughout, mono numbers - too fintech for family-run trust.
- "Field & porch": olive/brick warm Americana - drifts back toward the beige default and
  fights the Blue Sky name.
