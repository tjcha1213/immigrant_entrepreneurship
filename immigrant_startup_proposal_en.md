# Built by Immigrants, Threatened by Policy
### Visualizing the Impact of Immigrant Entrepreneurs on the U.S. Innovation Economy
**Data Visualization Group Project Proposal — Harvard University, Spring 2025**

---

## 01 / Research Question

How have immigrant-founded startups shaped the U.S. innovation economy, and how has this relationship evolved alongside shifts in immigration policy?

> **Scope note:** This project focuses on **descriptive and exploratory analysis** — mapping the scale, composition, and geographic distribution of immigrant entrepreneurship and overlaying policy shifts as contextual factors. We do not attempt causal inference or predictive economic modelling; projections from existing studies (NFAP, Brookings) are cited as reference points, not original analysis.

---

## 02 / Intended Audience

**Primary audience: Educated general public** — people who engage with data journalism (e.g., NYT Upshot, Visual Capitalist readers). The narrative should be understood by non-experts within 2 minutes.

**Secondary audiences** are served through supplementary formats:

| Audience | How We Serve Them |
|----------|------------------|
| 🎓 Students & Entrepreneurs | The scrollytelling narrative itself — discover pathways taken by immigrant founders |
| 🏛️ Policymakers | PDF executive summary with high-resolution charts (2–4 pages, designed for briefings) |
| 💼 VCs & Investors | Filterable Tableau dashboard for exploratory analysis by origin, industry, and geography |

> **Design implication:** The primary scrollytelling narrative is optimized for **accessibility and narrative clarity** at a general-public level of granularity. Detailed, filterable data is available in the secondary Tableau dashboard for expert users.

---

## 03 / Story Arc — 5-Act Narrative Structure

### Act 1 — Hook
*"How many services did you use today that were founded by immigrants?"*
Google. YouTube. Zoom. Tesla. eBay. We open with familiar products to immediately capture attention. Facts land harder than feelings.

### Act 2 — Scale
Nearly 45% of Fortune 500 companies and roughly half of U.S. unicorn startups were founded by immigrants or their children.
We use macro-level data to establish an undeniable truth: immigrants are at the center of American innovation.

### Act 3 — Who / Where / What
We map the ecosystem across two reliable dimensions: **country of origin × industry** and **country of origin × U.S. geography**.
- Indian-born founders → AI & IT
- Chinese-born founders → Hardware
- Israeli-born founders → Cybersecurity

Choropleth maps and bubble charts make these patterns instantly visible.

> **Data limitation — Visa pathways:** Individual founders' visa histories (F-1, H-1B, O-1, EB-1, etc.) are **not systematically available** in any public dataset. USCIS does not publish individual-level visa records, and founders' immigration histories are scattered across interviews, press coverage, and self-reported profiles. The CSET Georgetown study (AI startup founders, n≈100) and NFAP reports provide aggregate estimates (e.g., "72% of AI founders initially arrived on F-1 visas"), but these are based on **small, hand-curated samples** with survivorship bias. We cite these aggregate figures with appropriate caveats rather than presenting visa-pathway data as comprehensive or individually verified.

### Act 4 — The Policy Context
We present H-1B and EB visa approval trends alongside key policy shifts across administrations (Obama, Trump, Biden, Trump 2nd term) as a **descriptive overlay** — showing how policy changes coincide with shifts in denial rates, processing backlogs, and talent-flow indicators.

> **Methodological note:** We present temporal co-occurrence, not causal claims. External factors — macroeconomic cycles, VC market conditions, COVID-19 — also affect startup founding rates. Where we cite existing studies that attempt causal analysis (e.g., NBER working papers on H-1B lotteries), we clearly attribute and note their methodologies.

### Act 5 — What's at Stake
We contextualize the findings by surfacing published estimates of economic impact from credible institutions (NFAP, Brookings, Hoover, Cato). We present these as **existing projections from cited sources**, not original modelling, and close with a synthesis of policy recommendations from leading research organizations.

