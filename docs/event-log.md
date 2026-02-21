# toddleSpot — Event Log

> A chronological record of decisions, milestones, and artefacts created throughout the project.

---

## Event History

### 2026-02-15 — Project Kickoff & Product Discovery

**What happened:**
- Initiated product discovery for toddleSpot — an iOS app helping parents find baby-friendly venues
- Completed 4 batches of structured discovery questions covering:
  - Vision & problem space
  - User experience & features
  - Technical & platform decisions
  - Go-to-market & growth strategy

**Key decisions made:**
- **Target users:** First-time parents with newborns and toddlers
- **Launch city:** Upminster, Essex (with architecture built to scale)
- **Platform:** iOS native app
- **Data strategy:** Crowdsourced parent reviews with structured baby-friendly criteria
- **MVP scope defined** — tag-based browse, venue detail pages, structured reviews, user profiles, map view, basic search
- **Post-MVP features parked** — Book Now, trip chaining, itineraries, community/forum, personalised recommendations
- **Business model:** To be validated (ads, sponsored venues, subscription with discounts, affiliates)
- **Privacy:** Collect child age only (not name) for MVP to reduce GDPR burden
- **Venue seeding:** Aaron to manually seed 20-30 venues in Upminster area before launch

**Artefact created:**
- `docs/product-discovery.md` — Full product discovery document

---

### 2026-02-15 — Competitor Research Completed

**What happened:**
- Conducted comprehensive competitor analysis across 12 apps in the parent/family space
- Identified TotSpots and BabyCities as closest competitors (both very early stage)
- Confirmed the core market gap: no established UK app for everyday venue baby-friendliness ratings

**Key findings:**
- **Market is wide open** — nobody owns "Yelp for parents" in the UK
- Existing apps solve adjacent problems (classes/activities or social/community) but not venue baby-friendliness
- toddleSpot's strategic advantages: hyper-local depth, structured criteria (not just stars), everyday venues (not just classes), accessibility-first
- Identified features to adopt: amenity icons, colour-coded map pins, composite baby-friendliness score, free-text parent tips

**Artefact created:**
- `docs/competitor-research.md` — Full competitor research with comparison table, gaps analysis, and positioning

---

### 2026-02-15 — Event Log Created

**What happened:**
- Created this event log to track project decisions, milestones, and artefacts chronologically

**Artefact created:**
- `docs/event-log.md` — This file

---

### 2026-02-21 — Landing Page User Stories & Brand Direction

**What happened:**
- Decided to build a website landing page as the first deliverable (before the app itself)
- Defined user stories for the landing page
- Established brand direction from Aaron's Canva mockup

**Key decisions made:**
- **Landing page goal:** Collect waitlist emails to validate demand and build a launch list
- **Brand direction:** Warm & playful — soft pastels (pink, yellow, light blue), hand-drawn doodle illustrations, speckled paper texture, hand-lettered heading style
- **Tagline:** "Baby friendly venues at your finger tips"
- **Figma project:** "Aarons Playground" created for design work (file key: `DIsOnqlNGB4dPGLwU2Qha6`)

**Landing page user stories:**
1. **Understand the value proposition** — Visitor immediately understands what toddleSpot does
2. **Sign up for launch updates** — Parent enters email to join the waitlist
3. **See what the app will offer** — Preview of key features (venue search, ratings, reviews)
4. **Feel trust and credibility** — Built by a real parent who gets the problem
5. **Share with other parents** — Easy sharing to spread the word (nice-to-have)
6. **See the launch area** — Know it's launching in Upminster/Essex (nice-to-have)

**Artefact created:**
- `docs/user-stories-landing-page.md` — Landing page user stories

---

### 2026-02-21 — Landing Page HTML Mockup & Figma Push

