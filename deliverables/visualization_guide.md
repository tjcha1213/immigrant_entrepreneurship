# Visualization Implementation Guide
## Chart-by-Chart Specifications for the 5-Act Narrative (REVISED)

**Last Updated:** March 2026
**Revision Note:** Updated to match revised research data. Added methodological overlay requirements per instructor feedback. All visualizations must include source attribution, definition notes, and key caveats.

---

## General Requirements for ALL Visualizations

Every chart must include:
1. **Source attribution** (e.g., "Source: American Immigration Council, 2025")
2. **Definition used** (e.g., "Includes both first-generation immigrants and children of immigrants")
3. **Time period** (e.g., "Based on FY 2024 revenue data")
4. **Methodological note** where applicable (see chart-specific notes below)

---

## Act 1 — Hook: "How Many Services Did You Use Today?"

### Chart 1.1: Daily Services Icon Grid
- **Type:** Interactive icon grid / logo wall
- **Tool:** Flourish (Scrollytelling)
- **Data:** `research/act2_scale/key_datapoints.md` → Section F (Notable Companies)
- **Design:** Display recognizable company logos (Google, YouTube, Zoom, Tesla, WhatsApp, Stripe, eBay, DoorDash, NVIDIA); on hover/click, reveal founder name, country of origin, and "Founded by an immigrant from [country]"
- **Interaction:** Progressive reveal — logos appear one by one as user scrolls

---

## Act 2 — Scale: "The Immigrant Premium"

### Chart 2.1: Big Number + Donut Chart — Fortune 500
- **Type:** Donut chart with central big number
- **Tool:** Datawrapper
- **Data:** `research/act2_scale/key_datapoints.md` → Section B
- **Key Number:** 46.2% / 231 of 500
- **Segments:** Immigrant-founded (109), Children of immigrants (122), Non-immigrant-founded (269)
- **Annotation:** "$8.6 trillion in annual revenue — larger than any economy except the U.S. and China"

### Chart 2.2: "The Immigrant Premium" Waffle/Bar Chart
- **Type:** Waffle chart (100-square grid) series OR grouped horizontal bar chart
- **Tool:** Datawrapper or Flourish
- **Data:** `research/act2_scale/key_datapoints.md` → Section A
- **Design:** For each metric, show population share (14-15%) vs. contribution share; vertical reference line at 14-15% baseline
- **Metrics (ascending):** Labor force (17.1%), Business owners (21.7%), New entrepreneurs (~25%), Patents direct (23%), Patents total (36%), Fortune 500 (46.2%), Unicorn founders (55%)
- **Color:** Population baseline in gray; contribution in bold color
- **Required caveat footnote:** "Metrics come from different sources with different definitions and time periods. Not directly comparable. Fortune 500 includes 2nd generation; patent data is first-generation only."

### Chart 2.3: Unicorn Growth — Small Multiples
- **Type:** Small multiples (three scaled circle/square charts) or line chart
- **Tool:** Flourish
- **Data:** `research/act3_ecosystem/visualization_data.md` → Table 11
- **Design:** Three proportional area charts for 2016, 2018, 2022, each showing total unicorns as outer shape and immigrant-founded as filled portion
- **Key data:** 2016: 44/87 (51%), 2018: 50/91 (55%), 2022: 319/582 (55%)
- **Annotation:** "538% increase in absolute numbers while proportion stayed stable at ~55%"
- **IMPORTANT:** Only 3 NFAP data points exist (2016, 2018, 2022). Do NOT interpolate between years.

### Chart 2.4: Market Cap Treemap
- **Type:** Treemap
- **Tool:** Flourish or Tableau
- **Data:** `research/act2_scale/key_datapoints.md` → Section G
- **Design:** Rectangle sizes proportional to market cap; NVIDIA (~$5.0T), Apple* (~$4.0T), Alphabet (~$3.0T), Amazon* (~$2.5T), Tesla (~$1.6T), Broadcom* (~$1.0T)
- **Color-code:** First-generation immigrant founder vs. child of immigrant
- **Annotation:** "These 6 immigrant-connected companies = ~28% of the S&P 500 (~$17.1T combined)"
- **Required caveat:** "Market caps approximate as of early 2026; fluctuate daily. *Apple, Amazon, Broadcom founded by children of immigrants."

