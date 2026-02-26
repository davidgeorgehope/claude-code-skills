---
name: elastic-brand-guidelines
description: Applies Elastic's official brand colors, typography, and design rules to any artifact, presentation, document, dashboard, HTML page, React component, or visual output. Use this skill whenever creating anything visual for Elastic — slides, one-pagers, landing pages, diagrams, data visualizations, social media graphics, or any content that should look like it came from Elastic. Trigger on mentions of Elastic branding, Elastic colors, Elastic style, Elastic design, or any visual output where the user works at Elastic or wants Elastic's look-and-feel. Also use when creating competitive materials, webinar slides, conference presentations, or marketing assets for Elastic.
---

# Elastic Brand Guidelines

## Overview

This skill defines Elastic's official brand identity: core colors, background colors, text colors, color usage proportions, and design principles. Apply these rules whenever producing visual output for Elastic.

**Keywords**: Elastic, branding, brand colors, Elastic Blue, observability, corporate identity, visual identity, styling, design system, Elastic brand

---

## Core Colors

These are Elastic's primary brand palette. All visual output should draw from these colors.

| Name            | Hex       | RGB              | Pantone    | CMYK              |
|-----------------|-----------|------------------|------------|--------------------|
| Elastic Blue    | `#0B64DD` | rgb(11, 100, 221)| 2387 C     | 83, 63, 0, 0       |
| Light Teal      | `#48EFCF` | rgb(72, 239, 207)| 333 C      | 53, 0, 32, 0        |
| Light Poppy     | `#FF957D` | rgb(255, 149, 125)| 2022 C    | 0, 52, 46, 0        |
| Pink            | `#F04E98` | rgb(240, 78, 152)| 2038 C     | 0, 84, 3, 0         |
| Yellow          | `#FEC514` | rgb(254, 197, 20)| 123 C      | 0, 23, 98, 0        |
| Midnight        | `#153385` | rgb(21, 51, 133) | 661 C      | 100, 92, 17, 4      |
| Developer Blue  | `#101C3F` | rgb(16, 28, 63)  | 2768 C     | 99, 90, 43, 52      |

### CSS/JS Quick Reference
```
--elastic-blue: #0B64DD;
--light-teal: #48EFCF;
--light-poppy: #FF957D;
--pink: #F04E98;
--yellow: #FEC514;
--midnight: #153385;
--developer-blue: #101C3F;
```

---

## Background Colors

Use these for page/slide/section backgrounds:

| Name            | Hex       | RGB                | Usage                          |
|-----------------|-----------|--------------------|--------------------------------|
| Developer Blue  | `#101C3F` | rgb(16, 28, 63)    | Dark/hero backgrounds          |
| Light Grey      | `#F5F7FA` | rgb(245, 247, 250) | Alternating section backgrounds|
| White           | `#FFFFFF` | rgb(255, 255, 255) | Default/clean backgrounds      |
| Elastic Blue    | `#0B64DD` | rgb(11, 100, 221)  | Accent/feature backgrounds     |

---

## Text Colors

| Name     | Hex       | RGB              | Usage                              |
|----------|-----------|------------------|------------------------------------|
| Dark Ink | `#1C1E23` | rgb(28, 30, 35)  | Primary text on light backgrounds  |
| Ink      | `#343741` | rgb(52, 55, 65)  | Body text, secondary text          |
| White    | `#FFFFFF` | rgb(255, 255, 255)| Text on dark/colored backgrounds  |

---

## Color Proportions (CRITICAL)

The Elastic brand guide specifies how much of each color should appear across visual materials. These proportions are extracted from the official brand guide color ratio donut chart:

### Tier 1 — Dominant (40% of visual space)
| Color            | Proportion | Role                                              |
|------------------|------------|----------------------------------------------------|
| Elastic Blue     | **20%**    | Primary brand color — headers, CTAs, key elements, feature sections |
| White            | **20%**    | Breathing room, content backgrounds, whitespace    |

### Tier 2 — Supporting (36% of visual space)
| Color            | Proportion | Role                                              |
|------------------|------------|----------------------------------------------------|
| Developer Blue   | **15%**    | Dark hero sections, title slides, footers          |
| Light Teal       | **11%**    | Primary accent — highlights, success, visual pop   |
| Light Grey       | **10%**    | Alternating section backgrounds, cards, dividers   |

### Tier 3 — Accent (24% of visual space, ~4% each)
| Color            | Proportion | Role                                              |
|------------------|------------|----------------------------------------------------|
| Dark Ink         | **4%**     | Text color only — never as a design fill           |
| Midnight         | **4%**     | Small dark accent moments, not a major background  |
| Pink             | **4%**     | Badges, tags, secondary highlights                 |
| Yellow           | **4%**     | Warnings, callouts, small emphasis                 |
| Medium Grey      | **4%**     | Borders, subtle dividers, disabled states          |
| Light Poppy      | **4%**     | Warm highlights, alerts, attention grabbers        |

