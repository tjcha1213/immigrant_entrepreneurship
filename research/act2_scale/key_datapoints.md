# Act 2 - Scale: Key Data Points for Data Visualization (REVISED)

**Purpose:** Visualization-ready data points with chart type recommendations for the Harvard Data Visualization Project.
**Last Updated:** March 4, 2026
**Revision Note:** Added visualization type recommendations for every data point. Added methodological caveats per instructor feedback. All analysis is descriptive only.

---

## A. The "Immigrant Premium" -- Population Share vs. Impact Share

**Recommended Visualization: WAFFLE CHART (100-square grid) or ICON ARRAY**

Each metric shown as a separate waffle chart (100 icons, with filled icons representing the immigrant share). Stacking them vertically creates a powerful visual escalation from ~14% to ~55%.

**Alternative: Horizontal bar chart** with a vertical reference line at 14-15% (population share) to show how each metric exceeds the baseline.

| Metric | Value | Population Baseline | Multiple | Source | Year |
|--------|------:|:-------------------:|---------:|--------|------|
| Share of U.S. population | 14-15% | -- | 1.0x | U.S. Census Bureau | 2023 |
| Share of U.S. labor force | 17.1% | 14-15% | 1.2x | American Immigration Council | 2019 |
| Share of all U.S. business owners | 21.7% | 14-15% | 1.5x | American Immigration Council | 2019 |
| Share of new entrepreneurs | ~25% | 14-15% | 1.8x | Kauffman Foundation | 2019 |
| Share of U.S. patents (direct)* | 23% | 14-15% | 1.6x | NBER Working Paper 30797 | 2023 |
| Share of U.S. innovation (direct + spillover)* | 36% | 14-15% | 2.5x | NBER Working Paper 30797 | 2023 |
| Share of Fortune 500 founders (incl. 2nd gen) | 46.2% | 14-15% | 3.2x | American Immigration Council | 2025 |
| Share of unicorn startup founders | 55% | 14-15% | 3.8x | NFAP | 2022 |

*Patent figures cited from NBER published analysis, not independently verified. See findings.md Section 4 caveats.

**CAVEAT FOR VISUALIZATION:** These metrics come from different sources, use different definitions of "immigrant," and cover different time periods. The visual escalation is real but should include a footnote noting that metrics are not directly comparable (e.g., Fortune 500 includes 2nd generation; patent data is first-generation only).

---

## B. Fortune 500: Immigrant-Founded Companies

### B1. Headline Split

**Recommended Visualization: DONUT CHART**

A donut chart showing the 500 companies split three ways: 109 immigrant-founded (21.8%), 122 children-of-immigrant-founded (24.4%), and 269 other (53.8%). The donut hole can display "231 / 500" or "46.2%".

| Segment | Count | Percentage |
|---------|------:|-----------:|
| Founded by first-generation immigrants | 109 | 21.8% |
| Founded by children of immigrants | 122 | 24.4% |
| Other Fortune 500 companies | 269 | 53.8% |
| **Total** | **500** | **100%** |

Source: American Immigration Council, 2025

### B2. Revenue and Employment

**Recommended Visualization: BIG ANIMATED COUNTER NUMBERS**

These are best presented as large, scrolling "odometer-style" counters that tick up to the final number as the user scrolls into view:

| Data Point | Value | Context Comparison | Source |
|-----------|-------|-------------------|--------|
| Combined annual revenue | **$8.6 trillion** | Would rank as 3rd-largest economy globally (behind U.S. at $28.8T and China at $18.5T) | AIC, FY 2024 |
| Combined worldwide employees | **15.4 million** | Larger than the population of Pennsylvania | AIC, 2025 |

### B3. Industry Sector Breakdown

**Recommended Visualization: HORIZONTAL BAR CHART**

Horizontal bars showing each sector with the immigrant-founded percentage filled in. A vertical reference line at 46.2% (overall average) helps readers see which sectors are above or below average.

