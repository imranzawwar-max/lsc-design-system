---
name: lsc-brochure-design
description: LSC Brochure Design Skill — produces complete programme brochures in McKinsey publication style with full LSC branding. Use when the user wants to create a brochure, prospectus, participant guide, or programme publication for any LSC programme, course, or event. Produces a high-fidelity HTML visual mockup at A4 proportions with correct LSC palette, typographic system, and page architecture, plus Figma construction specifications. Invoke with /lsc-brochure-design.
---

# LSC Brochure Design Skill

A specialist brochure production skill for the London Strategy Centre. When invoked, it designs a complete programme brochure in McKinsey publication style — structural layout, typographic system, and page architecture — with full LSC branding applied. Output is a published HTML artifact showing all pages as high-fidelity visual mockups, plus Figma construction specifications.

## When to invoke this skill

Use this skill when the user:
- Wants to create a brochure for an LSC programme, course, or event
- Asks for a "McKinsey-style" publication with LSC branding
- Wants to design a programme guide, prospectus, or participant brochure
- Asks to produce a brochure for a specific named programme (e.g. Advanced Strategy Programme, Board Leadership Programme)
- Wants a Figma-ready specification for a new brochure

Do NOT use this skill for design extraction/analysis of existing documents. That is a different task.

---

## Input

The user must provide some or all of the following before you begin:

**Required (always ask before proceeding):**
- Programme name (full title)
- Programme type (open enrolment / in-company / executive short course / etc.)
- Target audience (who this brochure is for)
- **Number of pages** — always ask this explicitly. Do not assume or default. Suggested range: 4–16 pages. Ask: "How many pages should this brochure be?"

**Strongly recommended:**
- Programme overview (1–3 paragraph description)
- Programme structure (modules, days, schedule)
- Key outcomes or benefits (3–6 bullet points)
- Faculty names and bios (or "TBC")
- Dates and location(s)
- Fee / investment level (or "on request")
- Application/contact details

**Optional:**
- Any specific pages to include or exclude
- Special emphasis or tone notes

If any required information is missing, ask for it before proceeding. Do not design a brochure with placeholder [PROGRAMME NAME] fields — get the real content first. Do not begin designing until the page count is confirmed.

---

## Design System: McKinsey Structure + LSC Brand

### Page Architecture (McKinsey structural template)

Apply this structure scaled to the confirmed page count. The page types below are the full 8-page reference template — compress or expand it to fit the number the user specified. Never add or remove pages beyond what was confirmed.

| Page | Type | Purpose |
|------|------|---------|
| 1 | Cover | Full-bleed dark background, programme title, executive subtitle, LSC logo |
| 2 | Programme Overview | Dark background, 3-column intro with headline stat or positioning statement |
| 3 | Who Should Attend | Light background, 3-column grid, participant profile bullets |
| 4 | Programme Structure | Light background, detailed module/schedule table |
| 5 | Learning Outcomes | Dark background, 3-column outcomes with accent markers |
| 6 | Faculty | Light background, faculty cards with photo zones, names, titles, bios |
| 7 | Logistics & Investment | Light background, dates / venue / fee / application process |
| 8 | Back Cover | Dark background, LSC contact details, website, logo, social handles |

Scale to the confirmed page count:
- **4 pages:** Cover → Overview + Structure → Faculty + Logistics → Back Cover
- **6 pages:** Cover → Overview → Who Attends + Structure → Outcomes → Faculty → Logistics + Back Cover
- **8 pages:** Full template above
- **10–12 pages:** Add programme deep-dives, testimonials, or case study pages between Faculty and Logistics
- **14–16 pages:** Add module detail pages, partner pages, or alumni pages

### LSC Brand Palette

Apply these exact values throughout. Do not use McKinsey's original navy/cyan palette or any other colour not listed here.

```
LSC Navy (Primary):    #002060  (RGB 0,32,96 — dark backgrounds, headings, key graphical elements)
Primary Text:          #000000  (body text, tables, chart labels, captions)
Secondary Text:        #4D4D4D  (supporting text, notes, secondary information)
Tertiary Text:         #7A7A7A  (footnotes, sources, low-priority information)
White:                 #FFFFFF  (reverse typography on dark, backgrounds, dividers on dark)
Light Grey:            #F2F2F2  (table fills, alternate row shading, background panels)
Medium Grey:           #D9D9D9  (borders, dividers, secondary graphic elements)
Chart Tertiary:        #A6A6A6  (third data series in charts and infographics)
```

**Reverse colour rule (dark background sections):**
- Background: #002060
- Text: #FFFFFF only — no grey text on navy
- Icons, dividers, graphical accents: #FFFFFF
- Never use grey text on a navy background