---

## 04 / Data Sources

### Primary Sources

| Dataset | Provider | Key Variables | Relevant Acts | Feasibility Notes |
|---------|----------|---------------|---------------|-------------------|
| Fortune 500 Immigrant Founders Report | [American Immigration Council](https://www.americanimmigrationcouncil.org/report/fortune-500-companies-founded-by-immigrants-2025/) | Founder origin, company, revenue, employees | Act 2, 3 | Full report freely available; 231 companies identified |
| Immigrant Founders of Billion-Dollar Companies | [NFAP](https://nfap.com/research/new-nfap-policy-brief-immigrant-entrepreneurs-and-u-s-billion-dollar-companies/) | Founder origin, sector, valuation, visa pathway | Act 2, 3 | 319 companies; structured data available in policy brief |
| USCIS H-1B & EB Visa Statistics | USCIS | Visa approvals, denial rates, nationality, employer | Act 4 | Official public data; annual reports downloadable |
| Kauffman Indicators of Entrepreneurship | Kauffman Foundation | Startup rate, immigrant share, native-born comparison | Act 2 | Public dashboard with downloadable data |
| U.S. Census Bureau ACS PUMS | Census | Immigrant population by state, education, income | Act 3 | Publicly available microdata |

### Secondary / Referenced Sources

| Dataset | Provider | Use | Notes |
|---------|----------|-----|-------|
| Immigrant-Founded Billion-Dollar Companies (Visual) | [Visual Capitalist](https://www.visualcapitalist.com/immigrant-founders-us-billion-dollar-companies/) | Act 2, 3 | Pre-visualized data; useful for cross-validation |
| Immigrants' Fiscal Effects (1994–2023) | [Cato Institute](https://www.cato.org/white-paper/immigrants-recent-effects-government-budgets-1994-2023) | Act 5 | $14.5T fiscal surplus estimate; cited as-is |
| Immigration and Entrepreneurship in the U.S. | [NBER Working Paper 32400](https://www.nber.org/papers/w32400) | Act 2, 4 | Peer-reviewed causal analysis; cited with methodology attribution |
| High-Skilled Immigration and Innovation | [NBER Working Paper 30797](https://www.nber.org/papers/w30797) | Act 2, 5 | Patent data; immigrant share of U.S. innovation (36%) |
| Economic Impact of Immigration Policies | [NFAP, Oct 2025](https://nfap.com/wp-content/uploads/2025/10/Economic-Impact-of-The-Trump-Administration-Immigration-Policies.NFAP-Policy-Brief.2025-1.pdf) | Act 5 | GDP/workforce projections; cited as external estimates |

### Sources Considered but Deprioritized

| Dataset | Provider | Reason |
|---------|----------|--------|
| Crunchbase Open Data Map | Crunchbase | Available via HBS library, but **download limit of 1,000 records per export** makes comprehensive analysis impractical. We use NFAP's curated dataset (319 companies) and AIC's Fortune 500 dataset (231 companies) instead, supplemented with individual Crunchbase lookups for enrichment. |
| USPTO PatentsView | USPTO | Inventor nationality is **not directly recorded** in patent filings. Estimation requires name-based ethnicity inference (e.g., NBER's linked datasets) or matching with visa records, which introduces methodological uncertainty. We cite NBER's published patent analysis (Working Paper 30797) rather than conducting original patent-nationality linkage. |

---

## 05 / Analysis & Visualization Plan

| Chart Type | Description | Tool | Act |
|------------|-------------|------|-----|
| Big Number + Donut Chart | Share of unicorns and Fortune 500 companies founded by immigrants | Datawrapper | 2 |
| Horizontal Bar Chart | "Immigrant Premium" — population share vs. contribution share across metrics | Datawrapper | 2 |
| Market Cap Treemap | Top immigrant-connected companies by market capitalization | Flourish | 2 |
| Choropleth Map (World) | Number of billion-dollar companies by founder's country of origin | Tableau | 3 |
| Heatmap Matrix | Country of origin × industry sector concentration | Flourish | 3 |
| Bubble Chart | Companies by origin country × industry × valuation | Flourish | 3 |
| Choropleth Map (U.S.) | Density of immigrant-founded companies by state/metro | Tableau | 3 |
| Donut Chart | Visa pathway distribution of immigrant founders (aggregate estimates from CSET/NFAP; labeled as illustrative, not comprehensive) | Datawrapper | 3 |
| Line Chart + Era Bands | H-1B denial rates over time with policy-era color bands | Flourish | 4 |
| Policy Timeline | Key immigration policy events (2010–2026) coded by direction and impact | Flourish | 4 |
| Grouped Bar Chart | Green card backlog wait times by country and category | Datawrapper | 4 |
| KPI Cards | Brain drain indicators (employer loss %, scientist departure intent, etc.) | Custom HTML | 4 |
| Scenario Bar Chart | Published GDP/workforce projections under three policy scenarios (cited, not modelled) | Datawrapper | 5 |
| Before/After Comparison | 1920s immigration restriction — historical precedent (Stanford GSB data) | Flourish | 5 |
| Comparison Table | Global talent competition scorecard (U.S. vs. Canada, UK, Germany, Singapore) | Custom HTML | 5 |
| Radar / Star Chart | Team skills visualization across 4 dimensions | Flourish | — |

---

## 06 / Success Criteria

| Criterion | Definition |
|-----------|------------|
| **Educate the Public** | Key findings should be understood by non-experts within 2 minutes (validated through user testing) |
| **Inform Decision Makers** | Deliver at least 3 policy-relevant data points in the executive summary, formatted for briefings |
| **Exploratory Depth** | Tableau dashboard enables filtering by origin country, industry, and geography for expert users |
| **Visual Accessibility** | All charts pass colorblind accessibility checks (WCAG AA); responsive layout for desktop and mobile |
| **Methodological Integrity** | All causal claims are attributed to cited studies with methodology notes; original analysis is descriptive only |

---

## 07 / Team Members

> *(To be updated once team roles are confirmed)*

Team skills will be visualized using a **Flourish Star Chart** across four dimensions:
- Data Wrangling
- Visual Design
- Storytelling
- Domain Expertise

---

## 08 / Final Media Format

| Format | Description |
|--------|-------------|
| 🌐 Interactive Web Story | Scrollytelling page — data unfolds across the 5-act narrative for a general audience. **Primary deliverable.** |
| 📊 Tableau Dashboard | Filterable public dashboard for exploratory analysis by origin, industry, and region |
| 📄 PDF Executive Summary | 2–4 page static report with high-resolution charts, designed for policymakers |
| ⭐ Flourish Radar Chart | Star chart showing each team member's skill profile across 4 dimensions |

---

## 09 / Revision Log

| Date | Reviewer | Changes |
|------|----------|---------|
| Mar 1, 2025 | Tsukasa Nakamura | Narrowed research question to descriptive analysis (removed economic modelling scope). Prioritized general public as primary audience. Added feasibility notes for Crunchbase (download limit) and USPTO (nationality estimation). Reframed Act 4 as descriptive overlay with confounding-variable caveat. Reframed Act 5 as citing existing projections rather than original modelling. Added 4 recommended data sources. Added methodological integrity criterion. |
| Mar 4, 2025 | (internal) | Added data limitation note on visa pathway data: individual visa histories are not systematically available in public datasets; aggregate figures from CSET/NFAP are small-sample estimates with survivorship bias. Visa pathway donut chart labeled as illustrative. |

---

*Data Visualization Group Project Proposal · Harvard University · Spring 2025 · Tools: Tableau · Flourish · Datawrapper · Python (Pandas)*