| Sector | Immigrant-Founded % | Count (of Total) |
|--------|--------------------:|:----------------:|
| Professional & Other Services | 80.0% | 8 of 10 |
| Manufacturing | 65.6% | 40 of 61 |
| Information | 57.5% | 23 of 40 |
| Entertainment, Accommodations & Food Services | 55.0% | 11 of 20 |
| Retail | 52.8% | 19 of 36 |
| *Overall Fortune 500 average* | *46.2%* | *231 of 500* |

Source: American Immigration Council, 2025

**Note:** The AIC report provides detailed breakdowns for the above five sectors. Additional sectors (finance, healthcare, energy, transportation, etc.) are present in the full dataset but sector-level percentages were not separately reported in the publicly available summary.

---

## C. Unicorn Startups ($1B+ Valuation)

### C1. Headline Split

**Recommended Visualization: DONUT CHART or PIE CHART**

Similar to Fortune 500, a donut showing 319 immigrant-founded vs. 263 other, out of 582 total.

| Data Point | Value | Source | Year |
|-----------|-------|--------|------|
| U.S. unicorns with immigrant founder | 319 of 582 (55%) | NFAP | 2022 |
| U.S. unicorns with immigrant founder OR key leader | 451 of 582 (~78%) | NFAP | 2022 |
| Collective value of immigrant-founded unicorns | $1.2 trillion+ | NFAP | 2022 |
| Average jobs per immigrant-founded unicorn | 859 | NFAP | 2022 |

### C2. Growth Over Time

**Recommended Visualization: SMALL MULTIPLES (three scaled circle/square charts)**

Three proportional area charts for 2016, 2018, and 2022, each showing total unicorns as the outer shape and immigrant-founded as the filled portion. The dramatic size increase from 87 to 582 total unicorns creates a strong visual.

| Year | Total U.S. Unicorns | Immigrant-Founded | Percentage | Source |
|------|--------------------:|------------------:|-----------:|--------|
| 2016 | 87 | 44 | 51% | NFAP 2016 |
| 2018 | 91 | 50 | 55% | NFAP 2018 |
| 2022 | 582 | 319 | 55% | NFAP 2022 |

**Visualization note:** The story here is the 538% absolute increase while the proportion stayed stable at ~55%. The small multiples approach conveys both the proportion AND the scale change.

### C3. Country of Origin Breakdown

**Recommended Visualization: TREEMAP or HORIZONTAL BAR CHART (top 15 countries)**

A treemap where each rectangle is sized by number of companies founded. Color-code by region (South Asia, Middle East, Europe, East Asia, etc.).

| Country | Companies | Country | Companies |
|---------|----------:|---------|----------:|
| India | 66 | Ukraine | 10 |
| Israel | 54 | Iran | 8 |
| United Kingdom | 27 | Australia | 7 |
| Canada | 22 | Romania | 6 |
| China | 21 | Italy | 6 |
| France | 18 | Nigeria | 6 |
| Germany | 15 | Poland | 6 |
| Russia | 11 | South Korea | 5 |

Source: NFAP, 2022

**CAVEAT:** Country-of-origin data reflects the country from which founders immigrated. Some founders have dual citizenship or lived in multiple countries. This is per NFAP's methodology.

### C4. Top Valued Immigrant-Founded Unicorns

**Recommended Visualization: HORIZONTAL BAR CHART (sorted by valuation)**

| Company | Valuation (2022) | Founder Origin |
|---------|----------------:|---------------|
| SpaceX | $125B | South Africa |
| Stripe | $95B | Ireland |
| Instacart | $39B | India/Canada |
| Databricks | $38B | Iran/Sweden |
| Epic Games | $31.5B | U.S. (immigrant leadership) |
| Miro | $17.5B | Russia |
| Discord | $15B | Ukraine (co-founder) |

Source: NFAP, 2022. **Note:** These are 2022 private-market valuations, not current public market caps. Values have shifted significantly since publication.

---

## D. Entrepreneurship Rate Comparison (Kauffman Index)

### D1. Rate Comparison Over Time

**Recommended Visualization: PAIRED HORIZONTAL BAR CHART or DIVERGING BAR CHART**

Two bars per year (immigrant rate and native-born rate) stacked or paired. The widening gap over time tells the story. Alternatively, a slope chart connecting the two rates for each year.

