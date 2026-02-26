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
| Light Grey      | `#F5F7FA` | rgb(245, 247, 250) | Subtle light backgrounds       |
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

The Elastic brand guide specifies how much of each color should appear across visual materials. Think of this as the overall "feel" — **White and Elastic Blue dominate; accent colors are used sparingly.** The proportions below are derived from the official brand guide color ratio chart:

| Color            | Approximate Proportion | Role                          |
|------------------|----------------------|-------------------------------|
| White            | ~28%                 | Dominant — breathing room, backgrounds, whitespace |
| Elastic Blue     | ~20%                 | Primary brand color — headers, CTAs, key elements  |
| Developer Blue   | ~14%                 | Dark sections, hero areas, footers                  |
| Midnight         | ~10%                 | Supporting dark accent, depth                       |
| Light Teal       | ~8%                  | Accent — highlights, success states, visual pop     |
| Light Poppy      | ~6%                  | Accent — warm highlights, alerts, attention         |
| Pink             | ~5%                  | Accent — badges, tags, secondary highlights         |
| Yellow           | ~4%                  | Accent — warnings, callouts, small emphasis         |
| Light Grey       | ~3%                  | Subtle backgrounds, borders, dividers               |
| Dark Ink         | ~2%                  | Text only — not as a design element                 |

### Proportion Rules
1. **White space is king.** Never fill every surface with color. Elastic's brand breathes.
2. **Elastic Blue is the hero.** It should be the most prominent *color* (vs. white, which is negative space).
3. **Dark tones (Developer Blue + Midnight) create contrast.** Use for hero sections, dark mode, headers.
4. **Accent colors (Teal, Poppy, Pink, Yellow) are seasoning, not the main course.** They bring energy and variety but should never dominate. Each should be used in small doses.
5. **Never use accent colors for large filled backgrounds** unless it's a deliberate single-accent hero section.
6. **Teal is the primary accent** — when you need one accent color, reach for Teal first.

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
- Title slides: Developer Blue or Midnight background with White text
- Content slides: White or Light Grey background with Dark Ink/Ink text
- Accent elements: Elastic Blue for headers, Teal/Poppy for highlights
- Charts/data viz: Use the full accent palette (Teal, Poppy, Pink, Yellow, Elastic Blue)

**Web / HTML / React:**
- Primary buttons: Elastic Blue (`#0B64DD`) with White text
- Secondary buttons: White with Elastic Blue border/text
- Navigation: Developer Blue or White
- Links: Elastic Blue
- Success states: Light Teal
- Warning states: Yellow
- Error states: Light Poppy or Pink
- Cards/sections: Alternate White and Light Grey backgrounds

**Documents (Word/PDF):**
- Headers: Elastic Blue or Midnight
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
}
```

### For React / Tailwind (custom config)
When using Tailwind in React artifacts, define colors inline since we can't modify tailwind config:
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
// Use via inline styles: style={{ backgroundColor: colors.elasticBlue }}
```

### For openpyxl (spreadsheets)
```python
from openpyxl.styles import PatternFill, Font

ELASTIC_BLUE_FILL = PatternFill(start_color="0B64DD", end_color="0B64DD", fill_type="solid")
HEADER_FONT = Font(color="FFFFFF", bold=True, size=12)
```