---

## Act 3 — Who / Where / What

### Chart 3.1: World Choropleth Map — Countries of Origin
- **Type:** Choropleth world map
- **Tool:** Tableau
- **Data:** `research/act3_ecosystem/visualization_data.md` → Table 1 + Table 13 (coordinates)
- **Color intensity:** Number of billion-dollar companies founded
- **Interaction:** Hover to see country name, company count, top industries, notable companies
- **Highlight:** India (66), Israel (54), UK (27), Canada (22), China (21)

### Chart 3.2: Country × Industry Heatmap
- **Type:** Heatmap matrix
- **Tool:** Flourish or Tableau
- **Data:** `research/act3_ecosystem/visualization_data.md` → Table 2
- **Rows:** Top 15 origin countries
- **Columns:** 10 industry sectors
- **Color scale:** 0 (none) to 5 (world-leading)
- **Key patterns to highlight:** India→AI/SaaS, Israel→Cybersecurity, China/Taiwan→Hardware

### Chart 3.3: U.S. State Choropleth — Startup Density
- **Type:** U.S. choropleth map
- **Tool:** Tableau
- **Data:** `research/act3_ecosystem/visualization_data.md` → Table 3 + Table 14 (city coordinates)
- **Color intensity:** Number of immigrant-founded companies
- **Bubble overlay:** City-level bubbles sized by startup count/valuation
- **Highlight:** California (66%), New York (16%), Massachusetts (10%)

### Chart 3.4: Bubble Chart — Companies by Origin × Industry × Valuation
- **Type:** Bubble chart
- **Tool:** Flourish
- **Data:** `research/act3_ecosystem/visualization_data.md` → Table 6
- **X-axis:** Industry category
- **Y-axis:** Valuation (log scale)
- **Bubble size:** log(employees)
- **Bubble color:** Origin country/region
- **Top bubbles:** NVIDIA ($3T+), Alphabet ($2.2T), Tesla ($1.1T), SpaceX ($350B)
- **Required caveat:** "Public companies use market cap; private companies use last known funding round valuation."

### Chart 3.5: Sankey Diagram — Origin → U.S. City → Industry
- **Type:** Sankey / alluvial diagram
- **Tool:** Flourish
- **Data:** `research/act3_ecosystem/visualization_data.md` → Table 5
- **Left column:** Origin countries (India, Israel, China, Iran, Ireland, etc.)
- **Middle column:** U.S. destination cities (Silicon Valley, NYC, Boston, etc.)
- **Right column:** Industry sectors (AI, Cybersecurity, Fintech, etc.)
- **Flow width:** Relative connection strength (1-40 scale; NOT absolute company counts)
- **Required note:** "Flow weights are relative measures indicating strength of connection, not exact company counts."

### Chart 3.6: Visa Pathway Pie Chart (ILLUSTRATIVE ONLY)
- **Type:** Pie/donut chart
- **Tool:** Datawrapper
- **Data:** `research/act3_ecosystem/visualization_data.md` → Table 10
- **Segments:** F-1 Student (72%), H-1B Work (15%), O-1 Extraordinary (3%), EB-1 (3%), L-1 (2%), Other (5%)
- **Key insight:** "72% of AI immigrant founders first came as students"
- **CRITICAL REQUIRED CAVEAT:** "These percentages are from a small-sample CSET study of Forbes AI 50 founders (2019) with significant survivorship bias. Individual visa pathway data is NOT systematically available. This chart is ILLUSTRATIVE, not comprehensive. Categories labeled 'Estimate' are rough approximations."
- **Visual treatment:** Use dotted borders or reduced opacity to signal uncertainty

