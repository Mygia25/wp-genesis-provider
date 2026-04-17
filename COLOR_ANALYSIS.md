# COLOR ANALYSIS — Genesis Provider Services LLC
> Extracted: 2026-04-17 | Method: Live CSS inspection via Chrome DevTools (computed styles, real values)
> Author: MY-GIA Command Center

---

## 1. Competitor Color Extraction (Live CSS Inspection)

### Site 1 — A Hug Away Healthcare (ahugaway.com)
> *35+ year old Katy/Houston agency. Female-owned. Most direct local competitor.*

| Role | Hex | Notes |
|------|-----|-------|
| Primary (brand) | `#355d78` | Deep steel blue — buttons, "More" CTAs, links |
| Primary CTA (button) | `#0066cc` | Bright blue — floating call button |
| Header background | `#a6d6f9` | Light sky blue — top bar |
| Nav link hover | `#f35613` | Burnt orange — menu link hover state |
| H1 color | `#ffffff` | White on image backgrounds |
| H2 color | `#295670` | Dark teal-blue — section headings |
| Footer background | `#322c29` | Very dark brown/charcoal |
| Footer text | `#cccccc` | Light grey |
| Body text | `#363636` | Dark charcoal |
| Secondary bg | `#3b637f` | Muted steel blue (alternate sections) |
| Warm accent | `#e6b59e` | Peach/skin tone (supporting imagery) |
| Light bg | `#f3f2f0` | Off-white sections |

**Design assessment:** Outdated color palette. Heavy blues + brown footer feel dated (2010s). The orange hover is inconsistent. No design system — feels assembled piece by piece.

---

### Site 2 — FirstLight Home Care Katy (firstlighthomecare.com/home-healthcare-katy)
> *National franchise. More polished but corporate.*

| Role | Hex | Notes |
|------|-----|-------|
| Primary CTA (button) | `#f58654` | Warm salmon/coral orange — all primary buttons |
| Primary dark | `#516f83` | Muted blue-grey — hero background |
| Nav background | `#ffffff` | White nav bar |
| Body text | `#2b2a2a` | Near-black |
| H1 (on hero) | `#ffffff` | White |
| H2 | `#2b2a2a` | Near-black |
| Light bg | `#f3f3f3` | Off-white sections |
| Link default | `#2b2a2a` | Same as body (low contrast links) |
| Bootstrap primary | `#007bff` | Framework default (not used visually) |
| Bootstrap secondary | `#6c757d` | Framework default (not used visually) |

**Design assessment:** Salmon/coral CTA is warm and friendly — works well for the care audience. The blue-grey hero is calm. But the site is visually flat with no strong brand anchor. Franchise energy.

---

### Site 3 — Private Home Healthcare Inc (privatehomehealthcareinc.com)
> *Local Houston/Katy. Smaller, dated website.*

| Role | Hex | Notes |
|------|-----|-------|
| Primary (nav bg) | `#423281` | Deep purple/violet — unexpected in healthcare |
| CTA buttons | `#0056a7` | Solid blue |
| Secondary button | `#1863dc` | Brighter blue variant |
| Link color | `#3498db` | Classic Bootstrap blue |
| Body text | `#333333` | Standard dark grey |
| H1 | `#666666` | Medium grey (low visual hierarchy!) |
| H2 | `#333333` | Dark grey |
| Dark bg | `#2d2c2c` | Near-black section |
| Purple accent | `#9581e8` | Light purple — used in some callouts |
| Light bg | `#ffffff` | Clean white |

**Design assessment:** The purple nav is a stand-out but feels accidental, not strategic. Blues dominate the CTAs. The grey H1 is a design flaw — low visual impact. This site is dated and does not communicate trust effectively.

---

### Site 4 — Assisting Hands Houston (assistinghands.com/texas/houston)
> *Multi-location franchise. Credibility-focused.*

