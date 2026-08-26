# Blue Sky - neutral requirements (extracted 26.08.2026, then the original is dropped)

## Audience & goal
- Primary: second-home owners in NC / SC / GA (45-70, affluent, non-technical) deciding
  who should manage their vacation rental. Goal: submit the earnings-estimate form or call.
- Secondary: prospective owners in new regions ("we're growing").
- Brand context: the management business now does business as **The Blue Sky Portfolio
  Group** (Ryan's decision 25.08). **Blue Sky Village** remains the guest-facing rental
  brand. The new site is the management/owner site.

## Content blocks that must exist (what, not how)
1. Value proposition: family-run vacation rental management since 2013, Carolinas & Georgia.
2. Proof numbers: est. 2013, 16+ homes, NC/SC/GA.
3. What is included: channel listing (Airbnb/VRBO/Booking/Expedia/Google), daily pricing,
   cleaning + inspection every stay, 24/7 guest care, maintenance at cost, owner updates.
4. How it works: 3 steps (tell us about the home; we list and run it; you get paid).
5. Pricing: 25% of gross booking value; cleaning/maintenance at cost, no markup;
   no lock-in; owner keeps listing and reviews.
6. Owner testimonial (Karen R., Mooresville NC).
7. FAQ: what 25% covers, no lock-in, owner use of home, cleaning cadence, ~3 weeks to live.
8. Earnings-estimate form -> POST https://photo.proptonomy.ai/bsv-lead
   fields: place, bedrooms, name, contact, honeypot "website". Email fallback on error.
9. Contact: 704-902-5644, blueskyvillagerentals@gmail.com, 320 Bridgewater, Mooresville NC.
10. Guest link: blueskyvillage.guestybookings.com ("Book a stay").

## Hard brand constraints (KEEP)
- Heron crest asset (assets/heron-badge.png), brand names Blue Sky Village /
  The Blue Sky Portfolio Group, Est. 2013, the honest plainspoken voice
  ("We'll tell you honestly if your home isn't a fit"), phone/email/address,
  form endpoint + field names (analytics/backend contract), booking URL.

## BREAK (deliberately change)
- Layout & structure: magazine-cover masthead, centered cover, dropcap, magazine TOC,
  pull-quote band, scroll cue, caption chips overlaid on photos.
- Type system: Fraunces serif display + Hanken Grotesk.
- Color story: warm paper cream + sage + gold (the beige/brass family).
- Paper-grain overlay, golden-hour gradient placeholder blocks.
- window scroll listener for nav state.
- Section order may change; content must not be lost.

## Old-system audit (for the guideline's "before" chapter)
- Palette: #F8F4EC bg, #FBF8F1 surface, #E7ECE7 sage surface, #283744 ink, #E0B148 gold
  accent (#B5862A deep), lines #E2DAC9. Warm-cream editorial.
- Type: Fraunces 340-600 display / Hanken Grotesk body; dropcaps; masthead 6.4rem.
- Imagery: real photos in .shot frames (radius 10-14px) with caption chips
  (blurred dark pill bottom-left), bottom scrims for text, gradient "golden hour"
  placeholders (.photo--lake/.photo--dusk), paper-grain fixed overlay at 3.5% opacity.
- Motion: settle-in masthead (staggered translateY), IntersectionObserver reveals,
  clip-path plate reveal, 28s cover Ken Burns drift. Reduced-motion respected.
- Structure: cover -> feature opener (asym 2-col) -> what-we-do (photo pair) ->
  3 steps -> magazine TOC -> sage pull-quote -> pricing spread -> trust row ->
  FAQ accordion -> ink closing + form -> slim footer.
- Weaknesses: brand called "Blue Sky" but zero blue anywhere; the cream+serif+gold look
  is the generic AI-editorial default; caption pills and scroll cue are clutter;
  photography carries no consistent art direction; masthead pushes CTA below fold on
  small laptops; magazine conceit reads decorative rather than trustworthy.
