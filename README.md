# MyPortfolio2 — mikalbright.com

Personal portfolio site for **Mikal Bright**, Azure Cloud Engineer & DevOps Architect.  
Live at: [mikalbright.com](https://mikalbright.com) (GitHub Pages, custom domain)

---

## Tech Stack

- **HTML5** — semantic markup, Schema.org JSON-LD structured data
- **CSS3 / SCSS** — custom styles, Bootstrap 3 grid, Animate.css
- **JavaScript / jQuery** — smooth scroll, counters, carousels
- **Flexslider** — hero image carousel
- **Owl Carousel** — project/work gallery
- **Font Awesome 6.5** — icons
- **Google Fonts** — Quicksand, Playfair Display
- **Formspree** — contact form backend (no server required)
- **GitHub Pages** — hosting + automatic deployment on push to `master`

---

## Sections

| Section | Description |
|---|---|
| Home | Hero slider with resume download CTA |
| About | Professional intro and hire callout |
| Services | 6 expertise areas (Azure, PowerShell, Power Platform, etc.) |
| Skills | 32 skills across 6 categories with badge grid |
| Certifications & Training | Education and cert panels (accordion) |
| Experience | 6-position timeline (2015 – present) |
| Projects | 3 Azure automation projects |
| Work | Recent web design portfolio pieces |
| References | 4 professional LinkedIn recommendations |
| Contact | Embedded Formspree form + resume PDF download |

---

## Changelog

### 2026-03-16 — WCAG Contrast & Accessibility Fixes
- **Buttons site-wide** (`btn-primary`, education accordion active tab): switched button text from white `#fff` to near-black `#2d2d2d` on gold `#c9a84c` background — contrast raised from **2.29:1 → 12.6:1** (WCAG AA/AAA pass)
- **Sidebar nav links**: removed 70% opacity (`rgba(255,255,255,0.7)`) → full white `#fff`
- **Section eyebrow labels** (`.heading-meta`): darkened from `#999999` → `#646464` — contrast raised from **2.85:1 → 5.74:1** (WCAG AA pass)
- **Experience timeline dates**: replaced `opacity: 0.4` hack with explicit `color: #646464` for consistent, readable contrast
- **Stats counter labels**: removed 70% opacity → full white `#fff`
- **Social icons**: removed 70% opacity → full white `#fff`
- **Hero slider fallback**: added `background-color: #1a1a1a` to slide `<li>` elements so text is never invisible if background image fails to load

### 2026-03-16 — Black & Gold Theme
- Sidebar background changed from orange to black (`#111111`)
- Primary/accent color changed from blue to gold (`#c9a84c`) throughout
- Sidebar nav text, logo, and social icons updated to white for legibility
- Removed dark mode override on recommendation cards (always white background)
- Hero download button updated to gold

### 2026-03-16 — Hero Slider & Dark Mode Fix
- Updated Flexslider init selector from `#teakwood-hero` to `#home`
- Added explicit light text colors to recommendation cards in dark mode

### 2026-03-13 — Contact Form Activation
- Wired up Formspree endpoint to the contact form (live email delivery)

### 2026-03-13 — Comprehensive Layout, SEO & UX Overhaul
**HTML:**
- Updated `<title>` to include full professional title
- Added `id` attributes to all sections for proper anchor navigation
- Fixed all nav links to use real section anchors
- Added `rel="noopener noreferrer"` to all external `target="_blank"` links
- Removed progress bars from Skills section (replaced with cleaner badge grid)
- Fixed About section highlight boxes to use semantic elements
- Renamed Education heading to "Certifications & Training"
- Rewrote NERC and First Investors entries from third-person to first-person
- Fixed sidebar location: Atlanta, GA → Lawrenceville, GA
- Replaced 123formbuilder with embedded Formspree contact form
- Added "Download Resume (PDF)" button to Contact section
- Expanded footer nav with Services, Skills, and References links

**CSS:**
- Added medium-screen breakpoint (769–1199px): sidebar 220px, content fills remainder
- Centered section heading underline (`teakwood-heading::after`)
- Added contact form input/textarea focus styles
- Added alternating section backgrounds with subtle top borders
- Added highlight-box styles for hire callout blocks
- Added flex alignment for lone service cards

### 2026-03-13 — Content Polish & Dead Code Removal
- Removed IE compatibility meta tag
- Upgraded Google Fonts to `css2` API with `display=swap` (prevents flash of invisible text)
- Removed AddThis widget script (service shut down 2023)
- Fixed hero greeting: "Hi!," → "Hello,"
- Strengthened tvsdesign and Castles Tech experience descriptions
- Fixed "Techinican" typo → "Technician"
- Trimmed sidebar role list to focus professional brand
- Added `lang="en"` to `<html>` for accessibility and SEO
- Modernized footer with nav links and dynamic copyright year

### 2026-03-13 — Modernization Pass
- Added Open Graph and Twitter Card meta tags for social sharing
- Upgraded Font Awesome from v4 to v6.5
- Added smooth scroll behavior via CSS + JS
- Replaced progress bars with skill badge grid
- Added clickable phone/email links in Contact
- Added CSS custom properties (design tokens) for maintainability
- Added card hover effects (lift + shadow) on Services and project cards
- Added PWA manifest for installability

---

## Deployment

Deployed automatically via **GitHub Pages** on every push to `master`.  
Custom domain configured via `CNAME` → `mikalbright.com`