**Chart and infographic series:**
- Primary series: #002060
- Secondary series: #4D4D4D
- Tertiary series: #A6A6A6
- Gridlines: #D9D9D9
- Highlight series: #002060

### Typography System

Use system fonts only in the HTML artifact (no external CDN). Map them to the McKinsey typographic roles:

| Role | McKinsey Equivalent | HTML/CSS Stack | Size | Weight |
|------|--------------------|----|------|--------|
| Display / Cover Title | McKinsey Serif Display | Georgia, 'Times New Roman', serif | 44–52pt | 700 |
| Section Title | McKinsey Serif | Georgia, 'Times New Roman', serif | 28–34pt | 700 |
| Column Heading | McKinsey Sans Bold | system-ui, -apple-system, 'Segoe UI', sans-serif | 13pt | 700 |
| Sub-heading | McKinsey Sans Medium | system-ui, -apple-system, 'Segoe UI', sans-serif | 11pt | 600 |
| Body Text | McKinsey Sans Regular | system-ui, -apple-system, 'Segoe UI', sans-serif | 9.5–10pt | 400 |
| Captions | McKinsey Sans Light | system-ui, -apple-system, 'Segoe UI', sans-serif | 8pt | 300 |
| Table Text | McKinsey Sans Regular | system-ui, -apple-system, 'Segoe UI', sans-serif | 9pt | 400 |
| Page Number | McKinsey Sans Regular | system-ui, -apple-system, 'Segoe UI', sans-serif | 8pt | 400 |
| Specs / Measurements | Monospace | 'Courier New', 'Lucida Console', monospace | 9pt | 400 |

### Grid System (A4 Portrait — 210mm × 297mm)

```
Page dimensions:   210mm × 297mm
Margins:           Top 18mm / Bottom 16mm / Left 18mm / Right 18mm
Content width:     174mm
Content height:    263mm
Footer zone:       10mm from bottom margin

3-column grid (default for content pages):
  Column width:    52mm
  Gutter:          9mm
  Col 1 start:     18mm from left
  Col 2 start:     79mm from left
  Col 3 start:     140mm from left

2-column grid (for faculty / logistics pages):
  Column width:    81mm
  Gutter:          12mm
  Col 1 start:     18mm from left
  Col 2 start:     111mm from left

Full-bleed zone:   0mm to 210mm × 0mm to 297mm
```

### McKinsey Design Language — LSC Colour Application

Apply these rules to every page:

