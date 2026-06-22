# Site Audit: Wisconsin Anesthesia Professionals
**Live URL:** https://www.anesthesiaserviceswi.com/
**Audit Date:** 2026-06-22
**Platform:** WordPress + Elementor (page builder)
**Last CMS Update Detected:** August 19, 2024

---

## HOW TO UPDATE THIS DOCUMENT
This audit was generated via WebFetch. When you begin the rebuild:
1. After each section is rebuilt, note what changed under the relevant section below with a `[REBUILT]` tag.
2. If new content is discovered on the live site, add it under the appropriate section.
3. When design decisions deviate from the original, document the reason under a `## Rebuild Decisions` heading at the bottom.
4. Mark the overall status at the top: `Status: AUDITED | IN PROGRESS | COMPLETE`

**Status: AUDITED**

---

## 1. Business Information

| Field | Value |
|---|---|
| Business Name | Wisconsin Anesthesia Professionals |
| Tagline | Comprehensive Anesthesia Services for the People of Wisconsin |
| Description | A group of anesthesiologists and CRNAs dedicated to delivering expert ambulatory anesthesia services |
| Address | 1433 North Water Street, Milwaukee, Wisconsin 53202 |
| Phone | (414) 279-7060 |
| Social — Facebook | Linked in footer |
| Social — Twitter | Linked in footer |
| Social — LinkedIn | Linked in footer |
| Blog Author | Sally Li |

---

## 2. Site Structure & Pages

### Pages That Exist
| URL | Status | Notes |
|---|---|---|
| `/` | ✅ Live | Homepage — all main content lives here as anchored sections |
| `/blog/` | ✅ Live | Blog index, 30+ posts |
| `/blog/[slug]/` | ✅ Live | Individual blog posts (e.g. `/blog/individual-variability-in-sevoflurane-sensitivity/`) |

### Pages That Return 404
| URL | Notes |
|---|---|
| `/about/` | Content is a section on homepage, not a separate page |
| `/contact/` | No standalone contact page — contact info is in footer only |
| `/our-anesthesia-professionals/` | Section on homepage only |

### Navigation Structure
The site has a single navigation bar with:
- Skip to content (accessibility link)
- Logo (104×93px)
- Internal anchor link: "Learn More" → `#about`
- "Contact us" text link embedded within the About section body copy

There is no multi-page top nav — all navigation is anchor-based on the single homepage.

---

## 3. Homepage Sections (Top to Bottom)

### 3.1 Hero
- **Headline:** "Comprehensive Anesthesia Services for the People of Wisconsin"
- **CTA Button:** "Learn More" (scrolls to About section)
- **Background:** Large hero image (`Anesthesiologist1-scaled.jpg`, 2560×1757px)
- **Layout:** Full-width, headline over image background

### 3.2 About Us
- **Heading:** "About Us"
- **Body:** "At Wisconsin Anesthesia Professionals, our management team is led by an experienced anesthesiologist with over twenty years of expertise. Our comprehensive approach to delivering anesthesia services is designed to continuously enhance all aspects of perioperative care. This includes collaborating with exceptional clinicians and maintaining a responsive and knowledgeable office team."
- **CTA:** "Contact us to learn more" (inline text link)
- **Layout:** Text alongside a professional medical image
- **Image position:** Image paired with text block (alternating or side-by-side)

### 3.3 Our Anesthesia Professionals
- **Heading:** "Our Anesthesia Professionals"
- **Body:** Describes team expertise, certifications, commitment to patient satisfaction, relationships with surgeons and client facilities, compassionate care, transparent communication, and empathetic bedside manner
- **Layout:** Text + surgical team photograph

### 3.4 Billing
- **Heading:** "Billing"
- **Body:** In-house billing team with proficiency in compliance, medical technology, EMR integration, and patient-friendly anesthesia billing practices. Emphasizes efficiency.
- **Layout:** Text + business/technology-focused image

### 3.5 Supply Chain Management
- **Heading:** "Supply Chain Management"
- **Body:** Certified anesthesia technicians managing inventory, ensuring equipment functionality, understanding of federal and state regulations, compliance for office-based practices.
- **Layout:** Text + equipment-related image

### 3.6 Dedicated Anesthesia Services
- **Heading:** "Dedicated Anesthesia Services"
- **Body:** Relies on evidence-based best practices. Openness to research advances and innovation. Client feedback incorporated into service delivery.
- **Layout:** Text + medical image

### 3.7 Why Work With Us
- **Heading:** "Why Work With Us"
- **Layout:** Four-column feature grid
- **Four pillars:**
  1. Teamwork
  2. Productivity
  3. Client Satisfaction
  4. Quality Service
- Each pillar appears as a labeled block (likely icon + label, no long body copy confirmed)

### 3.8 Blog Preview
- **Heading:** "Blog" (also described as "Stay Tuned with the latest healthcare trends")
- **Layout:** Two featured blog post cards with thumbnails + "VIEW ALL" link
- **Featured Posts:**
  1. "Individual Variability in Sevoflurane Sensitivity" — June 8, 2026
     - Excerpt: "Sevoflurane is widely used because its low blood–gas solubility permits relatively rapid uptake..."
  2. "Tools to Measure Intraoperative Nociception and Analgesia" — May 1, 2026
     - Excerpt: "Traditionally, the management of perioperative analgesia has depended on hemodynamic parameters..."

