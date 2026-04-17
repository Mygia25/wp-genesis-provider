# Genesis Provider Services — Design Score Audit
**Date:** 2026-04-17  
**File evaluated:** `index.html`  
**Auditor:** MY-GIA Design Review

---

## Summary Score

| Criteria | Weight | Raw Score | Weighted |
|----------|--------|-----------|---------|
| Mobile-First | 25% | 88 | 22.0 |
| Perceived Speed | 15% | 78 | 11.7 |
| Clear CTA | 20% | 92 | 18.4 |
| Trust | 20% | 85 | 17.0 |
| Friendliness | 20% | 90 | 18.0 |
| **TOTAL** | **100%** | — | **87.1 / 100** |

**Grade: B+ (Strong foundation, minor gaps)**

---

## 1. Mobile-First — 88/100 (Weight 25%)

### What works
- `viewport` meta tag present and correct
- Multiple responsive breakpoints: `@media (max-width: 820px)`, `768px`, `640px`, `540px`, `900px`
- Hero collapses to single column at 768px (`grid-template-columns: 1fr`)
- Services grid collapses to single column at 640px
- Hamburger menu appears at 820px, full mobile menu overlay implemented with ESC/focus management
- Buttons use `padding: 0.875rem 1.75rem` — vertical padding ~14px, total touch target ~44px minimum (passes)
- `clamp()` used throughout for fluid typography and spacing
- `min-height: 100svh` on hero (uses `svh` for mobile browser chrome)
- `overflow-x: hidden` on body prevents horizontal scroll
- `flex-wrap: wrap` on hero actions for small screens

### Issues to fix
- **Nav phone button hidden on mobile** (display:none at 820px) — on small screens there is no persistent phone number visible in nav. Only the hamburger → mobile menu CTA. Users should see at least a tap-to-call icon in the mobile nav bar.
- **Footer grid goes to 2-col at 900px but `footer__col` has no explicit `gap` reduction** — could feel cramped at 768-900px
- **Hero visual card**: images load without `loading="lazy"` — on mobile, images below the fold use bandwidth unnecessarily

---

## 2. Perceived Speed — 78/100 (Weight 15%)

### What works
- No render-blocking JS frameworks (no React, Vue, Webpack bundles)
- Pure CSS animations — no GSAP dependency
- Intersection Observer for scroll animations (deferred, non-blocking)
- CSS gradients used for hero background and shapes (no external images for decoration)
- Lucide icons loaded from unpkg CDN (single script, replaces SVG sprites)
- `font-display=swap` implied by Google Fonts `?display=swap` parameter
- `preconnect` to `fonts.googleapis.com` and `fonts.gstatic.com`
- Scroll animations use `will-change`-friendly properties (opacity + transform)

### Issues to fix
- **Google Fonts loaded synchronously** — the `<link rel="stylesheet">` for Fonts blocks render. Should add `media="print" onload="this.media='all'"` pattern or use `font-display:optional` for CLS prevention
- **Hero image** (`images/hero.png`): no `loading="lazy"` but it's above-fold so that's correct — however no `fetchpriority="high"` hint. Adding `fetchpriority="high"` would improve LCP
- **Service card images** (`images/service-assistant.png`, `images/service-home.png`) lack `loading="lazy"` — these are below the fold and should be lazy-loaded
- **Lucide from unpkg CDN** — `unpkg.com` is a third-party CDN with no SLA. If it's slow, all icons fail. Consider self-hosting or inlining critical icons as SVG
- **No `<link rel="preload">` for hero image** — largest contentful paint could be improved

---

## 3. Clear CTA — 92/100 (Weight 20%)

### What works
- Phone number `(832) 523-9529` appears in: nav bar, hero button, how-it-works CTA, bottom CTA section, footer
- All phone links use `tel:+18325239529` (clickable on mobile)
- Email `info@genesisproviderserv.com` appears in bottom CTA and footer with `mailto:` links
- Every major section has a clear next action:
  - Hero: "Call Us Now" + "Our Services →"
  - How It Works: "Start the Conversation"
  - Bottom CTA: "Call (832) 523-9529"
- CTA buttons are visually distinct (blue `#3B82F6` against sage/white backgrounds)
- Mobile menu has full-width call button
- Bottom CTA section uses dark background to create strong visual separation