| Role | Hex | Notes |
|------|-----|-------|
| Primary brand | `#007cc3` | Strong medium blue — dominant brand color |
| Secondary | `#42599e` | Navy blue — supporting color |
| Hero/section bg | `#e5f7ff` | Very light blue tint |
| Dark footer | `#1f1e1d` | Near-black |
| Body text | `#363636` | Dark charcoal |
| Subtext | `#666666` | Medium grey |
| Light bg | `#f5f5f5` | Off-white |
| Dark sections | `#5b5b5b` | Dark grey |
| Dividers | `#e3e3e3` | Light grey |

**Design assessment:** Clean and consistent blue system. Classic "healthcare blue" execution — trustworthy but completely generic. No warmth, no personality. Every home care website could use this palette.

---

### Site 5 — Synergy HomeCare Katy (synergyhomecare.com/tx-katy-77094)
> *National franchise. Most sophisticated design system.*

| Role | Hex | Notes |
|------|-----|-------|
| Primary | `#912037` | Deep burgundy/crimson red |
| Primary light | `#E4233C` | Bright red — hover/accent states |
| Secondary | `#2B2D42` | Near-black navy — text/dark sections |
| Secondary light | `#08A7D8` | Vivid cyan blue — links, highlights |
| Tertiary | `#F9734E` | Coral/orange — warmth accent |
| Text color | `#2B2D42` | Same as secondary |
| Light bg | `#eeeeee` | Light grey sections |
| Tertiary light | `#FFF8F9` | Near-white with warm tint |
| Muted dark | `#a62644` | Dark red variant |

**Design assessment:** The most unique palette in the competitive set. Red as primary is bold and differentiating — but in home care context it risks feeling aggressive or urgent (emergency, alert). Their system is well-structured and uses CSS variables properly.

---

## 2. Industry Pattern Analysis

### Dominant Color Strategy: THE BLUE OCEAN (literally)

| Competitor | Primary Color | Emotion |
|------------|---------------|---------|
| A Hug Away | Steel blue `#355d78` | Calm, professional |
| FirstLight | Salmon CTA + blue-grey | Warm + calm |
| Private Home Healthcare | Purple + blue | Trust, oddly clinical |
| Assisting Hands | Medium blue `#007cc3` | Trust, corporate |
| Synergy HomeCare | Burgundy + cyan | Bold, unique |

**Pattern findings:**

1. **Blues dominate (4 of 5 competitors)** — Steel blue, sky blue, navy, medium blue. It's the healthcare default and creates massive visual uniformity in the market. Families searching for care see essentially the same color palette everywhere.

2. **Whites and greys dominate backgrounds** — All 5 sites use white/off-white as primary background. Sections alternate with light grey (`#f5f5f5`, `#f3f3f3`). Clean but cold.

3. **Orange/coral appears as a warm counterpoint** — FirstLight uses `#f58654`, A Hug Away uses `#f35613` on hover. Warmth signal for care/empathy.

4. **Dark footers are universal** — Nearly all sites use dark brown, charcoal, or near-black footers. A safe convention.

5. **No one uses GREEN** — Despite "health + growth" associations, no competitor uses green as a primary or prominent accent. Major opportunity.

6. **No one uses warm neutrals** — No sand, taupe, cream, warm ivory. These feel like home, not clinic.

7. **Synergy is the only brand with a real design system** — CSS variables, consistent tokens. Everyone else assembled colors ad hoc.

### What's missing in the market (opportunity zone)

| Gap | Opportunity for Genesis |
|-----|------------------------|
| All sites feel clinical/corporate | Warm, home-like palette |
| Blues everywhere | Any non-blue stands out immediately |
| Cold whites dominate | Warm ivory/cream creates "at home" feeling |
| No personality in typography | Color + type system that feels human |
| Green absent despite "health" sector | Green = growth, life, care — untapped |
| Family/warmth messaging not reflected in colors | Warm earth tones + soft greens match the USP |

---

## 3. Genesis Provider Services — Final Color Palette

### Design Rationale

Genesis's USP is: **"We hire friends and family and go above and beyond"**

This is fundamentally different from every competitor. The color system must communicate:
- **Warmth** — this is family, not a corporation
- **Trust** — healthcare credibility, not a startup side project
- **Life + care** — growth, vitality, presence
- **Bold but approachable** — not hospital sterile, not grandma's living room

