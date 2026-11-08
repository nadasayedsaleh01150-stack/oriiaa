# ORIA | Longevity & Wellness Resort — change log

Two separate websites, built from one shared design system (same CSS, components, fonts and imagery), each with its own pages, navigation, copy and calls to action.

| | Marketing Website | Operator Website |
|---|---|---|
| Folder | ORIA_Marketing_Website | ORIA_Operator_Website |
| Audience | Future guests and the public | Wellness brands and resort operators |
| Pages | 5 | 9 |
| Status | Unlisted until public launch is approved | Unlisted — shared by link |

## Access and privacy (both sites)
- **No password protection** on either site, as requested. Anyone with the link can open them.
- **Kept** `robots.txt` (Disallow all) and a `noindex, nofollow, noarchive` tag on every page, so search engines don't list either site. Remove these from the marketing site when public launch is approved.
- **Kept** each site ships only its own translations; the marketing pages carry no operator text in their source.

## Marketing Website — new
**Added: five pages.** Home · About ORIA · The Destination · Wellness Experience · Contact. All five are in English and Arabic, with right-to-left layout and mobile layouts.
- **Home:** the scroll film with the brief's headline, supporting text and "Discover ORIA". Then "Water. Heat. Time.", the three pillars, "A Sanctuary Shaped by Nature", a five-image wellness gallery and the closing statement.
- **About ORIA:** "The Philosophy of ORIA", the meaning of the name (ōra / aura), Water · Heat · Time, "More Than a Spa" and the vision.
- **The Destination:** "A Destination Within the Desert", the location, the masterplan you can drag, "From Desert to Water", "Stone. Light. Water. Shadow." and a day/night section.
- **Wellness Experience:** "A World of Wellness", the Great Thermae, the thermal ritual, seven thermal experiences, "Beyond Bathing", the Longevity Kitchen, "Space to Slow Down", the Children's Wellness Garden and the closing section.
- **Contact:** Full name, email, enquiry type and message, a consent checkbox, verified contact details and "A Development by El Alfy Holding".

**Excluded on purpose:**
- Operator and partnership content.
- Commercial figures and revenue lines.
- Residences sales content.
- Booking functions and opening dates.
- Security systems.
- The World Record attempt, until its public wording is approved.
- Facility sizes and capacities.

## Operator Website
- **Added** a ninth page, *Feasibility* ("Can it work"), with content from the operator presentation: the two water scenarios, water discipline, heat recovery, clinical governance and site safety, the seven risks, and the six unknowns with what closes each.
- **Moved** Governance and site safety from Destination to Feasibility, so the content isn't repeated.
- **Retained** every other page and section.

## Both sites
- **Changed** ORIA is always shown with "Longevity & Wellness Resort": header, page transitions, loading screen, footer, titles and copyright.
- **Changed** the credit now reads "Developed by OP Labs by Overpowered". The icon and the text both link to https://www.overpoweredagency.co.uk/index.html.
- **Changed** the hero film is the new video. It is used byte for byte, with no re-encode. The film's headlines are timed to its shots.

## Images (7 Nov 2026)
- **Replaced** every image on both sites with 18 of the 19 renders from ORIA_2.pdf. They are used as the original JPEG files from the PDF, byte for byte — never re-compressed or resized.
- **Removed** all earlier images, including the track-record photographs (Grand Sheikh Zayed Mosque, Etihad Museum, One Za'abeel) — those cards are now text only, since ORIA renders can't stand in for real projects.
- **Material swatches** (limestone, travertine, oak, linen) are close-up views of the same renders, not new files.
- **Kept** the hero video's own poster frame, so the film doesn't jump when it starts playing.

## Flagged for review: not found in the catalog (ORIA_Catalog_EN_v12)
1. **"Approximately 25 km inland"** — not in the catalog. The site says only "set well back from the shoreline", which the catalog does state. The catalog also lists a second location under evaluation (the inland water corridor, West Cairo / Giza side). Confirm the North Coast-only wording before launch.
2. **ōra / aura** — the catalog doesn't state where the name comes from. The meanings used are the standard Latin ones (ōra: shore, edge; aura: air, atmosphere). Please confirm.
3. **Children's Wellness Garden image** — there is no approved image of it. A garden image stands in until one is supplied.
4. **Steam Rooms and Hot Springs images** — the closest approved images are used. Please confirm or supply dedicated ones.
5. **El Alfy Holding link** — no verified website address was supplied, so the developer logo isn't linked yet.

## Review fixes (8 Nov 2026)
- Film: only the current chapter's label shows — no more overlapping labels.
- "Heat. Cold. Stillness. Again.": both lines are fully readable as soon as the section enters, and stay inside the screen.
- Header: gains a soft backing layer once you scroll, so text never runs underneath it.
- Phones: the "Why ORIA" cards put their text on a solid panel under the image; closing banners are full-bleed (no frame) with a calmer scrim.
- Intro: the counter now reaches 100 exactly as the last image settles; on phones the number and the ORIA wordmark no longer overlap.

- Footer and contact page: replaced the London office with El Alfy Holding offices (Egypt, UAE, Saudi Arabia, Turkey, United Kingdom), EN + AR.
- Hero legibility: stronger scrims behind hero text, hero text no longer fades to translucent on scroll, header stays dark until it has fully cleared the hero.
- Removed the aerial masterplan image (r13) everywhere; replaced with r11 (Why ORIA card) and r15 (Destination hero). Header is now always dark.
- Legibility pass: form dropdown options themed (light/dark), darker muted and gold text tokens, stronger secondary text on dark sections, footer legal text, ritual steps, dark-mode pills and names. All pages audited for WCAG AA contrast in light and dark.
- Review notes (credibility): site status corrected (site selection under evaluation), Guinness copy framed as a proposed attempt, commercial claims rephrased as design intent, "mineral" replaced by "thermal" pending survey, energy line subject to site study, Feasibility and season headlines revised. EN + AR.
- Enquiry form: posts JSON to ORIA_FORM_ENDPOINT (set in main.js) with source page, page trail, landing page, referrer, language and timestamp; on-page confirmation and error states; honeypot; mailto fallback while no endpoint is set. Operator site adds a request choice (working session / operator brief + NDA) and an NDA link on the CTA bands.
- Second review: preloader shortened to ~2s and shown only on the home page; film fetched only when home is shown (single transfer), phones get oria-film-mobile.mp4 (960px, 6.3 MB; the original film is unchanged for desktop); page images load only for the page being viewed; OS dark mode no longer changes the palette; header nav visible down to 1180px (World record moved to menu/footer on the operator site); Operators hero now r18; operator form button reads "Request a working session".
- Dark green/stone palette restored as the fixed ORIA palette for every visitor (no OS dependence). World record back in the operator header nav (nav shows from 1280px). Wider gap between card grids and the notes beneath them.
- Mobile/tablet pass (360, 390, 768, 834, 1024; EN+AR): contact form panel no longer overflows at 1024, form inputs size to their column, figures and programme cards fit small phones, risk register rows stack on mobile, no horizontal scrolling on any page.