### Proportion Rules
1. **Elastic Blue and White share the throne equally.** Each gets ~20% of visual space. White is not just "empty" — it's an intentional design element. Elastic Blue is the most prominent *color*.
2. **Developer Blue is for emphasis moments only.** At 15%, use it for title/closing slides, hero sections, dark-mode panels — never as the default background for all content.
3. **Light Teal is the primary accent.** At 11%, it's significantly larger than all other accents. When you need one accent color, reach for Teal first.
4. **Light Grey is a major player.** At 10%, it should appear frequently as alternating section backgrounds, card fills, and content area backgrounds. Do not neglect it.
5. **Midnight is NOT a major structural color.** At 4%, it's the same weight as Pink or Yellow. Do not use it for large backgrounds or treat it as a secondary dark theme — that role belongs to Developer Blue.
6. **All Tier 3 colors are seasoning.** Each at ~4%, they bring energy and variety but should never dominate. No accent color should fill a large background unless it's a deliberate single-accent hero moment.

---

## Typography

Elastic uses bold, confident typefaces to clearly communicate and leave a lasting impression.

### Type Family

| Font             | Weight     | Use Case                          | Availability          |
|------------------|------------|------------------------------------|-----------------------|
| Mier B           | Extrabold  | Headlines (external marketing)     | Licensed — limited use, design team only. Contact brand team before using. |
| Inter            | Regular/Bold | Paragraphs, UI, body text, headlines when Mier B unavailable | Open source, Google Fonts. Also used in product dashboards. |
| Space Mono       | Regular    | Code blocks, large numerals        | Open source, Google Fonts |
| Space Grotesk    | Various    | Developer-specific marketing headlines* | Open source, Google Fonts. *Requires brand design team approval. |

### Font Roles

**Headlines: Mier B Extrabold**
Mier B is a geometric sans that complements Elastic's clean layouts and geometric illustrations. It is a licensed font from General Type Studio with limited desktop licenses. Usage requires coordination with the brand team.

**Paragraphs and UI: Inter**
Inter is Elastic's most widely used font. It is specifically crafted for computer screens with a tall x-height for legibility at small sizes. Inter is also used in Elastic's product dashboards, unifying branding across all web interfaces.

**Numerals and Code: Space Mono**
Use Space Mono when displaying code snippets or large numerals/statistics.

**Special-use Headlines: Space Grotesk**
For developer-specific marketing or technical resources, Space Grotesk provides a more easily readable alternative to Space Mono. Must consult with brand design team before using.

### Alternate Fonts (fallback chain)

For internal documents, PowerPoint, Google Docs/Slides, or emails where Mier B isn't available:
1. **Inter** — Primary alternate for all contexts (headlines + body)
2. **Arial** — Last-resort fallback only when Inter isn't available

### Practical Font Selection Guide

| Context                                  | Headlines          | Body/Paragraphs | Code/Numbers     |
|------------------------------------------|--------------------|------------------|------------------|
| External marketing (web, print)          | Mier B Extrabold   | Inter            | Space Mono       |
| Developer marketing                     | Space Grotesk*     | Inter            | Space Mono       |
| Presentations (PPTX, Google Slides)      | Inter Bold         | Inter Regular    | Space Mono       |
| Internal documents, emails               | Inter Bold         | Inter Regular    | Space Mono       |
| Product UI / dashboards                  | Inter              | Inter            | Space Mono       |
| Claude-generated artifacts (HTML/React)  | Inter Bold         | Inter Regular    | Space Mono       |

*Requires brand design team approval.

---

## Design Principles

### Bold Minimalism
Elastic's design philosophy is "bold minimalism":
- Clean layouts with generous whitespace
- Strong typographic hierarchy
- Color used intentionally, not decoratively
- Let content breathe — avoid visual clutter

### Color Application by Context

**Presentations / Slides:**
- Title slides: Developer Blue background with White text
- Content slides: White or Light Grey background with Dark Ink/Ink text
- Closing slides: Developer Blue or Elastic Blue background
- Headers/titles on content slides: Elastic Blue text
- Accent elements: Light Teal first, then Poppy/Pink/Yellow sparingly
- Charts/data viz: Elastic Blue primary, then Teal, Poppy, Pink, Yellow
- Alternate Light Grey and White backgrounds across content slides for rhythm