### 3.9 Footer
- **Address:** 1433 North Water Street, Milwaukee, Wisconsin 53202
- **Phone:** (414) 279-7060
- **Social links:** Facebook, Twitter, LinkedIn
- **No multi-column footer nav confirmed** — appears to be simple contact info + socials

---

## 4. Blog

### Overview
- **URL:** `/blog/`
- **Volume:** 30+ posts dating back to November 2023
- **Author:** Sally Li
- **Format:** Chronological, featured image + excerpt + "Read More" link
- **No sidebar confirmed**

### All Known Blog Posts (Most Recent First)
| Title | Date |
|---|---|
| Individual Variability in Sevoflurane Sensitivity | June 8, 2026 |
| Tools to Measure Intraoperative Nociception and Analgesia | May 1, 2026 |
| Physiological Mechanism of Hypotension During Anesthesia Induction | March 16, 2026 |
| Use of Tracheostomy in Non-Emergent Cases | February 9, 2026 |
| The Effect of Isoflurane Anesthesia on Addiction | January 5, 2026 |
| The Power of Physician Advocacy in Healthcare | November 17, 2025 |
| Predicted Impact of the One Big Beautiful Bill Act on Healthcare | October 6, 2025 |
| *30+ additional posts back to November 2023* | — |

### Blog Post Layout (Single Post)
- **Breadcrumb:** Home > [Post Title]
- **Author + Date** shown
- **References section** at end (peer-reviewed citations)
- **Prev/Next navigation** at bottom
- **No sidebar confirmed**

---

## 5. Design & Visual Style

### Overall Aesthetic
- Conservative, professional, trust-forward medical services design
- Clean and minimal — no confirmed animations or dynamic effects
- Prioritizes readability and authority over visual flair
- **Assessment: Outdated** — typical early-2020s WordPress/Elementor template look

### Color Palette (Inferred — not confirmed from source)
No hex values were extractable via WebFetch. The following are inferred from the healthcare/medical industry aesthetic and professional tone:
- Background: White or near-white
- Text: Dark gray or near-black
- Accents: Conservative blue (trust color — common in medical)
- Buttons: Likely solid blue or dark
- **⚠️ TO CONFIRM:** Open the live site in a browser, use DevTools (F12 → Inspector) to get exact hex values from nav, buttons, headings, and section backgrounds.

### Typography (Inferred — not confirmed)
- No Google Fonts references were detectable in metadata
- Likely system font or common WordPress theme font
- Hierarchy: Large section headings → body text → small metadata
- **⚠️ TO CONFIRM:** Use DevTools on live site to identify exact font-family, weights, and sizes.

### Layout Patterns
- Single-column homepage with stacked sections
- Each section: text block + image, alternating sides or stacked
- "Why Work With Us" section: 4-column grid
- Blog section: 2-column card grid
- No confirmed sidebar anywhere on site

### Images
- Hero: Full-width background image (anesthesiologist in OR)
- Section images: Professional medical photography (surgical teams, equipment, clinical settings)
- Blog thumbnails: Per-post featured images
- Logo: 104×93px

---

## 6. Technical Details

| Detail | Value |
|---|---|
| CMS | WordPress |
| Page Builder | Elementor |
| Schema Markup | JSON-LD (MedicalOrganization + Organization) |
| OG Image | Anesthesiologist1-scaled.jpg (2560×1757px) |
| Accessibility | Skip-to-content link present |
| Mobile | Unknown — not confirmed responsive or not |

### Schema Markup Present
```json
{
  "@type": ["MedicalOrganization", "Organization"],
  "name": "Wisconsin Anesthesia Professionals",
  "address": "1433 North Water Street, Milwaukee, Wisconsin 53202",
  "telephone": "(414) 279-7060",
  "logo": { "width": 104, "height": 93 },
  "sameAs": ["facebook URL", "twitter URL", "linkedin URL"]
}
```

---

## 7. Content Gaps & Missing Pages
- **No standalone Contact page** — contact info only in footer
- **No Team/Bios page** — professionals described generically, no individual profiles
- **No Services detail pages** — all services described in homepage sections only
- **No testimonials/reviews** visible
- **No FAQ** visible
- **No privacy policy or terms** confirmed

---

## 8. Rebuild Notes (To Fill In As Work Progresses)

### Confirmed Improvements Requested
- [ ] More modern, professional, clean aesthetic
- [ ] Better visual hierarchy
- [ ] Cleaner layout

### Design Decisions Made During Rebuild
*(Fill in here as decisions are made)*

### Content Changes From Original
*(Note any copy edits, additions, or removals here)*

### Components to Build
- [ ] Navigation bar
- [ ] Hero section
- [ ] About section
- [ ] Services section (Professionals, Billing, Supply Chain, Dedicated Services)
- [ ] Why Work With Us (4 pillars)
- [ ] Blog preview section
- [ ] Footer
- [ ] Blog index page
- [ ] Blog post template
- [ ] Contact form (new — doesn't exist on current site)

---

## 9. Client Decisions (Answered 2026-06-22)

| # | Question | Answer |
|---|---|---|
| 1 | Colors/fonts? | Agent to choose — brand guide created at `.claude/brand-guide.md` |
| 2 | Contact page? | Yes — on the homepage, same page as everything else. Multiple form types with relevant fields per type. |
| 3 | Team bios? | No — original site has none, do not add |
| 4 | Services as subpages? | No — keep all as homepage sections |
| 5 | Images? | Use royalty-free images from the internet (Unsplash etc.) or generated images |
| 6 | Blog? | Preserve all content exactly; redesign the layout/style |