| Year | Immigrant New Entrepreneur Rate | Native-Born Rate | Ratio |
|------|-------------------------------:|----------------:|------:|
| 2020 | 0.59% | 0.34% | 1.7x |
| 2021 | 0.58% | 0.32% | 1.8x |
| 2023 | 0.67% | 0.28% | 2.4x |

Source: Kauffman Indicators of Entrepreneurship

**Visualization note:** Consider also showing the ratio (1.7x to 2.4x) as a big animated number that grows, emphasizing the widening gap.

### D2. Immigrant Share of New Entrepreneurs Over Time

**Recommended Visualization: AREA CHART or LINE CHART (1996-2023)**

A single line or area chart showing the immigrant share rising from 13.3% in 1996 to ~25-29% in recent years.

| Year | Immigrant Share of New Entrepreneurs |
|------|-------------------------------------:|
| 1996 | 13.3% |
| 2014 | 28.5% |
| 2019 | 25.4% |
| 2020-2023 | ~22-29% (varies by year) |

Source: Kauffman Foundation

### D3. Key Headline Numbers

**Recommended Visualization: BIG ANIMATED COUNTER NUMBERS**

| Statistic | Value | Source |
|-----------|-------|--------|
| Immigrants are X more likely to found a firm | **80% more likely** | Azoulay et al. / MIT, 2022 |
| Immigrant-founded firms create X more jobs | **42% more jobs** (relative to population) | Azoulay et al. / MIT, 2022 |
| Immigrant business ownership rate vs. population share | **21.7% owners vs. 14-15% population** | AIC, 2019 |

**CAVEAT:** The Azoulay et al. 80% figure is based on firm formations from 2005-2010. The Kauffman rate data captures monthly business starts. These are different measures of the same underlying pattern.

---

## E. Patent and Innovation Data

**CRITICAL NOTE:** All patent findings are cited from NBER Working Paper 30797 (Bernstein et al.). We do NOT claim to have independently verified these figures. Inventor nationality is not directly recorded in USPTO filings; the researchers used age-of-SSN-assignment as a proxy.

### E1. Patent Share Breakdown

**Recommended Visualization: WAFFLE CHART (100-unit grid)**

A 100-unit waffle chart where 23 units are highlighted to show the immigrant share of patents. A second waffle chart showing 36 units (adding the 13% collaboration) creates a powerful "before/after" effect.

**Alternative: Stacked bar or segmented bar** showing the 23% direct + 13% collaboration = 36% total.

| Metric | Value | Source |
|--------|------:|--------|
| Immigrant share of all U.S. inventors | 16% | NBER WP 30797 |
| Immigrant share of total U.S. patents (direct) | 23% | NBER WP 30797 |
| Citation-weighted patent share | 24% | NBER WP 30797 |
| Market-value-weighted patent share | 25% | NBER WP 30797 |
| Patents co-authored with native-born inventors | 13% | NBER WP 30797 |
| **Total innovation contribution (direct + indirect)** | **36%** | NBER WP 30797 |

### E2. Historical Diversification of Inventor Base

**Recommended Visualization: TWO-FRAME WAFFLE CHART or ANIMATED TRANSITION**

Show a 100-unit grid for 1975 (91 units = Anglo-Saxon/European names) and animate it to 2015 (72 units). The 19-unit shift represents the growing diversification.

| Year | Anglo-Saxon/European Share of Patents | Other Share |
|------|--------------------------------------:|------------:|
| 1975 | 91% | 9% |
| 2015 | 72% | 28% |

Source: NBER Working Paper 30797

**CAVEAT:** This is based on ethnic name analysis, which is an imperfect proxy for national origin or immigration status. The NBER paper acknowledges this limitation.

---

## F. Notable Immigrant-Founded Companies (Visualization-Ready)

### F1. Companies People Use Daily

**Recommended Visualization: ICON ARRAY / LOGO GRID**

Display company logos in a grid layout, organized by founder's country of origin or by industry. Each logo card can include the founder name and origin country. This is the most "human" and relatable visualization in Act 2.

