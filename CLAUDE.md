# OJZ — House of Jabri for Dates / بيت جبري للتمور

**Last Updated**: March 12, 2026 (Brand Identity Package added)

## Purpose
Premium Jordanian dates business website and market study for Omar Jabri (OJ). Bilingual EN/AR with language toggle.

## Brand
- **English**: The House of Jabri for Dates
- **Arabic**: بيت جبري للتمور
- **Owner**: Omar Jabri (OJ)
- **Location**: Amman, Jordan / sourced from Jordan Valley (Ghor)

## Files

| File | Purpose | Status |
|------|---------|--------|
| `index.html` | Main English website — products, about, gifting, contact | LIVE |
| `index-ar.html` | Full Arabic version (RTL) — same content, pure Arabic | LIVE |
| `market-study.html` | Comprehensive market study — global dates market, Jordan deep dive, JODA registration, investment tiers, SWOT, regulatory | LIVE |
| `House_of_Jabri_Dates_Market_Study.pdf` | PDF export of market study (1.5MB, generated via Playwright Chromium) | GENERATED |
| `logo.svg` | Full brand logo — palm tree icon + "House of Jabri" + "for Dates" + Arabic. Gold gradient on transparent | DONE |
| `logo-icon.svg` | Icon-only version — palm tree with date clusters in circular frame. No text | DONE |
| `logo-mono.svg` | Monochrome white version of full logo for dark backgrounds | DONE |
| `business-card.html` | Print-ready business card design (front + back), 3.5"x2" with bleed, dark+gold theme | DONE |
| `images/` | 14 Leonardo AI product photos (medjool, barhi, gift boxes, chocolate, stuffed, wholesale, export, palm) | DONE |

## Design System
- **Primary gold**: `#C8A96E`
- **Dark gold**: `#8B6914`
- **Light gold**: `#E8D5A8`
- **Background**: `#0F0A06`
- **Text**: `#D4C4B0`
- **Fonts**: Playfair Display (EN headings), Cairo (Arabic), Inter (EN body)
- Fully responsive, mobile-friendly
- CSS animations: staggered fade-up on scroll (cubic-bezier easing), `prefers-reduced-motion` supported
- Product cards: real photos, zoom-on-hover, dark gradient overlay, "View Details" hover label
- Product modals: image gallery carousel with keyboard nav, dots, arrows
- Hero: dates-palm.jpg background with dark overlay
- About: dates-palm.jpg visual image
- Language toggle: nav-integrated pill button — links between `index.html` and `index-ar.html`

## Brand Identity Package
- **Logo** (`logo.svg`): Palm tree icon with date clusters, serif "House of Jabri" / "for Dates", Arabic text below. Uses gold gradient (`#E8D5A8` to `#C8A96E` to `#8B6914`). Pure SVG, no external deps.
- **Icon** (`logo-icon.svg`): Palm tree only in circular frame. For favicons, app icons, social media avatars.
- **Mono** (`logo-mono.svg`): All-white version for watermarks, dark photo overlays, embossing.
- **Business Card** (`business-card.html`): Front (logo + Omar Jabri + contacts) and back (Arabic-centric with large icon). 3.5"x2" with 0.125" bleed. Print specs: 350gsm, spot UV, gold foil stamp recommended. Pantone 7503 C for gold.

## Contact Form
- Form displays on site but is NOT wired to a backend (shows success message locally)
- No email addresses displayed on site (removed per OJ's request)
- If backend needed later: wire to Formspree or `mail-handler.php` from ceramics toolkit

## Key Decisions
- **No privacy/terms needed** — B2B pitch site, no data collection, no e-commerce
- **No email on site** — form is sufficient, ozjabri@gmail.com removed from all pages
- **PDF generation** — uses Playwright Chromium with JS injection to force animations visible, remove backdrop-filter, fix nav positioning

## Products & Pricing (JOD)
- Medjool Royal: 12/kg
- Medjool Select: 8/kg
- Barhi Golden: 5/kg
- Luxury Gift Box: 25+
- Chocolate Dates: 15/box
- Stuffed Dates: 12/box
- Wholesale: custom pricing
- Export: FOB/CIF

## Session History
- **Session 137 (Mar 12)**: Created site (`index.html`), market study (`market-study.html`). Changed Arabic name from "بيت الجابري" to "بيت جبري". Removed email from all pages. Generated PDF. Sent PDF to OJ on WhatsApp. Changed English name to "House of Jabri for Dates". Created Arabic version (`index-ar.html`) with full RTL. Added language toggle to both pages.
- **Session 138 (Mar 12)**: Brand identity package — `logo.svg` (full logo with palm tree, text EN+AR), `logo-icon.svg` (icon-only in circular frame), `logo-mono.svg` (white monochrome), `business-card.html` (print-ready front+back, 3.5x2" with bleed marks, dark+gold theme, Omar Jabri / Founder, placeholder contacts, WhatsApp icon). **Leonardo AI product images** — 14 images generated via Phoenix model (medjool-royal, medjool-select, medjool-pile, barhi-golden, barhi-ripe, gift-box, gift-ramadan, chocolate-dates, chocolate-close, stuffed-dates, stuffed-variety, wholesale, export-boxes, dates-palm). All product cards now use real photos (background-image) instead of emojis. Product modals use local `images/*.jpg` paths. **UI/UX premium polish** — Hero section: dates-palm.jpg background with dark overlay. About section: dates-palm.jpg visual image added. Product cards: zoom-on-hover (scale 1.05), dark gradient overlay, "View Details" / "عرض التفاصيل" label appears on hover. Trust bar: subtle gold gradient. Staggered scroll-reveal animations with cubic-bezier easing. `prefers-reduced-motion` support added. All improvements applied to both EN and AR pages.
