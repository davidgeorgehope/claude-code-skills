# SEO/GEO Analyzer Skill

Analyze a URL or local HTML file for SEO health and GEO (Generative Engine Optimization) readiness using 2026 best practices.

## Arguments

$ARGUMENTS can be:
- A URL (e.g., `https://example.com/page`) - fetched via WebFetch
- A local file path (e.g., `./src/pages/landing.html`) - read via Read tool
- Empty - analyze HTML files currently in context or prompt for target

## Instructions

### Step 1: Obtain the Content

**If $ARGUMENTS is a URL** (starts with `http://` or `https://`):
- Use WebFetch to retrieve the page content
- Extract the full HTML for analysis

**If $ARGUMENTS is a file path**:
- Use Read tool to get the file contents
- Verify it's HTML content

**If $ARGUMENTS is empty**:
- Check if there are HTML files in the current context
- If not, ask the user what URL or file they want to analyze

### Step 2: Analyze All Categories

Perform a comprehensive analysis covering these categories:

---

#### A. Meta & Technical SEO

Check for:
- **Title tag**: Present? Length 50-60 chars? Primary keyword near start?
- **Meta description**: Present? Length 150-160 chars? Compelling CTA?
- **Canonical URL**: Present and correct?
- **Open Graph tags**: og:title, og:description, og:image, og:url
- **Twitter Card tags**: twitter:card, twitter:title, twitter:description, twitter:image
- **Schema markup**: JSON-LD present? Type appropriate (Article, Product, FAQ, etc.)?
- **Robots meta**: Indexable? Follow links?
- **Language**: `lang` attribute on `<html>` tag?
- **Viewport**: Mobile-friendly viewport meta tag?

---

#### B. Content Structure (Critical for GEO)

AI systems parse structure heavily. Check for:
- **H1 tag**: Exactly one present? Descriptive?
- **Heading hierarchy**: H2-H6 in logical order (no skipping levels)?
- **TL;DR sections**: Summary content near top of sections?
- **FAQ sections**: Q&A format content (highly GEO-friendly)?
- **Lists**: Bulleted or numbered lists for scannable content?
- **Tables**: Comparison or data tables present?
- **Definitions**: Clear term definitions (good for featured snippets)?
- **Section self-containment**: Can sections stand alone as AI citations?

---

#### C. GEO-Specific Elements

These elements significantly improve AI citation likelihood:
- **Statistics with sources**: Numbers with attribution (e.g., "40% of users according to [Study]")
- **Expert quotations**: Named quotes with credentials
- **Original data**: Unique research, surveys, or data
- **Quotable sentences**: Standalone factual statements AI can cite
- **Fluency optimization**: Natural, authoritative language
- **Comprehensiveness**: Topic covered thoroughly vs. superficially

---

#### D. E-E-A-T Signals (Experience, Expertise, Authoritativeness, Trust)

- **Author byline**: Named author visible?
- **Author credentials**: Bio, title, or expertise shown?
- **Publication date**: When was content published?
- **Last updated date**: When was content last modified?
- **About page link**: Link to about/team page?
- **Contact information**: Email, phone, or contact form?
- **Trust signals**: Certifications, awards, client logos?
- **Source citations**: External links to authoritative sources?

---

#### E. Content Quality Metrics

- **Word count**: <300 (thin), 300-1000 (moderate), 1000-2000 (comprehensive), 2000+ (in-depth)
- **Readability**: Sentence length, paragraph breaks, jargon level
- **Front-loaded info**: Key points in first 100 words?
- **Internal links**: Links to related content on same site?
- **External links**: Links to authoritative external sources?
- **Content freshness signals**: Recent dates, current year references?

---

#### F. Multi-Media & Accessibility

- **Images**: Present with descriptive `alt` text?
- **Videos**: Transcripts or captions available?
- **Data visualizations**: Charts/graphs with text labels?
- **Accessibility**: ARIA labels, semantic HTML?

