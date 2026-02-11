# QA Report: Rocio Donohoe

**Date:** 2026-02-11
**URL:** https://cofoundy.github.io/portfolio-rocio-donohoe/
**Status:** PASS

## Data Validation
- [x] Name matches source: "Rocio Donohoe, PMP" — matches config.ts and Google Sheet (married name as requested)
- [x] Email matches source: rociodonohoe@icloud.com — matches Google Sheet exactly
- [x] Title matches source: "International Project & Administrative Professional" — from CV/research
- [x] Companies listed match CV: IBTCI, Gleeds, Arup, Canadian Commercial Corp, Embassy of Canada (x2)
- [x] Education institutions match CV: PMI, USAID University, FITT, Government of Canada, UNIFE
- [x] Dates match source data (all verified against config.ts and research-notes.md)
- [x] No hallucinated data detected

## Content Validation (English Language)
- [x] html lang="en" (verified via curl raw source)
- [x] Nav labels: "About Me", "Key Projects", "Experience", "Education" (English)
- [x] Section headings: "About Me", "Key Projects", "Experience", "Education & Certifications" (English)
- [x] Footer text: "All rights reserved." (English)
- [x] Footer nav: "About Me", "Key Projects", "Experience", "Education" (English)
- [x] NOTE: Chrome screenshot showed Spanish text due to browser auto-translate extension — raw HTML confirmed all-English

## Hero Section
- [x] Profile photo present in HTML (profile.jpg, HTTP 200, circular with border-4 navy)
- [x] Name displayed as "Rocio Donohoe, PMP"
- [x] Title displayed as "International Project & Administrative Professional"
- [x] Location: "Darien, CT" shown
- [x] Tagline shown (italic quote)
- [x] Stats row: 15+ Years Experience, 6+ Countries, PMP Certification
- [x] Social icons: Email + LinkedIn only (no Twitter/GitHub)
- [x] No programming symbols in background (uses clean grid pattern)

## Clean Deploy
- [x] No watermarks (no "Powered by", "Made with", "Built with")
- [x] No placeholder text (no "Lorem ipsum", "Your name here", "[placeholder]")
- [x] No template links (no "View source", "View on GitHub", "Fork this")
- [x] No "undefined" or "null" in content
- [x] No broken links with "#" or "javascript:void(0)" as text
- [x] No Astro logo or Vercel badge visible

## Footer
- [x] Shows email icon (mailto:rociodonohoe@icloud.com)
- [x] Shows LinkedIn icon (linkedin.com/in/rocio-mendoza/)
- [x] NO Twitter icon/link present
- [x] NO GitHub icon/link present
- [x] Copyright: "2026 Rocio Donohoe, PMP. All rights reserved."

## Technical
- [x] Page loads: HTTP 200
- [x] CSS loads: `_astro/index.Cq0Fk61E.css` — HTTP 200
- [x] Profile image loads: `/portfolio-rocio-donohoe/profile.jpg` — HTTP 200
- [x] Favicon loads: `/portfolio-rocio-donohoe/favicon.svg` — HTTP 200
- [x] No critical console errors (only Chrome extension noise: Dark Reader, VSC extension)
- [x] astro.config.mjs has both `site` and `base` correctly set

## Typography
- [x] Google Fonts loaded: Libre Baskerville (headings) + Source Sans 3 (body)
- [x] Serif headings confirmed via global.css: `h1-h6 { font-family: 'Libre Baskerville', serif }`
- [x] Body font confirmed: `body { font-family: 'Source Sans 3', sans-serif }`

## Accent Color
- [x] Navy accent (#1e40af) applied via inline styles throughout
- [x] Verified in skill badges, experience timeline dots, section underlines, education dates

## Animations
- [x] Scroll reveal system present (IntersectionObserver with .reveal/.revealed classes)
- [x] Hero fade-in animations with staggered delays (0.2s through 0.6s)
- [x] Reduced motion support via `@media (prefers-reduced-motion: reduce)`

## Section Counts
- [x] Experience: 6 entries (IBTCI, Gleeds, Arup, CCC, Embassy x2) — all with correct roles and dates
- [x] Education: 6 entries (PMP, USAID Rules, RMP, FITT, Ambassador Program, UNIFE)
- [x] Projects: 3 entries (GH-TAMS, KOULU, Canada Day)
- [x] Skills: 14 skill badges

## Mobile Responsiveness
- [x] `overflow-x: hidden` on html and body (global.css)
- [x] Responsive classes throughout (text-3xl sm:text-4xl md:text-5xl patterns)
- [x] Flexible grid layouts (grid-cols-1 lg:grid-cols-12)
- [x] Photo sizing responsive (w-36 sm:w-44 md:w-52)

## Issues Found
None.

## Notes
- Screenshot captured with Dark Reader + Chrome auto-translate active in browser, making the visual appear dark-themed with Spanish labels. Raw HTML curl confirms all content is in English on a white background.
- LinkedIn URL uses maiden name (rocio-mendoza) as noted in client-meta.md — this is the actual LinkedIn profile found.

## Evidence
- qa-desktop.png (captured with Dark Reader active — visual not representative of actual page appearance)