**What happened:**
- Built a self-contained HTML/CSS landing page mockup matching the brand direction
- Sections: hero with email CTA, problem statement, features grid, about (Aaron's story), launch area (Upminster), final CTA, footer
- Design uses Bubblegum Sans headings, Inter body text, pastel palette, paper texture, black outlines with shadow cards
- Pushed the mockup into Figma ("Aarons Playground") via the Figma MCP capture tool

**Key decisions made:**
- No hyphens in any copy (brand style choice)
- Emoji placeholders used for icons, to be replaced with custom hand-drawn illustrations in Figma
- Single self-contained HTML file (no external dependencies beyond Google Fonts)

**Artefacts created:**
- `landing-page-mockup/index.html` — Full landing page mockup (desktop)
- `landing-page-mockup/mobile.html` — Mobile optimised version (390px width)
- Both desktop and mobile versions pushed to Figma file `DIsOnqlNGB4dPGLwU2Qha6` on the "landing page" page (node `3:2`)

---

### 2026-02-21 — Landing Page Polish to Professional Quality

**What happened:**
- Redesigned both desktop and mobile landing page mockups from "craft project" to professional startup quality
- Inspired by peanut-app.io's design language: large confident typography, generous whitespace, soft warm backgrounds

**Key changes made:**
- **Typography:** Replaced Bubblegum Sans with Nunito (800/900 weight) — still friendly but far more professional
- **Icons:** Replaced all emoji icons with hand-drawn style inline SVGs (2px stroke, consistent 48x48 size) — 12 icons total across hero, pain points, features, about, and launch sections
- **Colours:** Refined palette — deeper pink (#F4A7BB), richer gold (#FFD84D), softer blue (#A8D8EA), cleaner paper (#FAF8F5), dark navy ink (#1A1A2E)
- **Layout:** Removed black outlines, hard box-shadows, paper texture, and doodle dividers; added soft shadows, increased section padding (80-100px), wider max-width (960px), alternating white/paper section backgrounds
- **CTAs:** Pill-shaped buttons with subtle hover lift, added "Join 100+ parents on the waitlist" social proof line
- **Highlight:** Changed pink highlight on "baby friendly" from bordered box to underline-style gradient highlight
- **Footer:** Replaced emoji social icons with clean text links (Twitter, Instagram, Email)
- **Cleanup:** Removed Figma capture script tags, border-top/bottom on sections, translate hover effects

**Artefacts updated:**
- `landing-page-mockup/index.html` — Fully redesigned desktop landing page
- `landing-page-mockup/mobile.html` — Fully redesigned mobile landing page

---

### 2026-02-21 — Landing Page Copy Overhaul & Founder Photo

**What happened:**
- Conducted a full copy review of the landing page and rewrote every section for clarity, specificity, and emotional impact
- Added Aaron's real photo (with child) to the "Built by a parent" section
- Fixed badge icon alignment issue in the Upminster launch section
- Pushed updated desktop and mobile versions to Figma

**Copy changes made:**
- **Hero tagline:** Removed generic "all in one app" phrasing → *"Real ratings from real parents, so every outing is one less thing to stress about."*
- **Hero CTA:** "Join the Waitlist" → *"Keep Me Posted"*; removed fake social proof placeholder; subtext now *"Free. No spam. Unsubscribe anytime."*
- **Pain point 1:** Reddit → Mumsnet (more relevant to UK parent audience)
- **Pain point 2:** Broadened from just "No changing table?" to *"Nasty surprises — No changing room, no high chairs, steps everywhere."*
- **Pain point 3:** "expedition" → *"a whole production"* (more natural parent language)
- **Features heading:** "Everything parents actually need" → *"The stuff Google Maps won't tell you"* (positions against the obvious alternative)
- **Search Nearby card:** Now lists specific filters: *"changing rooms, step-free access, parking, high chairs and more"*
- **Parent Reviews card:** Removed "structured baby-friendly criteria" (too product-spec-y) → *"Not just star ratings, but the stuff that actually matters."*
- **Nearby and Now card:** Removed post-MVP promise ("what other parents did next") → *"what's worth the trip with your little one"*
- **About section:** Rewrote to lead with the emotional hook: *"Every trip out with my baby meant the same routine — check Google, ask WhatsApp, scroll Mumsnet, hope for the best."*; replaced SVG icon with circular founder photo
- **Launch section:** "Starting local, growing everywhere" → *"Launching first in Upminster"*; reframed body as opportunity, not limitation
- **Final CTA:** "Be part of it from day one" → *"Help us build the app parents deserve"*; button "Count Me In" (different from hero CTA)
- **Footer:** Removed "Made with love in Upminster" — cleaner, more professional

**Artefacts updated:**
- `landing-page-mockup/index.html` — Updated copy, founder photo, badge fix
- `landing-page-mockup/mobile.html` — Matching changes
- `landing-page-mockup/aaron.jpg` — Founder photo (Aaron with child)
- Both versions pushed to Figma file `DIsOnqlNGB4dPGLwU2Qha6` on landing page page (node `3:2`)

---

### 2026-02-21 — Landing Page Deployed via GitHub Pages

**What happened:**
- Restructured project for deployment: copied production-ready HTML files to repo root (with Figma capture script removed), kept dev copies in `landing-page-mockup/`
- Initialised git repo, created `.gitignore`, added `CNAME` file for custom domain
- Created public GitHub repo at https://github.com/aaronjohal/toddleSpot
- Enabled GitHub Pages on `main` branch (root `/`)
- Custom domain `toddlespot.co.uk` configured via CNAME file

**Key decisions made:**
- **Hosting:** GitHub Pages (free, static, supports custom domains with HTTPS)
- **Repo structure:** Production files at root, dev copies with Figma script in `landing-page-mockup/`
- **Repo visibility:** Public (required for free GitHub Pages)

**Also completed:**
- Configured GoDaddy DNS: 4x A records pointing to GitHub Pages IPs, CNAME `www` → `aaronjohal.github.io`
- TLS certificate provisioned by GitHub (Let's Encrypt)
- HTTPS enforced via repo Settings → Pages
- Site live and secure at **https://toddlespot.co.uk**

**Artefacts created:**
- `/index.html` — Production landing page (no Figma script)
- `/mobile.html` — Production mobile landing page (no Figma script)
- `/aaron.jpg` — Founder photo at repo root
- `/CNAME` — Custom domain config
- `/.gitignore` — Excludes .DS_Store, .obsidian/, .claude/
- GitHub repo: https://github.com/aaronjohal/toddleSpot

---

## Next Steps

| # | Action | Status |
|---|--------|--------|
| 1 | Define user stories for landing page | Done |
| 2 | Design landing page wireframe in Figma | Done (HTML mockup pushed to Figma) |
| 3 | Deploy landing page to GitHub Pages | Done |
| 3a | Configure GoDaddy DNS for toddlespot.co.uk | Done |
| 3b | Wire up email collection (form backend) | Pending |
| 4 | Define detailed user stories for MVP app features | Pending |
| 5 | Decide app technical architecture / tech stack | Pending |
| 6 | Design app prototypes / wireframes | Pending |
| 4 | Design data model (venues, reviews, users, attributes) | Pending |
| 5 | Draft privacy policy | Pending |
| 6 | Create venue seeding plan for Upminster area | Pending |
| 7 | Validate business model assumptions | Pending |