---

### Step 3: Calculate Scores

**SEO Health Score (1-10)**:
- 10 points total, deduct for issues:
  - Missing title tag: -2
  - Missing/poor meta description: -1
  - No H1 or multiple H1s: -1.5
  - Poor heading hierarchy: -1
  - No schema markup: -1
  - Missing Open Graph: -0.5
  - No canonical: -0.5
  - Thin content (<300 words): -1.5
  - No internal links: -0.5
  - No external links: -0.5

**GEO Readiness Score (1-10)**:
- 10 points total, deduct for issues:
  - No statistics with sources: -2
  - No expert quotes: -1
  - No FAQ section: -1
  - Poor content structure: -1.5
  - No author/E-E-A-T signals: -1.5
  - No quotable standalone facts: -1
  - Content not comprehensive: -1
  - No clear definitions: -0.5
  - No lists or tables: -0.5

---

### Step 4: Generate the Report

Output a structured report in this exact format:

```
## SEO/GEO Analysis Report

**URL/File**: [target analyzed]
**Analysis Date**: [current date]

---

### Overall Scores

| Metric | Score | Rating |
|--------|-------|--------|
| SEO Health | X/10 | [Poor/Fair/Good/Excellent] |
| GEO Readiness | X/10 | [Poor/Fair/Good/Excellent] |

Rating scale: 1-3 Poor, 4-5 Fair, 6-7 Good, 8-10 Excellent

---

### Critical Issues (Fix First)

[List issues that severely impact SEO or GEO with specific fixes]

1. **[Issue]**: [Current state] → [Recommended fix]

---

### GEO Opportunities

[High-impact changes to improve AI citation likelihood]

1. **[Opportunity]**: [Why it matters for AI] → [How to implement]

---

### SEO Improvements

[Traditional optimization recommendations]

1. **[Improvement]**: [Current state] → [Recommended change]

---

### Quick Wins

[Easy, fast improvements that take minimal effort]

- [ ] [Quick fix 1]
- [ ] [Quick fix 2]
- [ ] [Quick fix 3]

---

### Detailed Findings

#### Meta & Technical
[Checklist of what's present/missing]

#### Content Structure
[Analysis of heading hierarchy, lists, tables, etc.]

#### GEO Elements
[Statistics, quotes, quotable content found]

#### E-E-A-T Signals
[Author info, trust signals found]

#### Content Quality
[Word count, readability assessment]

---

### Summary

[2-3 sentence summary of overall status and top priority actions]
```

---

## Key 2026 Context

### Why GEO Matters
- Gartner predicts 25% drop in traditional search due to AI chatbots
- 63% of marketers now prioritize GEO
- AI Overviews causing up to 40% traffic losses for some publishers
- Content that gets **cited** by AI systems gains new visibility channel

### What Works for GEO
- Statistics with clear sources (+41% citation improvement)
- Expert quotations with attribution
- Comprehensive, authoritative content
- Clear structure AI can parse
- Self-contained, quotable sections

### What Hurts GEO
- Keyword stuffing (performs worse than natural language)
- Thin, superficial content
- Missing author/expertise signals
- Poor content structure
- No cited sources or data

---

## Example Analysis Patterns

**Good for GEO**:
```html
<p>According to a 2025 Stanford study, <strong>73% of enterprises</strong>
now use AI-assisted development tools, up from 45% in 2023.</p>
```

**Poor for GEO**:
```html
<p>Many companies use AI tools these days. It's becoming more popular.</p>
```

**Good structure**:
```html
<h2>What is GEO?</h2>
<p><strong>GEO (Generative Engine Optimization)</strong> is the practice of
optimizing content to appear in AI-generated responses...</p>
```

**Poor structure**:
```html
<div class="section">
<span class="title">What is GEO?</span>
<span>GEO means optimizing for AI...</span>
</div>
```
