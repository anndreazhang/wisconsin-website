# Brand Guide: Wisconsin Anesthesia Professionals
**Created:** 2026-06-22
**Status:** APPROVED — use these values for the rebuild

---

## Brand Personality

Wisconsin Anesthesia Professionals is a high-trust, clinically rigorous medical group.
The brand should feel:
- **Authoritative** — patients and facilities are trusting these professionals with lives
- **Calm** — anesthesia is anxiety-inducing; the brand should reduce that anxiety
- **Modern & clean** — not cold or sterile, but crisp and competent
- **Approachable** — compassionate care is explicitly part of their value proposition

The visual language should read like a premium medical institution, not a generic healthcare template.

---

## Color Palette

### Primary Colors

| Name | Hex | RGB | Usage |
|---|---|---|---|
| Navy Deep | `#0B1F3A` | 11, 31, 58 | Nav background, footer, dark text headings |
| Navy Mid | `#163354` | 22, 51, 84 | Section backgrounds, hover states |
| Brand Blue | `#1C5FA8` | 28, 95, 168 | Primary buttons, links, accents |
| Sky Blue | `#2F80ED` | 47, 128, 237 | Hover states on buttons, highlights |

### Secondary / Accent Colors

| Name | Hex | RGB | Usage |
|---|---|---|---|
| Teal | `#0D7377` | 13, 115, 119 | Secondary accent, icons, subtle highlights |
| Teal Light | `#E0F4F4` | 224, 244, 244 | Teal icon backgrounds, soft badges |

### Neutral Colors

| Name | Hex | RGB | Usage |
|---|---|---|---|
| White | `#FFFFFF` | 255, 255, 255 | Page backgrounds, card backgrounds |
| Off-White | `#F4F7FC` | 244, 247, 252 | Alternating section backgrounds |
| Light Border | `#DDE6F0` | 221, 230, 240 | Card borders, dividers, input borders |
| Text Primary | `#0F1C2E` | 15, 28, 46 | Main body headings |
| Text Body | `#3D5166` | 61, 81, 102 | Body paragraphs |
| Text Muted | `#7A90A8` | 122, 144, 168 | Dates, labels, secondary info |

### Status / Semantic Colors

| Name | Hex | Usage |
|---|---|---|
| Success | `#16A34A` | Form success, checkmarks |
| Error | `#DC2626` | Form validation errors |
| Accent Gold | `#C49A3C` | Rare — only for badges or "20+ years" callouts |

### CSS Variables (copy into stylesheet)
```css
:root {
  --color-navy-deep:   #0B1F3A;
  --color-navy-mid:    #163354;
  --color-brand-blue:  #1C5FA8;
  --color-sky-blue:    #2F80ED;
  --color-teal:        #0D7377;
  --color-teal-light:  #E0F4F4;

  --color-white:       #FFFFFF;
  --color-off-white:   #F4F7FC;
  --color-border:      #DDE6F0;

  --color-text-primary: #0F1C2E;
  --color-text-body:    #3D5166;
  --color-text-muted:   #7A90A8;

  --color-success:     #16A34A;
  --color-error:       #DC2626;
  --color-gold:        #C49A3C;
}
```

---

## Typography

### Font Stack
Both fonts load from Google Fonts.

```html
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet" />
```

| Role | Font | Weight | Notes |
|---|---|---|---|
| Display / Hero | Playfair Display | 700 | H1 only — large, authoritative serif |
| Section Headings | Playfair Display | 600 | H2, H3 |
| UI / Body | Inter | 400, 500, 600, 700 | Everything else |

### Type Scale

| Token | Size | Weight | Font | Usage |
|---|---|---|---|---|
| `--text-hero` | clamp(2.4rem, 5vw, 3.8rem) | 700 | Playfair Display | Hero headline |
| `--text-h2` | clamp(1.8rem, 3.5vw, 2.6rem) | 600 | Playfair Display | Section titles |
| `--text-h3` | 1.2rem | 700 | Inter | Card titles, subsection heads |
| `--text-body-lg` | 1.05rem | 400 | Inter | Lead paragraphs, hero sub-copy |
| `--text-body` | 0.95rem | 400 | Inter | Standard body copy |
| `--text-sm` | 0.85rem | 400–500 | Inter | Captions, dates, labels |
| `--text-label` | 0.72rem | 700 | Inter | Section labels (uppercase, tracked) |

### CSS Variables (type)
```css
:root {
  --font-serif: 'Playfair Display', Georgia, serif;
  --font-sans:  'Inter', system-ui, sans-serif;

  --text-hero:    clamp(2.4rem, 5vw, 3.8rem);
  --text-h2:      clamp(1.8rem, 3.5vw, 2.6rem);
  --text-h3:      1.2rem;
  --text-body-lg: 1.05rem;
  --text-body:    0.95rem;
  --text-sm:      0.85rem;
  --text-label:   0.72rem;
}
```

### Typography Rules
- Section labels (e.g. "ABOUT US", "OUR SERVICES") are always `--text-label`, `font-weight: 700`, `letter-spacing: 0.1em`, `text-transform: uppercase`, colored `--color-brand-blue`
- Section titles use `--font-serif` + `--text-h2`
- Body copy uses `--font-sans` + `--color-text-body`
- Never use Playfair Display below 1.1rem

---

## Spacing System

Based on a 4px base unit.

```css
:root {
  --space-1:  4px;
  --space-2:  8px;
  --space-3:  12px;
  --space-4:  16px;
  --space-5:  20px;
  --space-6:  24px;
  --space-8:  32px;
  --space-10: 40px;
  --space-12: 48px;
  --space-16: 64px;
  --space-20: 80px;
  --space-24: 96px;
}
```