| Company | Founder | Origin Country | Year Founded | Category |
|---------|---------|---------------|:------------:|----------|
| Google (Alphabet) | Sergey Brin | Russia | 1998 | Search / AI |
| Tesla | Elon Musk | South Africa | 2003 | Electric Vehicles |
| SpaceX | Elon Musk | South Africa | 2002 | Aerospace |
| Zoom | Eric Yuan | China | 2011 | Video Communications |
| eBay | Pierre Omidyar | France (Iranian parents) | 1995 | E-Commerce |
| YouTube | Steve Chen | Taiwan | 2005 | Video Platform |
| WhatsApp | Jan Koum | Ukraine | 2009 | Messaging |
| Stripe | Patrick & John Collison | Ireland | 2010 | Fintech |
| NVIDIA | Jensen Huang | Taiwan | 1993 | Semiconductors / AI |
| DoorDash | Tony Xu | China | 2013 | Food Delivery |
| Instacart | Apoorva Mehta | India (via Canada) | 2012 | Grocery Delivery |
| Chobani | Hamdi Ulukaya | Turkey | 2005 | Consumer Goods |

### F2. Children of Immigrants

| Company | Founder | Parent's Origin | Year Founded | Category |
|---------|---------|----------------|:------------:|----------|
| Apple | Steve Jobs | Syria | 1976 | Technology |
| Amazon | Jeff Bezos | Cuba (stepfather) | 1994 | E-Commerce / Cloud |
| Broadcom | Henry Samueli | Poland | 1991 | Semiconductors |

---

## G. Market Capitalization of Top Immigrant-Connected Companies

**Recommended Visualization: TREEMAP**

A treemap where each rectangle is proportional to market capitalization. Color-code by type (immigrant founder vs. child of immigrant). The massive rectangles for Apple and NVIDIA dominate the visual, showing scale.

**Alternative: Bubble chart** with bubbles sized by market cap and positioned by founding year on the x-axis.

| Company | Approx. Market Cap (early 2026) | Founder Origin | Type |
|---------|-------------------------------:|---------------|------|
| NVIDIA | ~$5.0 trillion | Taiwan | Immigrant |
| Apple | ~$4.0 trillion | Syria (father) | Child of immigrant |
| Alphabet (Google) | ~$3.0 trillion | Russia | Immigrant (co-founder) |
| Amazon | ~$2.5 trillion | Cuba (stepfather) | Child of immigrant |
| Tesla | ~$1.6 trillion | South Africa | Immigrant |
| Broadcom | ~$1.0 trillion | Poland (parents) | Child of immigrant |
| **Combined Total** | **~$17.1 trillion** | | |

**Context for visualization:** The S&P 500 total market cap is ~$61 trillion. These 6 companies = ~28% of the entire index. Consider showing the $17.1T as a proportion of $61T using a **segmented bar** or **nested square**.

**CAVEAT:** Market capitalizations fluctuate daily. These are approximate figures from late 2025 / early 2026. The $17.1T combined figure should be presented with a "as of approximately [date]" label in any visualization.

---

## H. Top-Line "Billboard" Statistics for Large-Format Visualization

**Recommended Visualization: BIG ANIMATED COUNTER NUMBERS (scrollytelling sequence)**

These are the "hero" numbers that should appear as large, animated counters in the scrollytelling narrative. Each should fill the viewport and count up to the final value as the user scrolls.

| # | Statistic | Display Text | Viz Type | Source |
|---|-----------|-------------|----------|--------|
| 1 | **46.2%** of Fortune 500 have immigrant roots | "Nearly half of America's largest companies" | Big counter | AIC 2025 |
| 2 | **$8.6 trillion** in annual revenue | "Larger than the GDP of Japan, Germany, India, or the UK" | Big counter with GDP comparison | AIC 2025 |
| 3 | **55%** of unicorns have immigrant founder | "More than half of billion-dollar startups" | Big counter | NFAP 2022 |
| 4 | **15.4 million** employees worldwide | "More people than the population of Pennsylvania" | Big counter | AIC 2025 |
| 5 | **36%** of all U.S. patent innovation involves immigrants* | "Over a third of American invention" | Waffle chart | NBER WP 30797 |
| 6 | **2.4x** entrepreneurship rate multiple | "Immigrants start businesses at 2.4x the native-born rate" | Big counter | Kauffman 2023 |
| 7 | **~$17.1 trillion** combined market cap, top 6 companies | "~28% of the entire S&P 500" | Treemap | Multiple sources |
| 8 | **319** billion-dollar startups with immigrant founders | "From 65 different countries" | Big counter | NFAP 2022 |