### Issues to fix
- **Services section has no CTA** — after reading about both services there's no "Call to learn more" or "Get started" button. A user interested in a specific service hits a dead end.
- **About section has no CTA** — ends with values list, could benefit from a soft CTA like "Meet your care team →"

---

## 4. Trust — 85/100 (Weight 20%)

### What works
- "Licensed in Texas" appears in hero trust row with shield-check icon
- Schema.org `LocalBusiness` markup with telephone, address, area served, and opening hours
- FAQ Schema.org markup (5 questions)
- Founder name (Charlene Okendu) appears in about section with personal narrative
- Testimonials with names and cities (Maria T./Katy, James R./Houston, Sandra L./Sugar Land)
- "Background-Checked Providers" stat in hero
- Professional polish: consistent design system, no clip-art or obvious template look
- Footer shows "Licensed in Texas · Family-First Care"
- Referral-based hiring process mentioned in FAQ and about section

### Issues to fix
- **No NPI number displayed** — NPI is a strong trust signal for healthcare/caregiving businesses. Should appear in footer or about section
- **No explicit license number** — "Licensed in Texas" is stated but no actual license or registration number shown. Adding a HHSC or DADS reference would improve credibility
- **Testimonials lack photos** — letter avatars (MT, JR, SL) are functional but real photos or verified review badges (Google Reviews widget) would increase trust significantly
- **No certifications or affiliations badges** — e.g., "Member of Texas Association of Home Care & Hospice" or similar
- **Schema type should be `HomeHealthBusiness` or `MedicalBusiness`** — currently using `HomeAndConstructionBusiness` which is inaccurate for a healthcare services company

---

## 5. Friendliness — 90/100 (Weight 20%)

### What works
- Warm Sage palette (#2E7D52) conveys life, health, and care — not clinical or corporate
- Background color `#FAFAF7` is warm off-white, not harsh pure white
- Nunito font (rounded, friendly) for headings pairs well with Inter for body
- Personal founder narrative in About section ("My name is Charlene Okendu...")
- Language is warm and human: "we send people who treat your family like their own"
- Hero badge visual (card with stats) feels approachable, not institutional
- Decorative radial gradient shapes add life without being distracting
- Testimonials feel authentic and specific (mention proactive caregiver behavior)
- "Family-First" floating badge on hero card
- FAQ tone is reassuring ("without judgment", "your peace of mind comes first")
- No stock-photo feel (illustrated/abstract portrait frame in about section)

### Issues to fix
- **About portrait uses a CSS gradient frame, not a real photo** — this is a placeholder visual. A real photo of the team or founders would dramatically increase warmth and trust
- **No visible team section** — families want to see WHO will care for them. Even 2-3 caregiver profile cards with names and photos would help
- **Stats feel modest** — "2 Core Services Available" and "5+ Service Areas" are accurate but not inspiring. Could frame as "Hundreds of families served" or lead with impact metrics

---

## Priority Fixes (Items Below or Near 70%)

All criteria passed 70%, but the following are highest ROI improvements:

| Priority | Fix | Impact |
|----------|-----|--------|
| HIGH | Add `loading="lazy"` to below-fold images | Speed + mobile perf |
| HIGH | Add NPI number to footer | Trust signal |
| HIGH | Add service-card CTAs ("Call to discuss →") | Conversion |
| HIGH | Replace schema type with `MedicalBusiness` or `HomeHealthBusiness` | SEO + trust |
| MEDIUM | Add `fetchpriority="high"` to hero image | LCP improvement |
| MEDIUM | Non-blocking Google Fonts load pattern | Render speed |
| MEDIUM | Show phone number/icon in mobile nav bar (not just hamburger) | Mobile conversion |
| LOW | Self-host Lucide or inline critical SVGs | Resilience |
| LOW | Add real founder/team photo | Emotional trust |

---

## Overall Assessment

Genesis Provider Services has an **exceptionally well-built foundation** for a local healthcare business site. The code quality is above average for a single-page site: semantic HTML5, ARIA labels, keyboard navigation, `prefers-reduced-motion` support, clean CSS custom properties, and no JS framework overhead. The design system is cohesive and the brand palette communicates warmth and healthcare credibility.

The primary gaps are: (1) performance hints for images, (2) missing trust credentials (NPI, license number), and (3) no CTAs within individual content sections. These are quick wins that would push the score to 93+.