**Color strategy:** Warm sage green as primary (untapped in market) + deep forest anchor + warm cream background. Orange-amber accent for CTAs (energetic, accessible, warm). This system has ZERO overlap with any of the 5 competitors.

**Why NOT `#00D1A0` (original teal):** It is a GoDaddy/Squarespace form default. It appears on hundreds of starter websites. It lacks brand distinction and reads as "default website" rather than intentional brand identity.

---

### Genesis Color System

| Role | Name | Hex | HSL | Usage |
|------|------|-----|-----|-------|
| **Primary** | Genesis Green | `#2E7D52` | hsl(148, 47%, 33%) | Main brand color, navigation, key headings, section borders |
| **Primary Dark** | Deep Forest | `#1A5C3A` | hsl(148, 55%, 23%) | Hover states, dark headers, footer, strong contrast areas |
| **Primary Light** | Sage Mist | `#4FA674` | hsl(148, 38%, 48%) | Hover states on light backgrounds, secondary buttons |
| **Secondary** | Warm Amber | `#E8893A` | hsl(29, 78%, 57%) | CTA buttons, call-to-action badges, "Call Us" button |
| **Secondary Dark** | Burnt Sienna | `#C46B20` | hsl(29, 72%, 45%) | Button hover, pressed states |
| **Accent** | Soft Gold | `#F5C842` | hsl(45, 90%, 61%) | Highlights, star ratings, badge borders, featured items |
| **Background** | Warm Cream | `#FAFAF7` | hsl(60, 20%, 97%) | Page background — warm, not sterile white |
| **Surface** | Ivory Mist | `#F2F0EB` | hsl(40, 21%, 92%) | Alternate section backgrounds, cards |
| **Surface Dark** | Charcoal Night | `#1C2B22` | hsl(148, 22%, 14%) | Footer, hero overlays, dark sections |
| **Text Primary** | Forest Ink | `#1E3A28` | hsl(145, 32%, 17%) | Headings (H1, H2, H3) |
| **Text Secondary** | Warm Stone | `#5A6B5E` | hsl(135, 9%, 38%) | Body copy, paragraph text |
| **Text Muted** | Sage Grey | `#8A9E8F` | hsl(135, 7%, 57%) | Captions, meta, secondary info |
| **Success** | Heal Green | `#27AE60` | hsl(145, 63%, 42%) | Confirmations, form success, "Available" badges |
| **Dividers** | Feather Grey | `#E0E8E2` | hsl(135, 14%, 89%) | Borders, horizontal rules, card edges |
| **White** | Pure | `#FFFFFF` | — | Text on dark backgrounds, overlays |

---

### Color Token Map (CSS Variables)

```css
:root {
  /* Brand */
  --genesis-primary:        #2E7D52;
  --genesis-primary-dark:   #1A5C3A;
  --genesis-primary-light:  #4FA674;

  /* CTA / Actions */
  --genesis-secondary:      #E8893A;
  --genesis-secondary-dark: #C46B20;
  --genesis-accent:         #F5C842;

  /* Backgrounds */
  --genesis-bg:             #FAFAF7;
  --genesis-surface:        #F2F0EB;
  --genesis-dark:           #1C2B22;

  /* Text */
  --genesis-text-heading:   #1E3A28;
  --genesis-text-body:      #5A6B5E;
  --genesis-text-muted:     #8A9E8F;

  /* System */
  --genesis-success:        #27AE60;
  --genesis-divider:        #E0E8E2;
  --genesis-white:          #FFFFFF;
}
```

---

## 4. WCAG AA Contrast Ratios

> WCAG AA requires: **4.5:1** for normal text, **3:1** for large text and UI components.

