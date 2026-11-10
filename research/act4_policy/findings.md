# Act 4 -- The Policy Context: Immigration Policy and the U.S. Innovation Economy

## Research Summary for Harvard Data Visualization Project (REVISED)

*Last updated: March 2026*
*Revision note: Restructured per instructor feedback. This act is DESCRIPTIVE AND EXPLORATORY. We present temporal co-occurrence between policy changes and startup ecosystem metrics, not causal claims. External factors (macroeconomic cycles, VC market conditions, COVID-19, global competition) also affect startup founding rates. Where we cite studies with causal analysis (e.g., NBER H-1B lottery papers), we attribute their methodologies explicitly.*

---

## Table of Contents

1. [Methodological Note](#1-methodological-note)
2. [H-1B Denial Rates by Fiscal Year and Policy Era](#2-h-1b-denial-rates-by-fiscal-year-and-policy-era)
3. [Request for Evidence (RFE) Rates](#3-request-for-evidence-rfe-rates)
4. [H-1B Nationality Breakdown](#4-h-1b-nationality-breakdown)
5. [Green Card Backlog: The Structural Bottleneck](#5-green-card-backlog-the-structural-bottleneck)
6. [Brain Drain Indicators](#6-brain-drain-indicators)
7. [Policy Events Timeline (2010-2026)](#7-policy-events-timeline-2010-2026)
8. [Current Policy Landscape: Trump Second Term](#8-current-policy-landscape-trump-second-term)
9. [Visualization Design Notes](#9-visualization-design-notes)
10. [Sources](#10-sources)

---

## 1. Methodological Note

This research presents descriptive data on immigration policy changes alongside innovation economy metrics. The relationship between H-1B policy and startup founding rates is complex and multidirectional:

- **What we can show:** Temporal co-occurrence of policy changes with shifts in denial rates, processing times, and talent flow indicators.
- **What we cannot claim:** That any single policy change caused a specific change in startup founding rates.
- **Confounding factors we acknowledge:** Macroeconomic cycles, venture capital market conditions, COVID-19 pandemic effects, technological shifts, global competition for talent, and individual firm-level decisions.
- **Causal studies we reference:** Where NBER or other researchers use quasi-experimental designs (e.g., H-1B lottery randomization), we note their methodology. The causal claims belong to those authors, not to our visualization project.

The H-1B correlation with startup founding rates is "presented and interpreted carefully" (per instructor feedback). We use language like "co-occurred with," "during this period," and "alongside" rather than "caused" or "led to."

---

## 2. H-1B Denial Rates by Fiscal Year and Policy Era

### 2.1 Year-by-Year Denial Rates for Initial Employment (FY 2010-2025)

The H-1B denial rate for petitions for initial (new) employment shows stark variation across presidential administrations. These rates reflect adjudication policy at USCIS, which is set by executive branch direction.

| Fiscal Year | Denial Rate | Policy Era | Key Context |
|-------------|-------------|------------|-------------|
| FY 2010 | 8% | Obama | Post-recession recovery; stable adjudication |
| FY 2011 | 7% | Obama | Consistent baseline |
| FY 2012 | 5% | Obama | Lowest of the Obama era |
| FY 2013 | 7% | Obama | Stable |
| FY 2014 | 8% | Obama | Modest uptick |
| FY 2015 | 6% | Obama | Stable baseline |
| FY 2016 | 10% | Obama | Uptick in final Obama year |
| FY 2017 | 13% | Trump 1 | BAHA EO signed April 2017; RFEs surge |
| FY 2018 | **24%** | Trump 1 | Peak denial rate; BAHA fully implemented |
| FY 2019 | **21%** | Trump 1 | Continued restrictive adjudication; RFE rate peaks |
| FY 2020 | 13% | Trump 1 | Partial rollback after ITServe Alliance litigation |
| FY 2021 | 4% | Biden | ITServe settlement effects; Biden transition; PA-2021-05 |
| FY 2022 | 2% | Biden | Historic low; Buy American Hire American rescinded |
| FY 2023 | 3.5% | Biden | Slight uptick, still near historic lows |
| FY 2024 | 2.5% | Biden | Stable near historic lows |
| FY 2025 | 2.8% | Trump 2 | NFAP Nov 2025 report; $100K fee takes effect Sept 2025 |

**Key observation (descriptive, not causal):** The denial rate for initial H-1B employment rose from 6% in FY 2015 to 24% in FY 2018 -- a 4x increase that co-occurred with the Buy American Hire American executive order and associated USCIS policy memos. The rate then declined to 2% by FY 2022, co-occurring with the ITServe Alliance v. Cissna settlement (2020), USCIS Policy Alert PA-2021-05, and the Biden administration's rescission of BAHA. Multiple factors contributed to these shifts, including litigation outcomes and changes in the composition of petitioning employers.

**Data sources:**
- [NFAP H-1B Denial Rate Table 2011-2024](https://nfap.com/newarticle/nfap-table-on-h-1b-denial-rate-2011-to-2024/)
- [NFAP FY 2025 Policy Brief (Nov 2025)](https://nfap.com/wp-content/uploads/2025/11/H-1B-Petitions-and-Denial-Rates-For-FY-2025.NFAP-Policy-Brief.2025.pdf)
- [NFAP FY 2024 Policy Brief](https://nfap.com/wp-content/uploads/2024/12/H-1B-Petitions-and-Denial-Rates-For-FY-2024.NFAP-Policy-Brief.December-2024.pdf)

### 2.2 H-1B Lottery Registration Trends

The H-1B electronic registration system (introduced FY 2021) provides data on demand:

| Season | Eligible Registrations | Selected | Selection Rate | Notes |
|--------|----------------------|----------|---------------|-------|
| FY 2022 | 308,613 | 131,924 | ~42.7% | Including subsequent rounds |
| FY 2023 | 474,421 | ~127,600 | ~26.9% | Demand growing |
| FY 2024 | 758,994 | ~110,791 | ~14.6% | Record registrations; fraud concerns |
| FY 2025 | ~470,000 | ~121,000 | ~25.6% | Post-integrity rule drop (~38% fewer registrations) |
| FY 2026 | 336,153 (unique) | 118,660 | ~35.3% | Beneficiary-centric selection; $100K fee announced |

**Data source:** [USCIS H-1B Electronic Registration Process](https://www.uscis.gov/working-in-the-united-states/temporary-workers/h-1b-specialty-occupations/h-1b-electronic-registration-process)

---

## 3. Request for Evidence (RFE) Rates

RFEs serve as a leading indicator of adjudication strictness. USCIS issues an RFE when it determines a petition lacks sufficient evidence, requiring the employer to submit additional documentation.

| Fiscal Year | RFE Rate | Policy Era | Notes |
|-------------|----------|------------|-------|
| FY 2015 | ~22% (est.) | Obama | Baseline estimate |
| FY 2016 | ~22% (est.) | Obama | Pre-BAHA baseline |
| FY 2017 | 21.4% | Trump 1 | BAHA signed mid-year; 85,000 RFEs Jan-Aug (+45% YoY) |
| FY 2018 | **38.0%** | Trump 1 | Near-doubling; BAHA fully in effect |
| FY 2019 | **40.2%** | Trump 1 | Peak RFE rate; 2 in 5 petitions challenged |
| FY 2020 | 28.8% | Trump 1 | Decline after ITServe litigation |
| FY 2021 | 16.2% | Biden | Sharp decline; PA-2021-05 issued |
| FY 2022 | 9.6% | Biden | Historic low |
| FY 2023 | 10.5% | Biden | Slight uptick; 39,222 petitions with RFE out of 397,231 |

**Approval rate after RFE:** In FY 2023, 79.8% of petitions that received an RFE were ultimately approved, down from 85.5% in FY 2022. During the peak restrictive period (FY 2018), the post-RFE approval rate dropped to approximately 60%.

**Data sources:**
- [USCIS FY 2023 H-1B Characteristics Report (PDF)](https://www.uscis.gov/sites/default/files/document/reports/OLA_Signed_H1B_Characteristics_Congressional_Report_FY2023.pdf)
- [Immigration Policy Tracking Project](https://immpolicytracking.org/policies/report-that-uscis-has-increased-rates-of-rfes-and-denials-of-h-1b-and-l-1-petitions/)

---

## 4. H-1B Nationality Breakdown

### 4.1 Country of Birth Distribution Over Time

India has dominated H-1B approvals throughout the study period, with its share increasing substantially:

| Period | India % | China % | Other % | Source |
|--------|---------|---------|---------|--------|
| FY 2001-2015 average | ~50.5% | ~9.7% | ~39.8% | Pew Research |
| FY 2019 | ~72% | ~13% | ~15% | USCIS FY2019 Report |
| FY 2020-2023 average | ~73.7% | ~16% | ~10.3% | Pew Research |
| FY 2023 | 73% | 12% | 15% | Pew Research |
| FY 2024 | 71% | 11.7% | 17.3% | USCIS FY2024 Report |

**Key observation:** India's share of H-1B approvals grew from approximately half in the 2001-2015 period to roughly three-quarters in recent years. India and China together account for more than 82% of all H-1B approvals. This concentration has implications for the green card backlog (Section 5) given per-country caps.

### 4.2 Specific FY 2024 Figures

- India: 283,397 approvals (71.0%)
- China: 46,680 approvals (11.7%)
- All other countries: 69,318 approvals (17.3%)
- Total: 399,395

**Data sources:**
- [Pew Research Center -- H-1B Visa Program Data (March 2025)](https://www.pewresearch.org/short-reads/2025/03/04/what-we-know-about-the-us-h-1b-visa-program/)
- [Visual Capitalist -- H-1B Visa Approvals by Country 2024](https://www.visualcapitalist.com/visualized-h-1b-visa-approvals-by-country-in-2024/)
- [USCIS FY 2024 H-1B Characteristics Report (PDF)](https://www.uscis.gov/sites/default/files/document/reports/ola_signed_h1b_characteristics_congressional_report_FY24.pdf)

---

## 5. Green Card Backlog: The Structural Bottleneck

### 5.1 The Scale of the Problem

The employment-based green card system is constrained by two structural factors:
1. An annual cap of ~140,000 employment-based immigrant visas (set by Congress in 1990)
2. A 7% per-country limit that applies regardless of demand

As of 2024, the Cato Institute documented **1.8 million people** in the employment-based green card backlog, of which:
- **1.1 million (63%)** are from India
- **~250,000 (14%)** are from China
- Remaining ~23% from all other countries

### 5.2 Wait Times by Category and Country (as of December 2025 / March 2026)

| Category | India Wait (Years) | China Wait (Years) | ROW Wait (Years) | India Priority Date | China Priority Date |
|----------|-------------------|-------------------|-------------------|--------------------|--------------------|
| EB-1 (Priority Workers) | ~3-4 | ~3-4 | 0 (current) | March 1, 2022 | Nov 1, 2022 |
| EB-2 (Advanced Degree) | **12-18** | 5-6 | 0-1 | Sept 15, 2013 | ~Dec 2021 (frozen) |
| EB-3 (Skilled Workers) | **11-12** | ~4 | 0-1 | ~Aug 2014 (frozen) | ~Jan 2022 (frozen) |
| EB-5 (Investors) | ~0 | ~0 | 0 | Current (post-RIA) | Current (post-RIA) |

**Critical data points:**
- EB-2 India applicants filing today face an estimated **134-year theoretical wait** (Boundless, 2024), though this is a projection based on current movement rates and assumes no legislative change.
- EB-1 India retrogressed by more than 10 years in August 2023 -- an unprecedented event signaling spillover from lower categories.
- EB-1 India moves approximately 10-15 months per year; China moves 15-20 months per year.
- Rest of World generally remains "current" (no backlog) for all categories.

### 5.3 Total Backlog in Context

- **1.8 million** in employment-based green card backlog (Cato, 2024)
- **11.3 million** total pending cases at USCIS as of Q2 FY2025 (record high)
- **483 days** average PERM labor certification processing time (DOL, mid-2025)
- The 140,000 annual EB visa cap has not been updated since the Immigration Act of 1990

**Data sources:**
- [Cato Institute -- 1.8 Million in Employment-Based Green Card Backlog](https://www.cato.org/blog/18-million-employment-based-green-card-backlog)
- [Boundless -- 134-Year Wait for Indian Nationals](https://www.boundless.com/blog/indians-face-134-year-wait-employment-based-green-card)
- [Fragomen -- Green Card Backlogs 2025](https://www.fragomen.com/insights/green-card-backlogs-and-visa-bulletin-trends-what-employers-can-do-in-2025-and-beyond.html)
- [Boundless -- March 2026 Visa Bulletin](https://www.boundless.com/blog/visa-bulletin)

---

## 6. Brain Drain Indicators

*Note: "Brain drain" indicators reflect survey data, renunciation records, and program statistics. They describe talent movement patterns but cannot isolate immigration policy as the sole driver. Economic opportunity, family considerations, and home-country conditions are also significant factors.*

### 6.1 Employer Experience

- **82%** of employers surveyed by Envoy Global (2023) reported having to let go of or reassign foreign employees in the past year due to visa difficulties.

**Source:** [Reason -- America's Immigrant Brain Drain (Sept 2023)](https://reason.com/2023/09/26/americas-immigrant-brain-drain/)

### 6.2 Scientist Departure Intent

- A 2025 Nature poll of **1,600 scientists** found that **75%** said they were considering leaving the United States, with Europe and Canada as top destinations.
- Among Chinese-born PhDs in the U.S., intent to stay dropped from **81% in 2016** to **77.5% in 2023** (reflects both immigration frustrations and China's growing career opportunities).
- Among Indian-born PhDs, **89%** expressed interest in remaining in the U.S. despite long green card waitlists.
- European Research Council early-career grant applications from the U.S. nearly tripled: 60 (2024 call) to 116 (2025 call) to 169 (2026 call).
- U.S. job-seekers applying abroad rose sharply in early 2025: **+41%** to Canada, **+32%** to Europe, **+20%** to China, **+39%** to other Asian countries (Nature jobs board data, compared to same period 2024).
- International scholars in the U.S. were down **18% vs. 2018 levels** as of 2024.

**Sources:**
- [STAT News -- Brain Drain (Dec 2025)](https://www.statnews.com/2025/12/17/research-cuts-fuel-scientific-brain-drain-american-science-shattered/)
- [ITIF -- US Brain Drain Threatens Leadership (Dec 2025)](https://itif.org/publications/2025/12/18/us-brain-drain-threatens-scientific-and-biopharmaceutical-leadership/)
- [Boston College IHE -- America's Brain Drain](https://ihe.bc.edu/pub/d6snhiz8)

### 6.3 Canada Start-Up Visa (SUV) Program Growth

Canada's SUV program provides a direct comparison point for talent competition:

| Year | New PRs Granted | Applications in System | Notes |
|------|----------------|----------------------|-------|
| 2020 | Low (pandemic) | ~2,000 | COVID disruption |
| 2021 | Recovery | Growing | Post-pandemic rebound begins |
| 2022 | ~601 processed | ~5,000 | Processing volume ramping |
| 2023 | Growing | ~10,000 | Program gaining traction |
| 2024 | **5,595** (record) | **18,514** | Peak year; 7x processing growth from 2022 |
| 2025 | Cap reduced to 2,000 | ~18,000 backlog | Refusal rate surges to 73% (incubator stream) |
| 2026-2027 | Cap further reduced to 1,000/year | Backlog clearing | Canada tightening intake |

**Key observation:** The Canada SUV saw explosive growth through 2024, with a nearly 7-fold increase in processing volume from 2022 to 2024. However, Canada itself has begun restricting intake, reducing the cap from ~6,000 to 1,000 per year by 2026-2027 -- suggesting that the "escape valve" narrative may be overstated going forward.

**Sources:**
- [Global Citizen Solutions -- Canada Startup Visa Statistics](https://www.globalcitizensolutions.com/canada-startup-visa-record-high/)
- [Canada.ca -- Start-up Visa Program Evaluation](https://www.canada.ca/en/immigration-refugees-citizenship/corporate/reports-statistics/evaluations/evaluation-start-up-visa-program.html)

### 6.4 Indian Citizenship Renunciation

| Year | Renunciations | Notes |
|------|--------------|-------|
| 2015 | 131,489 | Baseline |
| 2016 | 141,603 | |
| 2017 | 133,049 | |
| 2018 | 134,561 | |
| 2019 | 144,017 | Pre-pandemic peak |
| 2020 | 85,256 | COVID-related drop |
| 2021 | 163,370 | Post-pandemic surge |
| 2022 | **225,620** | Record high |
| 2023 | 216,219 | Near-record |
| 2024 | 206,378 | Sustained high levels |
| **Total 2019-2024** | **~1,040,240** | Over 1 million in 6 years |

**Context:** Renunciation of Indian citizenship is required when obtaining citizenship of another country (India does not permit dual citizenship). These numbers reflect Indians obtaining citizenship elsewhere -- primarily in the U.S., UK, Australia, and Canada. The sharp increase from 2020 onward co-occurs with expanded global talent competition but also reflects post-pandemic normalization. Not all renunciations are tech/startup-related.

**Source:** [Statista -- Indians Renouncing Citizenship 2011-2024](https://www.statista.com/statistics/1378071/india-number-of-people-renouncing-citizenship/); [VisaVerge -- 2024 Renunciation Data](https://www.visaverge.com/news/over-2-lakh-indians-renounced-citizenship-in-2024-govt-data-shows/)

### 6.5 Chinese Scientists Returning from the U.S.

- At least **85 prominent Chinese scientists** left U.S. institutions and joined Chinese research institutions since the beginning of 2025, concentrated in AI, semiconductors, and other strategic fields.
- This follows the broader "China Initiative" era (2018-2022) and heightened scrutiny of academic collaborations with China.

---

## 7. Policy Events Timeline (2010-2026)

### 7.1 Obama Administration (2009-2017): Generally Expansive

| Date | Event | Direction | Significance |
|------|-------|-----------|-------------|
| April 2010 | Arizona SB 1070 signed (state-level enforcement) | Restrictive | Medium |
| Dec 2010 | DREAM Act passes House, fails in Senate | Neutral | Medium |
| June 15, 2012 | DACA announced -- protects ~800,000 young immigrants | Expansive | High |
| Aug 2014 | EB-5 program hits capacity for first time | Neutral | Medium |
| Nov 20, 2014 | DAPA announced (expanded DACA) -- later blocked by courts | Expansive | High |
| Feb 2015 | H-4 EAD rule finalized -- spouses of H-1B holders can work | Expansive | High |
| Mar 11, 2016 | STEM OPT extension expanded to 24 months (36 months total) | Expansive | High |
| June 2016 | Supreme Court deadlocks 4-4 on DAPA, effectively blocking it | Restrictive | High |
| Jan 17, 2017 | International Entrepreneur Rule (IER) published as final rule | Expansive | High |

### 7.2 Trump First Term (2017-2021): Sharply Restrictive

| Date | Event | Direction | Significance |
|------|-------|-----------|-------------|
| Jan 27, 2017 | Travel Ban 1.0 -- 7 Muslim-majority countries; 700+ detained | Restrictive | Critical |
| Mar 6, 2017 | Travel Ban 2.0 -- revised to 6 countries | Restrictive | High |
| Apr 18, 2017 | Buy American Hire American EO signed | Restrictive | Critical |
| July 2017 | IER implementation delayed by DHS | Restrictive | High |
| Sept 5, 2017 | Trump announces end of DACA program | Restrictive | Critical |
| Sept 24, 2017 | Travel Ban 3.0 -- expanded to include Venezuela, North Korea | Restrictive | High |
| Dec 2017 | Federal court orders IER implementation | Expansive | Medium |
| Feb 2018 | USCIS rescission of Dec 2000 guidance on H-1B computer positions | Restrictive | High |
| June 26, 2018 | Supreme Court upholds travel ban (Trump v. Hawaii) | Restrictive | Critical |
| Feb 2019 | H-4 EAD rescission rule submitted to OIRA | Restrictive | High |
| Jan 31, 2020 | Travel ban expanded to 6 additional countries | Restrictive | High |
| Mar 10, 2020 | ITServe Alliance v. Cissna -- court strikes down itinerary requirement | Expansive | High |
| May 20, 2020 | ITServe settlement -- USCIS rescinds 2018 third-party worksite memo | Expansive | High |
| June 22, 2020 | Proclamation 10014: suspends immigrant entry (COVID context) | Restrictive | Critical |
| June 22, 2020 | Proclamation 10052: suspends H-1B, L-1, J-1 entry | Restrictive | Critical |
| Oct 2020 | DOL interim final rule raising prevailing wages (later vacated) | Restrictive | Medium |

### 7.3 Biden Administration (2021-2025): Expansive / Modernizing

| Date | Event | Direction | Significance |
|------|-------|-----------|-------------|
| Jan 20, 2021 | Biden takes office; begins rescinding Trump orders | Expansive | High |
| Jan 25, 2021 | H-4 EAD rescission rule withdrawn from OIRA review | Expansive | Medium |
| Mar 2021 | Biden rescinds Buy American Hire American EO | Expansive | High |
| May 2021 | IER proposed repeal withdrawn -- program revived | Expansive | Medium |
| June 2021 | USCIS Policy Alert PA-2021-05: restores deference to prior approvals | Expansive | High |
| Jan 21, 2022 | STEM talent initiatives: 22 new OPT fields added | Expansive | High |
| Jan 2022 | NIW guidance expanded for STEM professionals (EB-2) | Expansive | High |
| Mar 2022 | EB-5 Reform and Integrity Act signed | Expansive | Medium |
| Aug 2023 | EB-1 India retrogresses 10+ years (unprecedented backlog event) | Restrictive | High |
| Oct 2023 | H-1B modernization rule proposed | Expansive | Medium |
| Jan 17, 2025 | H-1B Modernization Final Rule takes effect (just before inauguration) | Expansive | High |

### 7.4 Trump Second Term (2025-present): Highly Restrictive

| Date | Event | Direction | Significance |
|------|-------|-----------|-------------|
| Jan 20, 2025 | 10 immigration EOs signed Day One: border emergency, asylum block, birthright citizenship attempt (blocked by 4 federal judges) | Restrictive | Critical |
| Jan 29, 2025 | Laken Riley Act signed -- mandatory detention for certain crimes | Restrictive | High |
| Sept 19, 2025 | Presidential Proclamation -- "Restriction on Entry of Certain Nonimmigrant Workers" | Restrictive | Critical |
| Sept 21, 2025 | $100,000 H-1B fee goes into effect for new petitions | Restrictive | Critical |
| Dec 15, 2025 | Enhanced social media vetting for H-1B and H-4 applicants | Restrictive | Medium |
| Dec 15, 2025 | Family Reunification Parole programs terminated | Restrictive | High |
| Dec 23, 2025 | Federal court upholds $100,000 H-1B fee | Restrictive | Critical |
| Jan 2026 | State Dept pauses immigrant visa processing from 75 countries | Restrictive | Critical |

---

## 8. Current Policy Landscape: Trump Second Term

### 8.1 The $100,000 H-1B Fee

The most significant policy change for high-skilled immigration since Buy American Hire American:

- **What:** Presidential Proclamation "Restriction on Entry of Certain Nonimmigrant Workers" (Sept 19, 2025)
- **Fee:** $100,000 per new H-1B petition filed for workers outside the U.S.
- **Previous cost:** ~$2,000-$5,000 per petition -- representing a **20-50x increase**
- **Effective:** September 21, 2025
- **Duration:** 12 months from effective date, subject to extension
- **Exemptions:** Does not apply to renewals, extensions, or previously issued H-1Bs. DHS can grant national interest exemptions.
- **Legal status:** Federal court upheld the fee on December 23, 2025, ruling it falls within broad executive power to restrict noncitizen entry.
- **Impact estimate:** A company sponsoring 10 new H-1B workers annually faces ~$1 million in additional costs.
- **Stated rationale:** Address "abuse" of H-1B program, prevent undercutting of U.S. worker wages, protect national security.

### 8.2 Day One Actions (January 20, 2025)

President Trump signed 10 immigration-related executive orders on his first day:
- Declared national emergency at the southern border
- Blocked asylum seekers from entering the U.S.
- Ended "catch and release" policy
- Attempted to end birthright citizenship for children of non-permanent-resident parents (Executive Order 14160 -- blocked by 4 federal judges; Supreme Court agreed to hear arguments)
- Suspended nearly all refugee admissions
- Restored "Remain in Mexico" policy
- Designated cartels as foreign terrorist organizations

### 8.3 Other Significant Actions

- **Laken Riley Act** (Jan 29, 2025): Mandates detention of immigrants charged with or convicted of certain crimes.
- **Enhanced social media vetting** (Dec 15, 2025): State Department expanded vetting to H-1B and H-4 nonimmigrants; applicants instructed to set social media profiles to "public."
- **Visa processing pause** (Jan 2026): State Department paused immigrant visa processing from 75 countries.
- **DOL prevailing wage increases** directed to ensure H-1B workers are not hired below market rates.
- **H-1B Modernization Rule status**: The Biden-era final rule (effective Jan 17, 2025) remains in effect as a formal regulation, requiring full rulemaking process to rescind. This provides some stability for provisions like entrepreneur self-petitioning and deference to prior approvals.

### 8.4 Policy Direction Signal

As of January 2026, Trump had signed 227 executive orders, 57 memoranda, and 116 proclamations in his second term. The immigration policy direction is decidedly restrictive, with the $100K H-1B fee representing the single largest financial barrier ever imposed on high-skilled visa sponsorship.

**Data sources:**
- [White House -- Restriction on Entry Fact Sheet (Sept 2025)](https://www.whitehouse.gov/fact-sheets/2025/09/fact-sheet-president-donald-j-trump-suspends-the-entry-of-certain-alien-nonimmigrant-workers/)
- [American Immigration Council -- $100K Fee Analysis](https://www.americanimmigrationcouncil.org/blog/uscis-implements-h1b-100000-fee/)
- [Ballotpedia -- Trump Executive Orders on Immigration 2025-2026](https://ballotpedia.org/Donald_Trump%27s_executive_orders_on_immigration,_2025)

---

## 9. Visualization Design Notes

### 9.1 Animated Line Chart with Policy-Era Bands
- **Data:** Section 2, Dataset 1 in timeline_data.md
- **X-axis:** FY 2010-2025; **Y-axis:** Denial Rate (%)
- **Background bands:** Obama (blue), Trump 1 (red), Biden (blue), Trump 2 (red)
- **Annotations:** Key policy events as vertical lines with labels (BAHA, Travel Ban, ITServe, PA-2021-05, $100K fee)
- **Animation:** Progressive reveal, left to right, pausing at each era transition
- **Methodological note overlay:** "Denial rates reflect USCIS adjudication policy. Temporal co-occurrence with policy changes does not establish causation."

### 9.2 Vertical Timeline
- **Data:** Dataset 5 in timeline_data.md
- **Layout:** Center vertical line, expansive events above, restrictive events below
- **Sizing:** Critical > High > Medium > Low (circle or marker size)
- **Color:** By era (Obama blue, Trump 1 red, Biden blue, Trump 2 red)
- **Hover/click:** Show full event description and source

### 9.3 Grouped Bar Chart: Green Card Wait Times
- **Data:** Dataset 8 in timeline_data.md
- **X-axis:** EB-1, EB-2, EB-3; **Y-axis:** Wait time in years
- **Groups:** India, China, Rest of World
- **Annotation:** "134-year theoretical wait" for EB-2 India new applicants
- **Context label:** "Annual cap: 140,000 (set in 1990, never updated)"

### 9.4 KPI Dashboard Cards: Brain Drain Metrics
- **Layout:** 4-6 large number cards with trend arrows
- Card 1: "75%" -- Scientists considering leaving the U.S. (Nature 2025 survey)
- Card 2: "82%" -- Employers who lost workers to visa issues (Envoy Global 2023)
- Card 3: "1.8M" -- Employment-based green card backlog (Cato)
- Card 4: "3x" -- Increase in ERC grant applications from U.S. (2024-2026)
- Card 5: "$100K" -- New H-1B petition fee (Sept 2025)
- Card 6: "134 years" -- Theoretical EB-2 India wait time

### 9.5 Small Multiples: Era Comparison
- **Data:** Dataset 11 in timeline_data.md
- **Metrics per panel:** Denial rate range, RFE rate peak, H-1B fee level, travel/visa restrictions, key executive action
- **Layout:** 4 columns (Obama, Trump 1, Biden, Trump 2)

### 9.6 Slope Chart: Before/After Key Policy Changes
- **Pair 1:** Denial rate pre-BAHA (FY 2016: 10%) vs. post-BAHA peak (FY 2018: 24%)
- **Pair 2:** Denial rate pre-Biden (FY 2020: 13%) vs. post-Biden (FY 2022: 2%)
- **Pair 3:** RFE rate pre-BAHA (FY 2017: 21.4%) vs. peak (FY 2019: 40.2%)
- **Pair 4:** H-1B fee pre-$100K ($2,000-$5,000) vs. post ($100,000)

### 9.7 Stacked Area Chart: H-1B Approvals by Nationality
- **Data:** Dataset 4 in timeline_data.md (supplemented with historical estimates)
- **X-axis:** FY 2010-2024; **Y-axis:** Approvals count or percentage
- **Stacks:** India (largest), China, Other
- **Note:** Historical data prior to FY 2019 requires interpolation from period averages

---

## 10. Sources

### Government Sources
- [USCIS H-1B Employer Data Hub](https://www.uscis.gov/tools/reports-and-studies/h-1b-employer-data-hub)
- [USCIS FY 2024 H-1B Characteristics Report (PDF)](https://www.uscis.gov/sites/default/files/document/reports/ola_signed_h1b_characteristics_congressional_report_FY24.pdf)
- [USCIS FY 2023 H-1B Characteristics Report (PDF)](https://www.uscis.gov/sites/default/files/document/reports/OLA_Signed_H1B_Characteristics_Congressional_Report_FY2023.pdf)
- [USCIS H-1B Electronic Registration Process](https://www.uscis.gov/working-in-the-united-states/temporary-workers/h-1b-specialty-occupations/h-1b-electronic-registration-process)
- [Dept of State -- Visa Bulletin](https://travel.state.gov/content/travel/en/legal/visa-law0/visa-bulletin.html)
- [White House -- Restriction on Entry Fact Sheet (Sept 2025)](https://www.whitehouse.gov/fact-sheets/2025/09/fact-sheet-president-donald-j-trump-suspends-the-entry-of-certain-alien-nonimmigrant-workers/)
- [White House Archives -- BAHA Executive Order](https://trumpwhitehouse.archives.gov/presidential-actions/presidential-executive-order-buy-american-hire-american/)
- [Canada.ca -- Start-up Visa Program Evaluation](https://www.canada.ca/en/immigration-refugees-citizenship/corporate/reports-statistics/evaluations/evaluation-start-up-visa-program.html)

### Research / Think Tanks
- [NFAP -- H-1B Denial Rate Table 2011-2024](https://nfap.com/newarticle/nfap-table-on-h-1b-denial-rate-2011-to-2024/)
- [NFAP -- FY 2025 Policy Brief (Nov 2025)](https://nfap.com/wp-content/uploads/2025/11/H-1B-Petitions-and-Denial-Rates-For-FY-2025.NFAP-Policy-Brief.2025.pdf)
- [NFAP -- FY 2024 Policy Brief](https://nfap.com/wp-content/uploads/2024/12/H-1B-Petitions-and-Denial-Rates-For-FY-2024.NFAP-Policy-Brief.December-2024.pdf)
- [Cato Institute -- 1.8 Million in EB Green Card Backlog](https://www.cato.org/blog/18-million-employment-based-green-card-backlog)
- [Pew Research Center -- H-1B Visa Program Data (March 2025)](https://www.pewresearch.org/short-reads/2025/03/04/what-we-know-about-the-us-h-1b-visa-program/)
- [ITIF -- US Brain Drain Threatens Leadership (Dec 2025)](https://itif.org/publications/2025/12/18/us-brain-drain-threatens-scientific-and-biopharmaceutical-leadership/)
- [Boundless -- 134-Year Wait for Indian Nationals](https://www.boundless.com/blog/indians-face-134-year-wait-employment-based-green-card)

### News and Analysis
- [American Immigration Council -- $100K Fee Analysis](https://www.americanimmigrationcouncil.org/blog/uscis-implements-h1b-100000-fee/)
- [Ballotpedia -- Trump Executive Orders on Immigration 2025-2026](https://ballotpedia.org/Donald_Trump%27s_executive_orders_on_immigration,_2025)
- [Visual Capitalist -- H-1B Approvals by Country 2024](https://www.visualcapitalist.com/visualized-h-1b-visa-approvals-by-country-in-2024/)
- [Fragomen -- Green Card Backlogs 2025](https://www.fragomen.com/insights/green-card-backlogs-and-visa-bulletin-trends-what-employers-can-do-in-2025-and-beyond.html)
- [Immigration Policy Tracking Project -- RFEs and Denials](https://immpolicytracking.org/policies/report-that-uscis-has-increased-rates-of-rfes-and-denials-of-h-1b-and-l-1-petitions/)
- [STAT News -- Brain Drain (Dec 2025)](https://www.statnews.com/2025/12/17/research-cuts-fuel-scientific-brain-drain-american-science-shattered/)
- [Global Citizen Solutions -- Canada SUV Statistics](https://www.globalcitizensolutions.com/canada-startup-visa-record-high/)
- [Statista -- Indians Renouncing Citizenship](https://www.statista.com/statistics/1378071/india-number-of-people-renouncing-citizenship/)

### Legal / Court Decisions Referenced
- ITServe Alliance, Inc. v. Cissna (D.D.C. 2020) -- struck down USCIS itinerary requirement for H-1B
- Trump v. Hawaii, 585 U.S. 667 (2018) -- upheld travel ban
- Federal court ruling upholding $100K H-1B fee (Dec 23, 2025)
- Four federal court injunctions blocking EO 14160 (birthright citizenship) (Feb 2025)
