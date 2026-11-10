# Act 5 -- Structured Datasets for Visualizations (REVISED)

## Data Source Classification Key

Every data point in this file is classified:
- **(SOURCED)** -- Directly reported by the cited study
- **(CITED PROJECTION)** -- Modeled/projected by the cited study
- **(OUR EXTRAPOLATION)** -- Our own calculation or extension from cited data; labeled with reasoning

---

## Visualization 1: Scenario Bar Chart -- 3 Bars (Restriction / Status Quo / Reform)

### Purpose
Three grouped bars comparing GDP, jobs, and debt outcomes across policy scenarios.

### GDP Impact (Cumulative, 2025-2035)

| Scenario | Cumulative GDP Impact | Annual Growth Rate | Classification | Source |
|----------|----------------------|-------------------|----------------|--------|
| Restriction | -$12.1 trillion vs. baseline | 1.3% avg | CITED PROJECTION | [NFAP Oct 2025](https://nfap.com/wp-content/uploads/2025/10/Economic-Impact-of-The-Trump-Administration-Immigration-Policies.NFAP-Policy-Brief.2025-1.pdf) |
| Status Quo | Baseline (CBO projection) | 1.8% avg | CITED PROJECTION | [NFAP Oct 2025](https://nfap.com/wp-content/uploads/2025/10/Economic-Impact-of-The-Trump-Administration-Immigration-Policies.NFAP-Policy-Brief.2025-1.pdf) (CBO baseline used) |
| Reform (H-1B expansion only) | +$456B over 10 years | ~2.0% avg (est.) | CITED PROJECTION (Hoover) + OUR EXTRAPOLATION (growth rate) | [Hoover Institution](https://www.hoover.org/research/additional-h-1b-workers-would-add-billions-gdp-and-federal-tax-revenue) |

**IMPORTANT VISUALIZATION NOTE:** The Restriction and Status Quo bars come from the same NFAP study and are directly comparable. The Reform bar comes from the Hoover Institution and covers ONLY H-1B expansion (not all immigration reform). These are not from the same model. Annotate this on the chart: "Reform figure reflects H-1B expansion only (Hoover); Restriction/Status Quo from NFAP comprehensive analysis."

### Workforce Impact (10-Year, by 2035)

| Scenario | Workforce Change | Classification | Source |
|----------|-----------------|----------------|--------|
| Restriction | -15.7 million workers | CITED PROJECTION | [NFAP Oct 2025](https://nfap.com/wp-content/uploads/2025/10/Economic-Impact-of-Trump-Admin-Immigration-Pollicies.DAY-OF-RELEASE.Oct-2025-1.pdf) |
| Status Quo | Baseline (CBO) | CITED PROJECTION | CBO baseline |
| Reform (H-1B expansion) | Net positive (not quantified in Hoover study beyond GDP/tax) | N/A | No directly comparable source |

**Note for visualization:** For the workforce bar, we have a strong sourced figure for Restriction (-15.7M from NFAP) but no directly comparable figure for Reform. Consider using only the Restriction vs. Status Quo comparison for this metric, or note that the Reform bar is not available from a comparable source.

### Federal Debt Impact (2025-2035)

| Scenario | Additional Federal Debt | Classification | Source |
|----------|------------------------|----------------|--------|
| Restriction | +$1.74 trillion | CITED PROJECTION | [NFAP Oct 2025](https://nfap.com/wp-content/uploads/2025/10/Economic-Impact-of-Trump-Admin-Immigration-Pollicies.DAY-OF-RELEASE.Oct-2025-1.pdf) |
| Status Quo | Baseline | -- | CBO baseline |
| Reform (H-1B expansion) | -$113B in added tax revenue (Hoover) | CITED PROJECTION | [Hoover Institution](https://www.hoover.org/research/additional-h-1b-workers-would-add-billions-gdp-and-federal-tax-revenue) |

**Short-term comparison (2025-2028):**

| Scenario | Additional Federal Debt | Classification | Source |
|----------|------------------------|----------------|--------|
| Restriction | +$252 billion | CITED PROJECTION | NFAP Oct 2025 |
| Status Quo | Baseline | -- | CBO |

### Chart Design Notes
- Y-axis: Dollar amounts (trillions for GDP, trillions for debt, millions for workforce)
- Colors: Red (Restriction), Gray (Status Quo), Green (Reform)
- Annotations: Source study name on each bar; footnote about different model origins
- Consider three sub-panels: GDP | Workforce | Debt

---

## Visualization 2: Before/After Comparison Bars -- 1920s Restriction Impact

### Purpose
Paired bars showing metrics before and after the Immigration Act of 1924, based on Moser & San research.

### Immigration Volume

| Period | Annual Immigration | Classification | Source |
|--------|-------------------|----------------|--------|
| Pre-1921 (Before) | ~360,000/year | SOURCED | [Moser & San (AEA 2020)](https://www.aeaweb.org/conference/2020/preliminary/paper/NydKa4TK) |
| Post-1924 (After) | ~165,000/year | SOURCED | [Moser & San (AEA 2020)](https://www.aeaweb.org/conference/2020/preliminary/paper/NydKa4TK) |
| Change | -54% decline | OUR EXTRAPOLATION | Calculated: (360K - 165K) / 360K |

### Invention Rate in Affected (ESE) Fields

| Period | Invention Output | Classification | Source |
|--------|-----------------|----------------|--------|
| Before quotas | Baseline (100%) | -- | [Moser & San](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3558718) |
| After quotas | -68% decline in ESE fields | SOURCED | [Moser & San](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3558718) |

### Native-Born Scientist Patents in ESE Fields

| Period | Patent Output by Native Scientists | Classification | Source |
|--------|-----------------------------------|----------------|--------|
| Before quotas | Baseline (100%) | -- | [Moser & San](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3558718) |
| After quotas | -45% fewer patents by U.S.-born scientists | SOURCED | [Moser & San](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3558718) |

### Fields with Zero Patents

| Period | ESE Fields with No Patents | Classification | Source |
|--------|---------------------------|----------------|--------|
| Before quotas | Baseline | -- | Moser & San |
| After quotas | 16% additional fields had zero patents | SOURCED | Moser & San |

### Duration of Effects

| Metric | Value | Classification | Source |
|--------|-------|----------------|--------|
| Duration of innovation decline | Persisted into the 1960s (~40 years) | SOURCED | Moser & San |
| Missing ESE-born scientists by 1950s | ~1,170 | SOURCED | Moser & San |

### Chart Design Notes
- Format: Paired horizontal bars for each metric (Before = blue, After = red)
- Three pairs: Immigration Volume, Invention Rate, Native Scientist Patents
- Add a timeline arrow at bottom showing "Effects lasted ~40 years (into the 1960s)"
- Annotation: "Even native-born scientists became less productive when immigrant colleagues were excluded"
- All data from a single study (Moser & San) -- methodologically consistent

---

## Visualization 3: Comparison Matrix/Scorecard -- US vs. Competitor Nations

### Purpose
Matrix or scorecard comparing the U.S. against Canada, UK, Germany, and Singapore on talent recruitment dimensions.

### Processing Time Comparison

| Country | Program Name | Processing Time | Classification | Source |
|---------|-------------|----------------|----------------|--------|
| United States | H-1B | 6-9 months (lottery) | SOURCED | [USCIS](https://egov.uscis.gov/processing-times/) |
| Canada | Global Talent Stream | 2 weeks | SOURCED | [Canada.ca](https://www.canada.ca/en/employment-social-development/services/foreign-workers/global-talent/requirements.html) |
| United Kingdom | Global Talent Visa | 2-4 months | SOURCED | [GOV.UK](https://www.gov.uk/global-talent) |
| Germany | Chancenkarte | 2-12 weeks | SOURCED | [Germany.info](https://www.germany.info/resource/blob/2663778/ab8cb2c068d1819dd3822b81231fe0b9/opportunity-card-data.pdf) |
| Singapore | Tech.Pass / ONE Pass | 4-8 weeks | SOURCED | [Singapore EDB](https://www.edb.gov.sg/en/incentives-and-programmes/incentives-and-facilitation-programmes/tech-pass.html) |

### Startup Visa Availability

| Country | Startup Visa? | Details | Classification | Source |
|---------|--------------|---------|----------------|--------|
| United States | No | No dedicated startup visa exists | SOURCED | -- |
| Canada | Yes (paused 2026) | Start-Up Visa Program; paused Jan 1, 2026; successor pilot launching | SOURCED | [Canada.ca](https://www.canada.ca/en/immigration-refugees-citizenship/services/immigrate-canada/start-visa/about.html) |
| United Kingdom | Yes (via Global Talent) | Innovator Founder visa + Global Talent pathway | SOURCED | [GOV.UK](https://www.gov.uk/global-talent) |
| Germany | Limited | Freelance/self-employment visa; no dedicated startup visa | SOURCED | [Germany.info](https://www.germany.info/resource/blob/2663778/ab8cb2c068d1819dd3822b81231fe0b9/opportunity-card-data.pdf) |
| Singapore | Yes | EntrePass for startup founders; Tech.Pass for tech entrepreneurs | SOURCED | [Singapore EDB](https://www.edb.gov.sg/en/incentives-and-programmes/incentives-and-facilitation-programmes/tech-pass.html) |

### Selection Method

| Country | Selection Method | Cap/Limit | Classification |
|---------|-----------------|-----------|----------------|
| United States | Random lottery | 85,000/year | SOURCED |
| Canada | Merit/employer-driven | No hard cap on GTS | SOURCED |
| United Kingdom | Merit/endorsement | No cap | SOURCED |
| Germany | Points-based | No hard cap | SOURCED |
| Singapore | Merit/salary threshold | Selective (no public cap) | SOURCED |

### Active Recruitment of U.S. Talent

| Country | Actively Recruiting from U.S.? | Notable Programs | Classification |
|---------|-------------------------------|-----------------|----------------|
| United States | N/A | N/A | -- |
| Canada | Yes | Microsoft Vancouver expansion; GTS 2-week processing | SOURCED |
| United Kingdom | Yes | Global Talent Visa; no job offer required | SOURCED |
| Germany | Yes | Removed language requirements for IT; Chancenkarte | SOURCED |
| Singapore | Yes | Tech.Pass; ONE Pass for top talent | SOURCED |

### Composite Scorecard (for matrix heatmap)

| Dimension | US | Canada | UK | Germany | Singapore |
|-----------|-----|--------|-----|---------|-----------|
| Processing speed | 1 | 5 | 3 | 3 | 4 |
| Startup pathway | 1 | 4 | 4 | 2 | 4 |
| Selection method | 1 | 4 | 5 | 4 | 4 |
| No cap/quota | 1 | 4 | 5 | 5 | 4 |
| Active recruitment | 1 | 5 | 4 | 3 | 4 |

**Scale: 1 (worst) to 5 (best). Classification: OUR EXTRAPOLATION based on the sourced data above. These scores are subjective assessments for visualization purposes and should be labeled as such.**

### Chart Design Notes
- Format: Matrix/heatmap with countries as columns, dimensions as rows
- Color coding: Dark green (5) to dark red (1)
- U.S. column should visually stand out as the weakest across most dimensions
- Alternative: Small multiples of bar charts for each dimension

---

## Visualization 4: Horizontal Bar Chart with Verdict Badges -- Counter-Arguments

### Purpose
Horizontal bars showing each counter-argument claim, rated by strength of evidence, with color-coded verdict badges.

### Counter-Argument Evidence Ratings

| Claim | Verdict | Badge Color | Key Evidence | Classification of Evidence | Source |
|-------|---------|-------------|-------------|---------------------------|--------|
| "H-1B workers displace Americans" | LARGELY FALSE | Green | No displacement found; firms that win H-1B lottery hire MORE native graduates | SOURCED | [Richmond Fed 2025](https://www.richmondfed.org/publications/research/economic_brief/2025/eb_25-39) |
| "Immigrants are a fiscal burden" | LARGELY FALSE | Green | $14.5T fiscal surplus (1994-2023); immigrants pay 17% more in taxes per capita | CITED PROJECTION (Cato) | [Cato Institute](https://www.cato.org/blog/cato-study-immigrants-reduced-deficits-145-trillion-1994) |
| "We can innovate without immigrants" | LARGELY FALSE | Green | 16% of inventors produce 36% of patents; 1920s restriction caused 68% invention decline in affected fields | SOURCED (NBER, Moser & San) | [NBER](https://www.nber.org/digest/20233/outsize-role-immigrants-us-innovation), [Moser & San](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3558718) |
| "Restricting immigration protects jobs" | LARGELY FALSE | Green | Firms offshore 0.3-0.9 jobs per unfilled H-1B; do NOT hire more Americans | SOURCED | [NBER/Glennon](https://www.nber.org/papers/w27538) |
| "H-1B workers suppress wages" | MIXED | Yellow | Firm-level suppression exists (60% below median); economy-wide effect is positive (+1.7-2.6%) | SOURCED (both sides) | [EPI](https://www.epi.org/publication/h-1b-visas-and-prevailing-wage-levels/), [NBER](https://www.nber.org/system/files/working_papers/w32389/w32389.pdf) |
| "Too many immigrants lower quality" | MIXED | Yellow | U.S. leads in patent importance despite lower volume; but concentration effects exist | SOURCED | [CSIS](https://www.csis.org/analysis/what-can-patent-data-reveal-about-us-china-technology-competition) |

### Chart Design Notes
- Format: Horizontal bars with claim text on Y-axis
- Bar length could represent "strength of evidence against the claim" (longer = more evidence disproving)
- Badge at end of each bar: Green circle = LARGELY FALSE, Yellow circle = MIXED
- No claims rated LARGELY TRUE (red) based on current evidence
- Include a brief "key evidence" annotation next to each bar
- Sort order: Green verdicts first (strongest evidence), then Yellow

---

## Visualization 5: Waterfall Chart -- Cumulative Fiscal Impact

### Purpose
Waterfall showing how immigrant fiscal contributions accumulated over 30 years ($14.5T total).

### Cumulative Fiscal Surplus Data

**Source:** Cato Institute, "Immigrants' Recent Effects on Government Budgets: 1994-2023"
**Methodology:** Based on NASEM fiscal model applied to 30 years of federal, state, and local budget data

| Component | Amount | Classification | Source |
|-----------|--------|----------------|--------|
| Total cumulative fiscal surplus | $14.5 trillion (real 2024 dollars) | CITED PROJECTION | [Cato](https://www.cato.org/white-paper/immigrants-recent-effects-government-budgets-1994-2023) |
| Of which: interest savings on debt | $3.9 trillion | CITED PROJECTION | [Cato](https://www.cato.org/blog/cato-study-immigrants-reduced-deficits-145-trillion-1994) |
| Of which: direct fiscal surplus | $10.6 trillion | OUR EXTRAPOLATION | Calculated: $14.5T - $3.9T |
| Immigrant share of tax revenue | 14% | SOURCED | Cato |
| Immigrant share of government spending | 7% | SOURCED | Cato |
| Per capita tax premium (immigrant vs. native) | +$100,000 (17% more) over 30 years | SOURCED | Cato |

### Waterfall Step Data (Approximate Decade Breakdown)

**IMPORTANT: The Cato study does not provide a decade-by-decade breakdown in publicly available summaries. The following is our approximation for visualization purposes only.**

| Period | Estimated Contribution | Classification | Reasoning |
|--------|----------------------|----------------|-----------|
| 1994-2003 | ~$3.5 trillion | OUR EXTRAPOLATION | Lower immigrant population; proportional estimate based on population growth |
| 2004-2013 | ~$4.5 trillion | OUR EXTRAPOLATION | Growing immigrant population; includes pre-2008 boom and recovery |
| 2014-2023 | ~$6.5 trillion | OUR EXTRAPOLATION | Largest immigrant population; highest absolute contribution period |
| Cumulative interest savings | $3.9 trillion | CITED PROJECTION | Cato study reports this as a separate component |
| **Subtotal** | **~$18.4 trillion** | -- | Note: does not sum to $14.5T because interest savings overlap with decade contributions |

**Better waterfall approach -- building blocks from sourced data:**

| Step | Amount | Classification |
|------|--------|----------------|
| Starting point: deficit without immigrants | -$48 trillion | CITED PROJECTION (Cato) |
| Immigrant tax contributions (14% of revenue) | +$14.5T surplus effect | CITED PROJECTION (Cato) |
| Ending point: actual deficit | Reduced by ~1/3 | CITED PROJECTION (Cato) |

**Alternative waterfall: Fiscal components**

| Step | Description | Direction | Classification |
|------|------------|-----------|----------------|
| 1 | Direct immigrant tax revenue (14% of all revenue) | + (positive) | SOURCED |
| 2 | Immigrant government spending (7% of all spending) | - (negative) | SOURCED |
| 3 | Net direct fiscal surplus | + ($10.6T est.) | OUR EXTRAPOLATION |
| 4 | Interest savings from lower debt | + ($3.9T) | CITED PROJECTION |
| 5 | **Total cumulative surplus** | **$14.5 trillion** | CITED PROJECTION |

### Counterfactual Comparison

| Metric | With Immigrants | Without Immigrants | Classification |
|--------|----------------|-------------------|----------------|
| Debt-to-GDP ratio (2023) | Actual ~100% | At least 205% | CITED PROJECTION (Cato) |

### Chart Design Notes
- Format: Waterfall chart building from fiscal components to total $14.5T
- Recommended approach: Use the "Fiscal components" version (Steps 1-5) above
- Colors: Green for positive contributions, red for costs, blue for net
- Final bar shows the $14.5T total
- Add a dashed line or annotation showing the 205% debt-to-GDP counterfactual
- Footnote: "Source: Cato Institute analysis building on NASEM fiscal model, covering 1994-2023"

---

## Visualization 6: Diverging Bar Chart -- Jobs Offshored vs. Retained

### Purpose
Diverging horizontal bars showing jobs going overseas (left/negative) vs. retained in U.S. (right/positive) under different H-1B denial rate scenarios.

### Core Data: Jobs per H-1B Denial

| Firm Type | Jobs Offshored per Denial | Classification | Source |
|-----------|--------------------------|----------------|--------|
| Average MNC | 0.3 | SOURCED | [Glennon, NBER WP 27538](https://www.nber.org/papers/w27538) |
| Highly globalized MNC | 0.9 | SOURCED | [Glennon, NBER WP 27538](https://www.nber.org/papers/w27538) |
| Historically H-1B-dependent firms | 27% higher offshore growth rate | SOURCED | [Glennon, NBER](https://www.nber.org/digest/sep20/restricting-visas-skilled-workers-leads-offshoring) |

### Scenario Projections Under Different Denial Rates

**Context:** The H-1B program receives approximately 400,000-780,000 registrations per year for 85,000 available slots (2023-2025 data). The effective "denial rate" in terms of unmet demand is approximately 70-90%.

| Denial Rate Scenario | Estimated Denials/Year | Jobs Offshored (avg MNC, 0.3x) | Jobs Offshored (global MNC, 0.9x) | Classification |
|---------------------|----------------------|-------------------------------|-----------------------------------|----------------|
| Low restriction (15% denial) | ~60,000 | ~18,000 | ~54,000 | OUR EXTRAPOLATION from Glennon ratios applied to approximate demand |
| Current system (~78% effective denial) | ~315,000 | ~94,500 | ~283,500 | OUR EXTRAPOLATION from Glennon ratios applied to approximate demand |
| High restriction (90%+ denial) | ~360,000+ | ~108,000 | ~324,000 | OUR EXTRAPOLATION from Glennon ratios applied to approximate demand |

**IMPORTANT CAVEAT:** The above scenario numbers are OUR EXTRAPOLATIONS. Glennon's study provides the per-denial offshoring ratios (0.3 and 0.9), which are SOURCED. We have multiplied these by estimated denial volumes to project aggregate offshoring. The actual relationship may not scale linearly. These figures should be labeled as illustrative projections in the visualization.

### Diverging Bar Data Format

For the diverging bar chart, show each scenario with:
- **Left side (negative/red):** Jobs offshored
- **Right side (positive/green):** Jobs retained in U.S. (filled H-1B positions)

| Scenario | Jobs Retained (U.S.) | Jobs Offshored (Overseas) | Net Effect | Classification |
|----------|---------------------|--------------------------|------------|----------------|
| Reform (more visas) | ~340,000 | ~18,000 to ~54,000 | Strongly positive | OUR EXTRAPOLATION |
| Status Quo | ~85,000 | ~94,500 to ~283,500 | Mixed | OUR EXTRAPOLATION |
| Further Restriction | ~42,500 (halved cap) | ~108,000 to ~324,000 | Strongly negative | OUR EXTRAPOLATION |

### Geographic Destination of Offshored Jobs

| Destination | Share of Offshoring | Classification | Source |
|-------------|-------------------|----------------|--------|
| India | Primary destination | SOURCED | [Glennon, NBER](https://www.nber.org/papers/w27538) |
| China | Major destination | SOURCED | Glennon, NBER |
| Canada | Growing destination (proximity advantage) | SOURCED | Glennon, NBER |

### Chart Design Notes
- Format: Diverging horizontal bars centered on zero
- Left (red): Jobs leaving the U.S.
- Right (green): Jobs staying in the U.S.
- Three rows: Reform / Status Quo / Further Restriction
- Include range bars to show the 0.3x to 0.9x range for each scenario
- Footnote: "Offshoring ratios (0.3x avg, 0.9x globalized MNCs) from Glennon (NBER). Aggregate projections are illustrative extrapolations."
- Consider adding small flag icons for India, China, Canada showing where jobs go

---

## Visualization 7: Radar/Spider Chart -- Country Competitiveness Comparison

### Purpose
Multi-dimensional comparison of U.S. vs. competitor nations across talent recruitment dimensions.

### Scoring Methodology

**Classification: ALL scores are OUR EXTRAPOLATION based on sourced underlying data.**

We score each country from 1-5 on each dimension based on the factual program characteristics documented in our research. The scoring rubric:

**Processing Speed (lower = better):**
- 5: Under 1 month (Canada GTS: 2 weeks)
- 4: 1-2 months (Singapore: 4-8 weeks)
- 3: 2-3 months (UK: 2-4 months; Germany: 2-12 weeks)
- 2: 3-6 months
- 1: 6+ months (US: 6-9 months)

**Startup Pathway:**
- 5: Dedicated startup visa, operational, accessible
- 4: Dedicated pathway exists with some limitations (Canada: paused but has successor; Singapore: EntrePass; UK: Innovator Founder)
- 3: Possible through other visa routes
- 2: Limited options (Germany: self-employment visa)
- 1: No startup visa (US)

**No Cap/Quota:**
- 5: No numerical cap (UK Global Talent; Germany Chancenkarte)
- 4: Flexible cap or high ceiling (Canada GTS; Singapore)
- 3: Moderate cap
- 2: Low cap with some flexibility
- 1: Hard cap with lottery (US: 85,000 with lottery)

**Merit-Based Selection:**
- 5: Pure merit/endorsement, no randomness (UK: endorsement bodies)
- 4: Merit-based with employer sponsorship (Canada, Germany, Singapore)
- 3: Mixed system
- 2: Primarily employer-driven with limited merit consideration
- 1: Random lottery (US H-1B)

**Portability/Flexibility:**
- 5: Can work for multiple employers, start businesses, switch freely
- 4: Significant flexibility (UK Global Talent: no employer tie; Singapore ONE Pass: multi-employer)
- 3: Some portability (Canada: employer-specific but transfer possible)
- 2: Employer-tied with transfer possible (Germany)
- 1: Employer-tied, difficult to switch (US H-1B: employer-sponsored)

### Radar Chart Data

| Dimension | US | Canada | UK | Germany | Singapore |
|-----------|-----|--------|-----|---------|-----------|
| Processing Speed | 1 | 5 | 3 | 3 | 4 |
| Startup Pathway | 1 | 4 | 4 | 2 | 4 |
| No Cap/Quota | 1 | 4 | 5 | 5 | 4 |
| Merit-Based Selection | 1 | 4 | 5 | 4 | 4 |
| Portability/Flexibility | 1 | 3 | 4 | 2 | 4 |

**Classification: OUR EXTRAPOLATION. All underlying program characteristics are SOURCED (see findings.md Section 4). The numerical scores are our subjective assessment for visualization purposes.**

### Composite Score

| Country | Total Score (out of 25) | Average | Classification |
|---------|------------------------|---------|----------------|
| United States | 5 | 1.0 | OUR EXTRAPOLATION |
| Canada | 20 | 4.0 | OUR EXTRAPOLATION |
| United Kingdom | 21 | 4.2 | OUR EXTRAPOLATION |
| Germany | 16 | 3.2 | OUR EXTRAPOLATION |
| Singapore | 20 | 4.0 | OUR EXTRAPOLATION |

### Chart Design Notes
- Format: Overlaid radar/spider charts, one line per country
- 5 axes radiating from center, one per dimension
- US line should form the smallest polygon (consistently lowest scores)
- UK and Canada should form the largest polygons
- Use distinct colors: US (red), Canada (blue), UK (purple), Germany (gold), Singapore (teal)
- Include a legend explaining the 1-5 scoring methodology
- Footnote: "Scores are our assessment based on documented program characteristics. See findings.md Section 4 for source data."

---

## Summary: Headline Metrics for All Visualizations

| Metric | Value | Timeframe | Classification | Source |
|--------|-------|-----------|----------------|--------|
| GDP loss from restriction | $12.1 trillion | 2025-2035 | CITED PROJECTION | NFAP Oct 2025 |
| GDP gain from H-1B reform | $456 billion | 10 years | CITED PROJECTION | Hoover Institution |
| Workforce reduction | 15.7 million | By 2035 | CITED PROJECTION | NFAP Oct 2025 |
| Additional federal debt | $1.74 trillion | 2025-2035 | CITED PROJECTION | NFAP Oct 2025 |
| Immigrant fiscal surplus | $14.5 trillion | 1994-2023 | CITED PROJECTION | Cato Institute |
| Interest savings component | $3.9 trillion | 1994-2023 | CITED PROJECTION | Cato Institute |
| Counterfactual debt-to-GDP | 205%+ | 2023 | CITED PROJECTION | Cato Institute |
| 1920s invention decline (ESE fields) | -68% | Post-1924 | SOURCED | Moser & San |
| 1920s native scientist patent decline | -45% | Post-1924 | SOURCED | Moser & San |
| Duration of 1920s effects | ~40 years | 1924-1960s | SOURCED | Moser & San |
| Immigrant share of U.S. patents | 36% (direct + collab) | 1990-2016 | SOURCED | NBER |
| Immigrant share of U.S. inventors | 16% | 1990-2016 | SOURCED | NBER |
| Jobs offshored per H-1B denial (avg) | 0.3 | Per denial | SOURCED | Glennon/NBER |
| Jobs offshored per H-1B denial (globalized MNCs) | 0.9 | Per denial | SOURCED | Glennon/NBER |
| Consumer spending reduction | $60-$110 billion | 2025-2026 | CITED PROJECTION | Brookings |
| H-1B expansion tax revenue | $113 billion | 10 years | CITED PROJECTION | Hoover Institution |
| US H-1B processing time | 6-9 months | 2025 | SOURCED | USCIS |
| Canada GTS processing time | 2 weeks | 2025 | SOURCED | Canada.ca |
| Monthly job creation (low immigration) | -20K to +20K | 2026 projection | CITED PROJECTION | Brookings |
| Monthly job creation (high immigration) | 10K to 50K | 2026 projection | CITED PROJECTION | Brookings |

---

*All estimates and extrapolations are explicitly labeled. Directly sourced figures and cited projections are distinguished throughout. No original economic modeling was performed. For detailed source citations and methodology notes, see findings.md.*