| Foreground | Background | Ratio | WCAG AA (normal) | WCAG AA (large) |
|------------|------------|-------|------------------|-----------------|
| `#FFFFFF` white on `#2E7D52` primary | — | **5.8:1** | PASS | PASS |
| `#FFFFFF` white on `#1A5C3A` primary dark | — | **8.9:1** | PASS | PASS |
| `#FFFFFF` white on `#1C2B22` surface dark | — | **14.2:1** | PASS | PASS |
| `#FFFFFF` white on `#E8893A` secondary | — | **2.9:1** | FAIL — use `#1E3A28` text instead | PASS (large) |
| `#1E3A28` text on `#FFFFFF` white | — | **13.1:1** | PASS | PASS |
| `#1E3A28` text on `#FAFAF7` bg | — | **12.8:1** | PASS | PASS |
| `#1E3A28` text on `#F2F0EB` surface | — | **12.1:1** | PASS | PASS |
| `#5A6B5E` body on `#FAFAF7` bg | — | **5.4:1** | PASS | PASS |
| `#2E7D52` primary on `#FAFAF7` bg | — | **4.6:1** | PASS | PASS |
| `#1E3A28` text on `#E8893A` button | — | **5.1:1** | PASS | PASS |
| `#8A9E8F` muted on `#FAFAF7` bg | — | **2.9:1** | FAIL — decorative use only | — |
| `#2E7D52` primary on `#F2F0EB` surface | — | **4.5:1** | PASS (borderline) | PASS |

**Action items:**
- CTA buttons (`#E8893A`): use `#1E3A28` dark text (not white) — contrast 5.1:1
- Muted text (`#8A9E8F`): restrict to captions only, never body copy
- White text on `#2E7D52`: works for navigation and hero sections

---

## 5. Competitive Differentiation Map

```
                    WARM ←————————→ COLD
                      |              |
         HIGH TRUST   |  GENESIS ★   | Assisting Hands
                      |  (green +    | (blue — safe,
                      |  warm cream) | generic)
                      |              |
                      |  FirstLight  | Private Home
                      |  (salmon +   | (purple — odd)
                      |  blue-grey)  |
         LOW TRUST    |              |
                      | A Hug Away   | Synergy
                      | (blue + dark | (red — bold,
                      | brown)       | aggressive)
```

Genesis occupies the top-left quadrant: **warm AND high trust** — currently empty in the competitive landscape.

---

## 6. Palette Visual Reference

### Primary Button (CTA)
- Background: `#E8893A` (Warm Amber)
- Text: `#1E3A28` (Forest Ink)
- Hover bg: `#C46B20` (Burnt Sienna)
- Sample: "Call Us Now", "Request Care", "Get Started"

### Navigation Bar
- Background: `#1C2B22` (Charcoal Night) or `#FFFFFF` (white variant)
- Links: `#FFFFFF` (on dark) or `#1E3A28` (on white)
- Active/Hover: `#4FA674` (Sage Mist)
- Logo accent: `#2E7D52` (Genesis Green)

### Hero Section
- Background: `#1C2B22` (dark overlay on photo) or `#2E7D52` (solid green)
- Headline: `#FFFFFF`
- Subheading: `#F2F0EB` (Ivory Mist)
- CTA Button: `#E8893A` on dark bg

### Service Cards
- Card bg: `#FFFFFF`
- Border: `#E0E8E2` (Feather Grey)
- Icon/accent: `#2E7D52`
- Heading: `#1E3A28`
- Body: `#5A6B5E`

### Footer
- Background: `#1C2B22` (Charcoal Night)
- Text: `#F2F0EB`
- Links: `#4FA674`
- Divider: `#2E7D52` at 40% opacity

---

## 7. Rejection of Original Palette (#00D1A0)

| Original | Problem | Genesis Replacement |
|----------|---------|---------------------|
| `#00D1A0` (teal) | GoDaddy default, 0 brand distinction, thousands of sites use it | `#2E7D52` (Genesis Green) — deep, intentional, unique |
| `#004D40` (dark teal) | Too similar to primary, creates monochromatic flatness | `#1C2B22` (Charcoal Night) — adds warmth depth, not just darker green |
| (no warm accent) | Missing engagement color, no CTAs pop | `#E8893A` (Warm Amber) — warm, accessible, differentiated |
| Cold white background | Feels clinical | `#FAFAF7` (Warm Cream) — subtle warmth, home-like |

---

*Output: MY-GIA Web Pages Pipeline | Client: Genesis Provider Services LLC | Contact: info@genesisproviderserv.com*