1. **Dark pages** (#002060 background): all text #FFFFFF, all dividers and graphical accents #FFFFFF, no grey text. LSC logo reversed to white at top-right or bottom-right.
2. **Light pages** (#FFFFFF or #F2F2F2 background): main headings #002060, body text #000000, supporting/secondary text #4D4D4D, footnotes #7A7A7A. LSC logo in #002060 at footer.
3. **Accent rule**: a 2pt horizontal rule — #002060 on light pages, #FFFFFF on dark pages — 40–80mm wide, sits between the section label and the section heading on every page.
4. **Section label**: ALL CAPS, 8pt, 150–200 letter-spacing, placed 4mm above the accent rule. Colour: #002060 on light pages, #FFFFFF on dark pages.
5. **Photo treatment**: photography areas shown as placeholder divs with a dark overlay (#002060 at 40% opacity). For faculty pages, circular photo zones (48mm diameter).
6. **Footer**: every page has a 10mm footer zone. Dark pages: #FFFFFF text. Light pages: #4D4D4D text. Always includes page number (right-aligned) and LSC website (left-aligned or centred). Footer divider: #D9D9D9 on light pages, #FFFFFF at 30% opacity on dark pages.
7. **Table headers**: #002060 background, #FFFFFF text, 9pt bold. Alternating rows: #F2F2F2 and #FFFFFF. Cell borders: 0.5pt #D9D9D9.
8. **Cover page**: full-bleed #002060. Programme title in Georgia 48pt #FFFFFF. Subtitle in sans 13pt #FFFFFF (secondary weight). LSC logo top-right 30mm, reversed white. A horizontal white rule 174mm wide at ~75% page height separating the title from the lower contact strip.
9. **General principle**: the palette is monochromatic navy and grey — no accent colours, no tints other than those listed. Maintain a clean, premium consulting-firm appearance. All decorative elements use #002060, #FFFFFF, or #D9D9D9 only.

---

## Instructions

### Phase 1 — Gather and plan

1. Confirm all programme content is in hand (see Input section above)
2. Determine the page count and page type sequence
3. Decide which pages use dark vs light background treatment
4. Note any content that requires special page types (e.g. testimonials, case studies, partner logos)
5. Plan the typography hierarchy for this specific programme — which heading will be the longest? Does it need size adjustment?

### Phase 2 — Write the copy

Before designing, write all content for every page:

- Do not use placeholder text
- Write body copy at programme-brochure register: executive, precise, outcome-focused
- Bullet points maximum 12 words each
- Section labels: short ALL CAPS (e.g. "THE PROGRAMME", "WHO ATTENDS", "YOUR FACULTY")
- Module names: clear, distinctive, not generic (e.g. "Strategic Clarity Under Uncertainty" not "Module 1")
- Faculty bios: 40–60 words each, third person, credential-first

### Phase 3 — Build the HTML artifact

Design every page as a CSS visual mockup rendered at A4 proportions (scale to fit screen width). Each page must look like a real brochure page, not a wireframe.

Apply the full LSC design system throughout: correct palette, typography sizes, grid positions, and component styles. The artifact is a design proof — it should be presentable to a client or design team as a visual reference.

**Do not produce a wireframe. Produce a visual design mockup.**

---

## Output Format

Produce a **published HTML artifact** using the Artifact tool.

### Artifact structure

**Masthead:** Dark navy (#002060) header band showing:
- "LSC BROCHURE DESIGN" in white small caps
- Programme name
- Page count and date

**Navigation:** Sticky page-jump bar linking to each brochure page (Page 1 through Page N)

**Page mockups:** Each page rendered as a scaled A4 rectangle (CSS aspect-ratio 210/297) with:
- All design elements positioned correctly using CSS (flex/grid, absolute positioning within relative containers)
- Real written content — not dummy text
- Photo placeholder zones with appropriate overlay treatment
- Logo placeholder (LSC initials in correct colour treatment if no SVG available)
- Correct typography, colour, spacing as per the design system
- Page number label above each mockup: "Page 1 — Cover" etc.

**Figma Specifications:** After each page mockup, a collapsible specification panel in monospace containing:
```
CANVAS
  Size: 210 × 297mm | 794 × 1123px @96dpi
  Background: #002060

LAYER: Section Label
  Text: "THE PROGRAMME"
  Font: Segoe UI / system-ui, 8pt, weight 700
  Color: #FFFFFF
  Position: top 18mm, left 18mm
  Letter-spacing: 180

LAYER: Accent Rule
  Shape: Rectangle 80mm × 2pt
  Fill: #FFFFFF
  Position: top 26mm, left 18mm

... (continue for every layer)
```

**Style Guide:** Final section summarising:
- Full colour palette with CSS swatches
- Typography scale
- Grid dimensions
- Component list with specs

### Artifact design palette (for the artifact container itself — not the brochure content)

The artifact container (outside the page mockups) uses a neutral presentation palette that does not compete with the brochure pages:
- Background: #F2F2F2 (light grey — matches LSC neutral)
- Text: #000000
- Accent: #002060 (LSC Navy — page labels, navigation active state)
- Surface: #FFFFFF
- Dividers: #D9D9D9

Favicon: 🖊️

### Required artifact features

- Sticky navigation linking to each page mockup
- Every page mockup at correct A4 aspect ratio, min-width 500px
- Real programme content throughout (no placeholder text)
- Photo placeholder zones shown as correctly-coloured divs (not grey boxes)
- All CSS inline — no external stylesheet or font CDN calls
- `prefers-reduced-motion` respected
- No horizontal body scroll — page mockups scroll vertically within their own containers if needed
- Collapsible Figma spec panels (CSS details/summary or similar)
- Style guide section at end

---

## Completion checklist

Before publishing the artifact, verify:
- [ ] All programme content is real — no [PLACEHOLDER] fields
- [ ] Every page designed (cover through back cover — no page skipped)
- [ ] LSC palette applied correctly — only #002060, #000000, #4D4D4D, #7A7A7A, #FFFFFF, #F2F2F2, #D9D9D9, #A6A6A6 used. No other colours.
- [ ] All pages at correct A4 aspect ratio
- [ ] Dark/light page alternation follows McKinsey structural pattern
- [ ] Section labels in ALL CAPS with accent rule
- [ ] Typography sizes and weights match the system
- [ ] Figma spec panel present for every page
- [ ] Style guide section present at end
- [ ] Artifact published with favicon 🖊️
- [ ] Sticky navigation links to every page
- [ ] No external CDN calls

---

## Invocation note

Invoke with `/lsc-brochure-design` in a Claude Code session. Provide programme details at invocation or the skill will ask for them before proceeding.

The canonical version of this skill file is maintained at:
`C:\Users\born2\OneDrive - London Strategy Centre\LSC - Team Site\Automations\Claude Skills\LSC Brochure Design Skill.md`