**Web / HTML / React:**
- Primary buttons: Elastic Blue (`#0B64DD`) with White text
- Secondary buttons: White with Elastic Blue border/text
- Navigation: Developer Blue or White
- Links: Elastic Blue
- Success states: Light Teal
- Warning states: Yellow
- Error states: Light Poppy or Pink
- Cards/sections: Alternate White and Light Grey backgrounds
- Hero sections: Developer Blue with White text

**Documents (Word/PDF):**
- Headers: Elastic Blue or Developer Blue
- Body text: Dark Ink (`#1C1E23`) or Ink (`#343741`)
- Accent lines/rules: Elastic Blue
- Callout boxes: Light Grey background with Elastic Blue left border
- Highlights: Light Teal sparingly

**Data Visualization:**
- Primary series: Elastic Blue
- Secondary series: Light Teal, Light Poppy, Pink, Yellow (in that order)
- Background: White or Light Grey
- Grid lines: Light Grey
- Axis labels: Ink

### Contrast & Accessibility
- Always ensure sufficient contrast between text and background
- Dark Ink / Ink on White or Light Grey: ✅
- White on Developer Blue, Midnight, or Elastic Blue: ✅
- White on Light Teal, Yellow, or Light Poppy: ❌ (insufficient contrast)
- Dark Ink on Light Teal, Yellow, or Light Poppy: ✅

---

## Implementation Notes

### For pptxgenjs (presentations in Node.js)
```javascript
const C = {
  elasticBlue:  "0B64DD",
  lightTeal:    "48EFCF",
  lightPoppy:   "FF957D",
  pink:         "F04E98",
  yellow:       "FEC514",
  midnight:     "153385",
  devBlue:      "101C3F",
  darkInk:      "1C1E23",
  ink:          "343741",
  lightGrey:    "F5F7FA",
  white:        "FFFFFF",
};
const FONT = {
  headline: "Inter",    // Mier B not available outside design team
  body:     "Inter",
  code:     "Space Mono",
};
```

### For python-pptx (presentations)
```python
from pptx.util import Pt, Inches
from pptx.dml.color import RGBColor

ELASTIC_BLUE = RGBColor(0x0B, 0x64, 0xDD)
LIGHT_TEAL = RGBColor(0x48, 0xEF, 0xCF)
LIGHT_POPPY = RGBColor(0xFF, 0x95, 0x7D)
PINK = RGBColor(0xF0, 0x4E, 0x98)
YELLOW = RGBColor(0xFE, 0xC5, 0x14)
MIDNIGHT = RGBColor(0x15, 0x33, 0x85)
DEVELOPER_BLUE = RGBColor(0x10, 0x1C, 0x3F)
DARK_INK = RGBColor(0x1C, 0x1E, 0x23)
INK = RGBColor(0x34, 0x37, 0x41)
LIGHT_GREY = RGBColor(0xF5, 0xF7, 0xFA)
WHITE = RGBColor(0xFF, 0xFF, 0xFF)
```

### For HTML/CSS
```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Space+Mono&family=Space+Grotesk:wght@400;500;600;700&display=swap');

:root {
  --elastic-blue: #0B64DD;
  --light-teal: #48EFCF;
  --light-poppy: #FF957D;
  --pink: #F04E98;
  --yellow: #FEC514;
  --midnight: #153385;
  --developer-blue: #101C3F;
  --dark-ink: #1C1E23;
  --ink: #343741;
  --light-grey: #F5F7FA;
  --white: #FFFFFF;

  --font-headline: 'Inter', Arial, sans-serif;
  --font-body: 'Inter', Arial, sans-serif;
  --font-code: 'Space Mono', monospace;
  --font-dev-headline: 'Space Grotesk', 'Inter', sans-serif;
}
```

### For React / Tailwind (custom config)
When using Tailwind in React artifacts, define colors and fonts inline:
```jsx
const colors = {
  elasticBlue: '#0B64DD',
  lightTeal: '#48EFCF',
  lightPoppy: '#FF957D',
  pink: '#F04E98',
  yellow: '#FEC514',
  midnight: '#153385',
  developerBlue: '#101C3F',
  darkInk: '#1C1E23',
  ink: '#343741',
  lightGrey: '#F5F7FA',
};
const fonts = {
  headline: "'Inter', Arial, sans-serif",
  body: "'Inter', Arial, sans-serif",
  code: "'Space Mono', monospace",
  devHeadline: "'Space Grotesk', 'Inter', sans-serif",
};
// Import in HTML head or at top of artifact:
// <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Space+Mono&family=Space+Grotesk:wght@400;700&display=swap" rel="stylesheet" />
```

### For openpyxl (spreadsheets)
```python
from openpyxl.styles import PatternFill, Font

ELASTIC_BLUE_FILL = PatternFill(start_color="0B64DD", end_color="0B64DD", fill_type="solid")
HEADER_FONT = Font(color="FFFFFF", bold=True, size=12)
```