*Cited from NBER Working Paper 30797; not independently verified.

---

## I. Visualization Sequence Recommendation for Act 2

The recommended narrative flow for scrollytelling:

1. **Open with big counter:** "46.2% of Fortune 500 companies..." (hooks the reader)
2. **Donut chart:** Fortune 500 breakdown (109 + 122 + 269)
3. **Big counters:** $8.6T revenue, 15.4M employees
4. **Horizontal bar chart:** Industry sector breakdown
5. **Transition to unicorns:** "55% of billion-dollar startups..." (big counter)
6. **Small multiples:** 2016 vs. 2018 vs. 2022 unicorn growth
7. **Treemap:** Country of origin for unicorn founders
8. **Paired bar chart:** Kauffman entrepreneurship rates (immigrant vs. native-born)
9. **Waffle charts:** Patent data (16% of inventors produce 23% of patents, 36% total contribution)
10. **Icon array / logo grid:** Companies people use daily
11. **Treemap:** Market capitalization of top immigrant-connected companies ($17.1T)
12. **Close with waffle chart escalation:** The "Immigrant Premium" table from Section A, shown as ascending waffle charts

---

## J. Methodological Notes for Visualization Labels

Every visualization in Act 2 should include a small-text footnote or tooltip with:

1. **Source attribution** (e.g., "Source: American Immigration Council, 2025")
2. **Definition used** (e.g., "Includes both first-generation immigrants and children of immigrants")
3. **Time period** (e.g., "Based on FY 2024 revenue data")
4. **Key caveat** where applicable:
   - For patent data: "Findings cited from NBER Working Paper 30797. Inventor nationality is not directly recorded in USPTO filings."
   - For unicorn valuations: "Private-market valuations as of May 2022. Values have shifted since publication."
   - For market cap: "Approximate values as of early 2026. Market capitalizations fluctuate daily."
   - For Fortune 500: "Revenue represents total company revenue, not revenue attributable to founder's immigrant status."
   - For Kauffman data: "New entrepreneur rate measures monthly business formation. Includes both opportunity and necessity entrepreneurship."
   - For the cross-cutting "Immigrant Premium" chart: "Metrics come from different sources with different definitions and time periods. Not directly comparable."

---

## Source Reference Key

| Abbreviation | Full Source | URL |
|-------------|------------|-----|
| AIC 2025 | American Immigration Council, Fortune 500 Report 2025 | https://www.americanimmigrationcouncil.org/report/fortune-500-companies-founded-by-immigrants-2025/ |
| NFAP 2022 | National Foundation for American Policy, Billion-Dollar Companies Brief | https://nfap.com/wp-content/uploads/2022/07/Immigrant-Entrepreneurs-and-Billion-Dollar-Companies.DAY-OF-RELEASE.2022.pdf |
| NFAP 2016 | National Foundation for American Policy, Billion-Dollar Startups Brief | https://nfap.com/wp-content/uploads/2016/03/Immigrants-and-Billion-Dollar-Startups.NFAP-Policy-Brief.March-2016.pdf |
| NBER WP 30797 | Bernstein et al., High-Skilled Immigrants and Innovation | https://www.nber.org/papers/w30797 |
| Kauffman | Kauffman Indicators of Entrepreneurship | https://indicators.kauffman.org |
| MIT/AER | Azoulay et al., Immigration and Entrepreneurship in the United States | https://news.mit.edu/2022/study-immigrants-more-likely-start-firms-create-jobs-0509 |
| Fairlie 2023 | Indicators of Entrepreneurial Activity: 2023 | https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4708111 |
| ITIF | Information Technology and Innovation Foundation | https://itif.org/publications/2023/07/17/immigrant-inventors-produce-23-percent-of-us-patents/ |

---

*Prepared for the Harvard Data Visualization Project -- Act 2: Scale. All analysis is descriptive and exploratory. No causal claims are made.*