---

## Act 4 — The Policy Reality

### Chart 4.1: H-1B Denial Rate — Animated Line Chart with Policy-Era Bands
- **Type:** Animated line chart with background era bands and event annotations
- **Tool:** Flourish or Tableau
- **Data:** `research/act4_policy/timeline_data.md` → Dataset 1
- **X-axis:** Fiscal Year 2010-2025
- **Y-axis:** H-1B Denial Rate (%)
- **Background bands:** Obama (#3B82F6, 15% opacity), Trump 1 (#EF4444), Biden (#3B82F6), Trump 2 (#DC2626)
- **Annotations:** Vertical lines with labels at key policy events (BAHA, Travel Ban, ITServe, PA-2021-05, $100K fee) — see timeline_data.md Annotation Points table
- **Animation:** Progressive reveal, left to right, pausing at each era transition
- **Peak highlight:** 24% denial rate in FY 2018 (4x the FY 2015 level)
- **Required methodological note overlay:** "Denial rates reflect USCIS adjudication policy. Temporal co-occurrence with policy changes does not establish causation."

### Chart 4.2: Policy Event Timeline
- **Type:** Horizontal scrolling timeline
- **Tool:** Flourish (Timeline template)
- **Data:** `research/act4_policy/timeline_data.md` → Dataset 5 (35 events)
- **Design:** Events above line = expansive; below line = restrictive
- **Size:** Scaled by significance (critical > high > medium)
- **Color:** By era (Obama, Trump1, Biden, Trump2)
- **Underlay:** H-1B denial rate line running beneath

### Chart 4.3: Green Card Backlog Bar Chart
- **Type:** Grouped bar chart
- **Tool:** Datawrapper
- **Data:** `research/act4_policy/timeline_data.md` → Dataset 6
- **X-axis:** Visa categories (EB-1, EB-2, EB-3)
- **Y-axis:** Wait time in years
- **Groups:** India, China, Rest of World
- **Key highlights:** India EB-2 = 12-18 years; India EB-1 = 3-4 years
- **Annotation:** "134-year theoretical wait for new EB-2 India applicants (Boundless, 2024)"
- **Context label:** "Annual cap: 140,000 (set in 1990, never updated)"

### Chart 4.4: Brain Drain KPI Dashboard Cards
- **Type:** 4-6 large number cards with trend arrows
- **Tool:** Custom HTML or Datawrapper
- **Data:** `research/act4_policy/timeline_data.md` → Dataset 7
- **Cards:**
  - "75%" — Scientists considering leaving the U.S. (Nature 2025 survey, n=1,600)
  - "82%" — Employers who lost workers to visa issues (Envoy Global 2023)
  - "1.8M" — Employment-based green card backlog (Cato 2024)
  - "3x" — Increase in ERC grant applications from U.S. (2024→2026)
  - "$100K" — New H-1B petition fee (Sept 2025)
  - "134 years" — Theoretical EB-2 India wait time
- **Required note:** "Brain drain indicators describe talent movement patterns but cannot isolate immigration policy as the sole driver."

### Chart 4.5: H-1B Nationality Breakdown (Stacked Area)
- **Type:** Stacked area chart
- **Tool:** Flourish or Tableau
- **Data:** `research/act4_policy/timeline_data.md` → Dataset 4
- **X-axis:** FY 2010-2024
- **Y-axis:** Approvals percentage
- **Stacks:** India (largest), China, Other
- **Key point:** India's share grew from ~50% (2001-2015 avg) to ~73% (2023)
- **Required note:** "Historical data prior to FY 2019 requires interpolation from period averages; data_quality column indicates confidence."

### Chart 4.6: Policy Era Comparison (Small Multiples)
- **Type:** Four-column comparison grid
- **Tool:** Custom HTML or Flourish
- **Data:** `research/act4_policy/timeline_data.md` → Dataset 11
- **Columns:** Obama, Trump 1, Biden, Trump 2
- **Rows:** Denial rate range, RFE rate peak, H-1B fee level, travel restrictions, signature policy

### Chart 4.7: Slope Chart — Before/After Key Policy Changes
- **Type:** Connected slope lines
- **Tool:** Flourish
- **Data:** `research/act4_policy/timeline_data.md` → Dataset 12
- **Pairs:** Pre-BAHA vs post-BAHA (denial), Pre-Biden vs post-Biden (denial), Pre-$100K vs post-$100K (fee)

---

## Act 5 — So What? The Cost of Restriction

### Chart 5.1: Scenario Comparison — GDP / Workforce / Debt (Three Sub-Panels)
- **Type:** Grouped bar chart with three sub-panels
- **Tool:** Datawrapper
- **Data:** `research/act5_projections/scenario_data.md` → Visualization 1
- **Bars:** Restriction (red), Status Quo (gray), Reform (green)
- **Sub-panels:** GDP Impact | Workforce Impact | Federal Debt Impact
- **GDP:** -$12.1T (NFAP) vs baseline vs +$456B (Hoover, H-1B only)
- **Workforce:** -15.7M workers (NFAP) vs baseline (Reform bar N/A from comparable source)
- **Debt:** +$1.74T (NFAP) vs baseline vs -$113B tax revenue (Hoover)
- **CRITICAL annotation:** "Reform figure reflects H-1B expansion only (Hoover); Restriction/Status Quo from NFAP comprehensive analysis. These are from different models and not directly comparable."

### Chart 5.2: 1920s Historical Precedent — Before/After Comparison
- **Type:** Paired horizontal bars
- **Tool:** Flourish
- **Data:** `research/act5_projections/scenario_data.md` → Visualization 2
- **Three pairs:** Immigration Volume (-54%), Invention Rate in ESE fields (-68%), Native Scientist Patents (-45%)
- **Colors:** Before (blue) vs. After (red)
- **Timeline arrow:** "Effects lasted ~40 years (into the 1960s)"
- **Key annotation:** "Even native-born scientists became less productive when immigrant colleagues were excluded"
- **Source:** Moser & San, AEA 2020

### Chart 5.3: Global Talent Competition Radar/Spider Chart
- **Type:** Overlaid radar/spider charts
- **Tool:** Flourish or Tableau
- **Data:** `research/act5_projections/scenario_data.md` → Visualization 7
- **Axes (5):** Processing Speed, Startup Pathway, No Cap/Quota, Merit-Based Selection, Portability
- **Countries:** US (red, smallest polygon), Canada (blue), UK (purple), Germany (gold), Singapore (teal)
- **Score scale:** 1-5 (OUR EXTRAPOLATION — label as subjective assessment)
- **Required footnote:** "Scores are our assessment based on documented program characteristics."

### Chart 5.4: Counter-Argument Evidence Bar Chart
- **Type:** Horizontal bars with verdict badges
- **Tool:** Datawrapper
- **Data:** `research/act5_projections/scenario_data.md` → Visualization 4
- **Claims (sorted by evidence strength):**
  - "H-1B workers displace Americans" — LARGELY FALSE (Richmond Fed 2025)
  - "Immigrants are a fiscal burden" — LARGELY FALSE (Cato $14.5T surplus)
  - "We can innovate without immigrants" — LARGELY FALSE (NBER 36% patents)
  - "Restricting immigration protects jobs" — LARGELY FALSE (NBER offshoring)
  - "H-1B workers suppress wages" — MIXED (firm-level yes, economy-wide no)
  - "Too many immigrants lower quality" — MIXED
- **Badge colors:** Green = LARGELY FALSE, Yellow = MIXED
- **Brief evidence annotation** next to each bar

### Chart 5.5: Waterfall Chart — Cumulative Fiscal Impact ($14.5T)
- **Type:** Waterfall chart
- **Tool:** Custom or Flourish
- **Data:** `research/act5_projections/scenario_data.md` → Visualization 5
- **Steps:** Direct immigrant tax revenue (14% of all revenue) → Immigrant spending (7% of all spending) → Net direct surplus (~$10.6T) → Interest savings ($3.9T) → Total $14.5T
- **Counterfactual annotation:** "Without immigrants, debt-to-GDP would be at least 205% (Cato)"
- **Source:** Cato Institute, building on NASEM fiscal model (1994-2023)

### Chart 5.6: Diverging Bar Chart — Jobs Offshored vs. Retained
- **Type:** Diverging horizontal bars centered on zero
- **Tool:** Flourish or custom
- **Data:** `research/act5_projections/scenario_data.md` → Visualization 6
- **Left (red):** Jobs leaving the U.S. (0.3x avg MNC, 0.9x globalized)
- **Right (green):** Jobs staying (filled H-1B positions)
- **Three rows:** Reform / Status Quo / Further Restriction
- **Required caveat:** "Offshoring ratios (0.3x, 0.9x) from Glennon (NBER). Aggregate projections are illustrative extrapolations."

---

## Scrollytelling Page Structure (Flourish Story)

```
Section 1: [Hook]           → Icon grid of daily-use companies (Chart 1.1)
Section 2: [Scale - F500]   → Big numbers + donut chart (Charts 2.1)
Section 3: [Scale - Data]   → Immigrant Premium waffle/bar + treemap (Charts 2.2, 2.4)
Section 4: [Scale - Growth] → Unicorn growth small multiples (Chart 2.3)
Section 5: [World Map]      → Choropleth + heatmap + bubble chart (Charts 3.1, 3.2, 3.4)
Section 6: [U.S. Map]       → State choropleth + Sankey diagram (Charts 3.3, 3.5)
Section 7: [Visa]           → Visa pathway (illustrative) (Chart 3.6)
Section 8: [Policy]         → Animated denial rate line chart + era comparison (Charts 4.1, 4.6)
Section 9: [Timeline]       → Policy events timeline (Chart 4.2)
Section 10: [Backlog]       → Green card wait times + slope chart (Charts 4.3, 4.7)
Section 11: [Brain Drain]   → KPI dashboard cards + nationality breakdown (Charts 4.4, 4.5)
Section 12: [Cost]          → Scenario bars + 1920s comparison (Charts 5.1, 5.2)
Section 13: [Fiscal]        → Waterfall chart ($14.5T) (Chart 5.5)
Section 14: [Offshoring]    → Diverging bar chart (Chart 5.6)
Section 15: [Competition]   → Radar chart + counter-arguments (Charts 5.3, 5.4)
Section 16: [Close]         → Key takeaways for policymakers
```

---

## Color Palette Recommendations

| Element | Color | Hex |
|---------|-------|-----|
| Immigrant-founded | Deep Blue | #1B4F72 |
| Non-immigrant | Light Gray | #D5D8DC |
| Obama era | Blue | #2980B9 |
| Trump era | Red | #C0392B |
| Biden era | Blue | #3498DB |
| Positive impact | Green | #27AE60 |
| Negative impact | Red | #E74C3C |
| Neutral | Gray | #95A5A6 |

**Accessibility:** All color combinations pass WCAG AA contrast requirements. Include patterns/textures as secondary encoding for colorblind accessibility.

---

## Data Confidence Visual Encoding Guide

| Confidence Level | Description | Visual Encoding |
|-----------------|-------------|-----------------|
| High | Direct from NFAP/AIC primary reports | Solid colors, full opacity |
| Medium | Derived via calculation or cross-referencing | Reduced opacity, dashed borders |
| Low | Small-sample estimates, survivorship bias | Low opacity, dotted borders, "estimated" label |
| Estimated | Gap-filled for visualization completeness | Hatched fill pattern, footnote marker |

---

*Implementation Guide · Harvard Data Visualization Group Project · Spring 2025*
*Revised March 2026 per instructor feedback on methodological rigor*
