# Xcel Contracting Website — Change Log

---

## Session: 2026-03-10

### Files Changed
- `index.html`
- `contracting.html`
- `entertainment.html`
- `contact.html`
- `ai-solutions.html`
- `style.css`

### Changes Made

**1. Nav — Added "Serving the Treasure Valley" tagline**
- Added a slim strip at the top of the sticky navigation bar on all pages
- Text reads "SERVING THE TREASURE VALLEY" in logo blue, uppercase, small font
- Replaces the old "Treasure Valley's Finest — Meridian, ID" hero eyebrow text

**2. Hero (index.html) — Removed location eyebrow text**
- Removed "Treasure Valley's Finest — Meridian, ID" line from the hero section

**3. Hero subtitle (index.html) — Updated text**
- Changed from: "Custom entertainment walls, media wall installations, and full residential remodeling — built with precision, delivered with pride."
- Changed to: "Media walls and installations — built with precision, delivered with pride."

**4. Footer — Replaced on all pages**
- Removed: logo, tagline, contact info, page links, service area list, copyright bar
- Replaced with: single centered tagline — "Let Your Entertainment Space XCEL"
- Background changed from dark charcoal to blue gradient (matching brand blue)
- "XCEL" appears in light blue accent color

**5. "What We Do" section removed (index.html)**
- Removed the 3-card grid section: Entertainment Walls / Residential Remodeling / Free Estimates

**6. "Who We Are" section removed (index.html)**
- Removed the intro band section: "eXCELence in Entertainment & Craftsmanship" with side image

**7. Trust bar — Replaced items with brand tagline (index.html)**
- Removed: Free Estimates, 5-Star Rated, Treasure Valley Based, Licensed & Insured, Family Owned
- Replaced with: "Let Your Entertainment Space XCEL" centered on the blue bar

**8. Contracting page — Renamed to Commercial**
- `contracting.html` renamed to `commercial.html`
- Page title and hero heading updated to "Commercial Services"
- Removed "Why Xcel / One Call. Total Project Management." intro section
- Secret hidden dot link on homepage updated to point to `commercial.html`

**9. Nav — Removed Contracting/Commercial link from all pages**
- Contracting/Commercial removed from visible nav on all 5 pages
- Added a secret hidden dot link just above the footer on the homepage as the only access point to the commercial page

**10. Nav — "Serving the Treasure Valley" moved inline**
- Removed the separate top strip
- Tagline now sits centered between the logo and nav links on the same row
- Hidden on mobile screens to keep the hamburger menu clean

**11. Hero (index.html) — Removed "Get a Free Estimate" button**
- Removed the blue "Get a Free Estimate" CTA button from the hero section
- "See Our Work" button remains

**12. Nav — "Get a Quote" renamed to "Contact Us" on all pages**
- Updated nav button label across all 5 pages

---

## Deploy Notes
- All changes are pushed to GitHub (`Motor1G/xcel-contracting`) and auto-deployed via Netlify
- Live site: https://xcelcontracting.com

---

## How to Deploy to Netlify

### Option A — Drag & Drop (easiest)
1. Go to https://app.netlify.com
2. Open your site → **Deploys** tab
3. Drag your entire `Website` folder onto the deploy drop zone
4. Netlify will update the live site automatically

### Option B — Via GitHub
1. Replace the changed files in your GitHub repo (`Motor1G/xcel-contracting`)
2. Netlify will auto-deploy within ~30 seconds

---

Session: 2026-03-11
Files Changed

index.html
assets/css/style.css

Changes Made
1. Nav — Background changed to black

Changed .nav background from var(--white) to #000000

2. Logo — Updated to new transparent PNG

Changed logo image from logo.jpg to XCEL_transparent.png
New file saved to assets/images/XCEL_transparent.png

3. Trust bar — Background changed to black

Changed .trust-bar background from var(--blue) to #000000

4. Trust bar — Added subtitle line

Moved hero subtitle "Media walls and installations — built with precision, delivered with pride." into the trust bar above the XCEL tagline
Styled with hero-sub class to maintain smaller font size
Font size reduced to 0.95rem to fit on one line
Centered using text-align: center and margin: auto

5. Hero heading — Split onto two lines

Added <br> before XCEL so it appears on its own line

6. Hero heading — XCEL accent color updated

Changed .accent color to #1565C0 to match logo blue

7. Hero content block — Repositioned

Moved right using margin-left: 38%
Moved up using margin-top: -80px
Centered text with text-align: center

8. Hero button — Centered

Added justify-content: center to .hero-ctas