- Section vertical padding: `var(--space-20)` top and bottom (80px)
- Card internal padding: `var(--space-8)` (32px)
- Nav height: 72px fixed
- Max content width: 1200px, centered

---

## Border & Shape

```css
:root {
  --radius-sm:  6px;   /* buttons, inputs, small badges */
  --radius-md:  12px;  /* cards */
  --radius-lg:  16px;  /* image containers, large cards */
  --radius-xl:  24px;  /* hero badges, pill shapes */
  --radius-full: 9999px; /* fully round pills */
  --shadow-sm:  0 2px 8px rgba(11,31,58,0.06);
  --shadow-md:  0 8px 24px rgba(11,31,58,0.10);
  --shadow-lg:  0 20px 48px rgba(11,31,58,0.14);
}
```

---

## Buttons

### Primary Button (dark navy background)
```css
background: var(--color-navy-deep);
color: #fff;
padding: 0.8rem 1.75rem;
border-radius: var(--radius-sm);
font-weight: 600;
font-size: var(--text-body);
/* hover: */ background: var(--color-navy-mid);
```

### Secondary Button (brand blue)
```css
background: var(--color-brand-blue);
color: #fff;
padding: 0.8rem 1.75rem;
border-radius: var(--radius-sm);
font-weight: 600;
/* hover: */ background: var(--color-sky-blue);
```

### Ghost Button (outlined, for use on dark backgrounds)
```css
background: transparent;
color: #fff;
border: 1.5px solid rgba(255,255,255,0.45);
padding: 0.8rem 1.75rem;
border-radius: var(--radius-sm);
font-weight: 600;
/* hover: */ border-color: #fff; background: rgba(255,255,255,0.08);
```

### Outline Button (on light backgrounds)
```css
background: transparent;
color: var(--color-brand-blue);
border: 2px solid var(--color-brand-blue);
padding: 0.75rem 1.75rem;
border-radius: var(--radius-sm);
font-weight: 700;
/* hover: */ background: var(--color-brand-blue); color: #fff;
```

---

## Iconography

- Use emoji icons as placeholders during build (👩‍⚕️ 🧾 📦 🔬 📍 📞)
- Preferred replacement: [Lucide Icons](https://lucide.dev) — clean, minimal, medically appropriate
- Icon container size: 48×48px with `--radius-md` background tint from the appropriate color

### Icon Color Pairings
| Icon type | Background | Icon color |
|---|---|---|
| Blue (main service) | `#DBEAFE` | `--color-brand-blue` |
| Teal (billing, admin) | `--color-teal-light` | `--color-teal` |
| Indigo (supply) | `#E0E7FF` | `#4338CA` |
| Rose (dedicated) | `#FFE4E6` | `#BE123C` |

---

## Photography Style

- **Subject matter:** Clinical environments, anesthesia professionals in OR, team collaboration, medical equipment (clean, not gory)
- **Tone:** Professional, bright, not dark or dramatic
- **Source:** Unsplash (free) — search terms: `anesthesiologist`, `operating room`, `surgical team`, `medical professional wisconsin`
- **Avoid:** Stock photos that look staged or overly cheerful; grainy images; photos with visible patient faces

### Hero Image Treatment
- Full-bleed background image
- Overlay: `linear-gradient(135deg, rgba(11,31,58,0.88), rgba(22,51,84,0.75))` — deep navy overlay to keep text readable

---

## Section Background Pattern

Alternating section backgrounds keep the page scannable without feeling repetitive:

| Section | Background |
|---|---|
| Hero | Dark navy overlay on photo |
| About | `--color-white` |
| Services | `--color-off-white` |
| Why Work With Us | `--color-navy-deep` (dark) |
| Blog Preview | `--color-white` |
| Contact | `--color-off-white` |
| Footer | `--color-navy-deep` |

---

## Contact Form Types

Per client direction, the Contact section includes multiple form types.
Each form type collects only the info relevant to that inquiry.

### Form 1 — General Inquiry
Fields: First Name, Last Name, Email, Phone, Message

### Form 2 — Anesthesia Services Request
Fields: First Name, Last Name, Organization/Facility Name, Role/Title, Email, Phone, Location (city/state), Services Needed (checkboxes: Professionals, Billing, Supply Chain, Dedicated Services), Message

### Form 3 — Billing Inquiry
Fields: First Name, Last Name, Facility Name, Email, Phone, EMR System (text or dropdown), Nature of Billing Issue (textarea)

### Implementation
Rendered as a tab switcher — three labeled tabs above a single form area. Switching tabs swaps the form fields. All forms submit to the same endpoint or can be differentiated by a hidden `form_type` field.

---

## Tone of Voice

| Context | Tone | Example |
|---|---|---|
| Hero | Confident, direct | "Comprehensive Anesthesia Services for Wisconsin" |
| Section body | Professional, warm | "We collaborate with exceptional clinicians..." |
| CTAs | Action-oriented, not pushy | "Learn More", "Get in Touch", "Contact Us" |
| Blog | Clinical, peer-level | Academic writing style with citations |
| Form labels | Clear, minimal | "First Name", not "Please enter your first name" |

---

## HOW TO UPDATE THIS DOCUMENT
- If a color is changed during the build, update the hex here and note why.
- If new component patterns are introduced (e.g. testimonials added later), add a section.
- Font sizes and spacing should not be changed ad-hoc — update the token here first, then apply everywhere.
- Reference this file at the top of every new CSS file or `<style>` block.
