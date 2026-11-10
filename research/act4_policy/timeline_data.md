# Act 4 -- Structured Datasets for Visualization

## Immigration Policy and Innovation Economy Data (REVISED)

*Last updated: March 2026*
*Note: All datasets below are descriptive. Temporal co-occurrence of policy changes with metric shifts does not establish causation. See findings.md Section 1 for full methodological note.*

---

## Dataset 1: H-1B Denial Rates for Initial Employment (FY 2010-2025)

**Visualization:** Animated line chart with policy-era background bands and annotated policy events.

```csv
fiscal_year,denial_rate_pct,approval_rate_pct,policy_era,era_color,key_event
2010,8.0,92.0,Obama,#3B82F6,
2011,7.0,93.0,Obama,#3B82F6,
2012,5.0,95.0,Obama,#3B82F6,DACA announced
2013,7.0,93.0,Obama,#3B82F6,
2014,8.0,92.0,Obama,#3B82F6,
2015,6.0,94.0,Obama,#3B82F6,H-4 EAD finalized
2016,10.0,90.0,Obama,#3B82F6,STEM OPT expanded
2017,13.0,87.0,Trump1,#EF4444,BAHA EO signed Apr 2017
2018,24.0,76.0,Trump1,#EF4444,Peak denial; Travel ban upheld
2019,21.0,79.0,Trump1,#EF4444,Peak RFE rate (40.2%)
2020,13.0,87.0,Trump1,#EF4444,ITServe settlement; COVID visa suspension
2021,4.0,96.0,Biden,#3B82F6,PA-2021-05; BAHA rescinded
2022,2.0,98.0,Biden,#3B82F6,Historic low; 442K total approvals
2023,3.5,96.5,Biden,#3B82F6,H-1B modernization proposed
2024,2.5,97.5,Biden,#3B82F6,Record 780K lottery registrations
2025,2.8,97.2,Trump2,#DC2626,$100K fee effective Sept 2025
```

**Sources:**
- NFAP H-1B Denial Rate Table 2011-2024: https://nfap.com/newarticle/nfap-table-on-h-1b-denial-rate-2011-to-2024/
- NFAP FY 2025 Policy Brief: https://nfap.com/wp-content/uploads/2025/11/H-1B-Petitions-and-Denial-Rates-For-FY-2025.NFAP-Policy-Brief.2025.pdf
- NFAP FY 2024 Policy Brief: https://nfap.com/wp-content/uploads/2024/12/H-1B-Petitions-and-Denial-Rates-For-FY-2024.NFAP-Policy-Brief.December-2024.pdf

**Notes:**
- FY 2010-2016 rates from NFAP analysis of USCIS data (FY 2016 10% figure confirmed in NFAP reporting).
- FY 2017 rate (13%) from NFAP; BAHA signed mid-year (Apr 2017) so full effect visible in FY 2018.
- FY 2025 rate (2.8%) from NFAP Nov 2025 report; covers full FY before $100K fee impact fully measured.
- All rates are for "initial employment" petitions only (new H-1B hires), not continuations/extensions.

---

## Dataset 2: H-1B Request for Evidence (RFE) Rates

**Visualization:** Overlay line on denial rate chart, or separate small-multiple panel.

```csv
fiscal_year,rfe_rate_pct,policy_era,post_rfe_approval_rate_pct
2015,22.0,Obama,
2016,22.0,Obama,
2017,21.4,Trump1,
2018,38.0,Trump1,60.0
2019,40.2,Trump1,
2020,28.8,Trump1,
2021,16.2,Biden,
2022,9.6,Biden,85.5
2023,10.5,Biden,79.8
```

**Sources:**
- USCIS FY 2023 H-1B Characteristics Report: https://www.uscis.gov/sites/default/files/document/reports/OLA_Signed_H1B_Characteristics_Congressional_Report_FY2023.pdf
- Immigration Policy Tracking Project: https://immpolicytracking.org/policies/report-that-uscis-has-increased-rates-of-rfes-and-denials-of-h-1b-and-l-1-petitions/

**Notes:**
- FY 2015-2016 values (~22%) are estimates based on pre-BAHA baselines.
- FY 2017-2021 values from USCIS data via multiple secondary sources.
- Post-RFE approval rate dropped to ~60% in FY 2018 (peak restrictive period).
- In FY 2023, 39,222 of 397,231 completed petitions (10%) received RFEs.

---

## Dataset 3: H-1B Lottery Registration and Selection

**Visualization:** Bar chart showing registrations vs. selections with selection rate line overlay.

```csv
fiscal_year,eligible_registrations,selected,selection_rate_pct,notes
2021,274000,106100,38.7,First year of electronic registration
2022,308613,131924,42.7,Including subsequent selection rounds
2023,474421,127600,26.9,Growing demand
2024,758994,110791,14.6,Record registrations; fraud concerns emerge
2025,470000,121000,25.6,38% drop after integrity rules (beneficiary-centric)
2026,336153,118660,35.3,Further decline; $100K fee announced during period
```

**Source:** USCIS H-1B Electronic Registration Process: https://www.uscis.gov/working-in-the-united-states/temporary-workers/h-1b-specialty-occupations/h-1b-electronic-registration-process

---

## Dataset 4: H-1B Approvals by Nationality (Stacked Area Chart)

**Visualization:** Stacked area chart showing India, China, Other shares over time.

```csv
fiscal_year,india_pct,china_pct,other_pct,total_approvals_approx,data_quality
2010,50.0,10.0,40.0,86600,estimated_from_period_avg
2011,50.0,10.0,40.0,84100,estimated_from_period_avg
2012,51.0,10.0,39.0,85300,estimated_from_period_avg
2013,51.0,10.0,39.0,,estimated_from_period_avg
2014,51.0,10.0,39.0,,estimated_from_period_avg
2015,51.0,10.0,39.0,275300,estimated_from_period_avg
2016,55.0,11.0,34.0,,interpolated
2017,60.0,12.0,28.0,,interpolated
2018,65.0,13.0,22.0,,interpolated
2019,72.0,13.0,15.0,,uscis_fy2019_report
2020,73.0,14.0,13.0,,estimated
2021,74.0,15.0,11.0,,estimated
2022,74.1,16.0,9.9,442425,pew_research
2023,73.0,12.0,15.0,386000,pew_research
2024,71.0,11.7,17.3,399395,uscis_official
```

**Sources:**
- Pew Research Center (March 2025): https://www.pewresearch.org/short-reads/2025/03/04/what-we-know-about-the-us-h-1b-visa-program/
- Visual Capitalist (2024): https://www.visualcapitalist.com/visualized-h-1b-visa-approvals-by-country-in-2024/
- USCIS FY 2024 Characteristics Report: https://www.uscis.gov/sites/default/files/document/reports/ola_signed_h1b_characteristics_congressional_report_FY24.pdf

**Notes:**
- FY 2010-2015: Pew reports "50.5% India, 9.7% China" as the 2001-2015 average. Individual year percentages are approximated.
- FY 2016-2018: Interpolated between 2015 period average and 2019 actuals.
- FY 2019 onward: Based on USCIS annual reports and Pew analysis.
- Total approvals not available for all years; consult USCIS annual reports.
- "data_quality" column indicates confidence level for each row.

---

## Dataset 5: Policy Events Timeline (Vertical Timeline Visualization)

**Visualization:** Vertical or horizontal timeline. Events above center line = expansive; below = restrictive. Marker size by significance. Color by era.

```csv
date,event,category,era,era_color,direction,significance,significance_score
2010-04-23,Arizona SB 1070 signed -- state immigration enforcement law,legislation,Obama,#3B82F6,restrictive,medium,2
2010-12-08,DREAM Act passes House but fails in Senate,legislation,Obama,#3B82F6,neutral,medium,2
2012-06-15,DACA announced -- protects ~800K young immigrants from deportation,executive_action,Obama,#3B82F6,expansive,high,3
2014-08-01,EB-5 Investor Visa program hits capacity for first time,visa_program,Obama,#3B82F6,neutral,medium,2
2014-11-20,DAPA announced -- expanded DACA eligibility (later blocked by courts),executive_action,Obama,#3B82F6,expansive,high,3
2015-02-25,H-4 EAD rule finalized -- H-1B spouses can work while awaiting green card,visa_program,Obama,#3B82F6,expansive,high,3
2016-03-11,STEM OPT extension expanded from 17 to 24 months (36 total),visa_program,Obama,#3B82F6,expansive,high,3
2016-06-23,Supreme Court deadlocks 4-4 on DAPA -- program effectively blocked,court_decision,Obama,#3B82F6,restrictive,high,3
2017-01-17,International Entrepreneur Rule (IER) published as final rule,visa_program,Obama,#3B82F6,expansive,high,3
2017-01-27,Travel Ban 1.0 -- 7 Muslim-majority countries barred; 700+ travelers detained,executive_action,Trump1,#EF4444,restrictive,critical,4
2017-03-06,Travel Ban 2.0 -- revised to 6 countries; 90-day restriction,executive_action,Trump1,#EF4444,restrictive,high,3
2017-04-18,Buy American Hire American (BAHA) Executive Order signed,executive_action,Trump1,#EF4444,restrictive,critical,4
2017-07-11,DHS delays International Entrepreneur Rule implementation,executive_action,Trump1,#EF4444,restrictive,high,3
2017-09-05,Trump announces termination of DACA program,executive_action,Trump1,#EF4444,restrictive,critical,4
2017-09-24,Travel Ban 3.0 -- expanded to include Venezuela and North Korea,executive_action,Trump1,#EF4444,restrictive,high,3
2017-12-01,Federal court orders DHS to implement the IER,court_decision,Trump1,#EF4444,expansive,medium,2
2018-02-22,USCIS rescinds Dec 2000 guidance on H-1B computer-related positions,agency_action,Trump1,#EF4444,restrictive,high,3
2018-06-26,Supreme Court upholds Travel Ban 3.0 in Trump v. Hawaii (5-4),court_decision,Trump1,#EF4444,restrictive,critical,4
2018-10-01,FY 2018 data: H-1B denial rate peaks at 24% -- 4x the pre-BAHA level,data_milestone,Trump1,#EF4444,restrictive,critical,4
2019-02-20,H-4 EAD rescission proposed rule submitted to OIRA,agency_action,Trump1,#EF4444,restrictive,high,3
2019-10-01,FY 2019 data: RFE rate peaks at 40.2% -- 2 in 5 petitions challenged,data_milestone,Trump1,#EF4444,restrictive,high,3
2020-01-31,Travel ban expanded to 6 additional countries (Nigeria included),executive_action,Trump1,#EF4444,restrictive,high,3
2020-03-10,ITServe Alliance v. Cissna -- court strikes down itinerary requirement for H-1B,court_decision,Trump1,#EF4444,expansive,high,3
2020-05-20,ITServe settlement -- USCIS rescinds 2018 third-party worksite memo,court_decision,Trump1,#EF4444,expansive,high,3
2020-06-22,Proclamation 10014 -- suspends immigrant entry citing COVID-19,executive_action,Trump1,#EF4444,restrictive,critical,4
2020-06-22,Proclamation 10052 -- suspends H-1B and L-1 and J-1 entry,executive_action,Trump1,#EF4444,restrictive,critical,4
2020-10-08,DOL interim final rule raising H-1B prevailing wages (later vacated by courts),agency_action,Trump1,#EF4444,restrictive,medium,2
2021-01-20,Biden takes office -- begins rescinding Trump immigration orders,executive_action,Biden,#3B82F6,expansive,high,3
2021-01-25,H-4 EAD rescission rule withdrawn from OIRA review,agency_action,Biden,#3B82F6,expansive,medium,2
2021-03-01,Biden formally rescinds Buy American Hire American EO,executive_action,Biden,#3B82F6,expansive,high,3
2021-05-10,IER proposed repeal withdrawn -- program revived,agency_action,Biden,#3B82F6,expansive,medium,2
2021-06-09,USCIS Policy Alert PA-2021-05 -- restores deference to prior H-1B approvals,agency_action,Biden,#3B82F6,expansive,high,3
2022-01-21,Biden STEM talent initiatives -- 22 new OPT-eligible fields added,visa_program,Biden,#3B82F6,expansive,high,3
2022-01-21,NIW guidance expanded for STEM professionals under EB-2,visa_program,Biden,#3B82F6,expansive,high,3
2022-03-15,EB-5 Reform and Integrity Act signed into law,legislation,Biden,#3B82F6,expansive,medium,2
2022-10-01,FY 2022 data: H-1B denial rate drops to 2% (historic low),data_milestone,Biden,#3B82F6,expansive,high,3
2023-08-01,EB-1 India retrogresses 10+ years -- unprecedented backlog spillover,data_milestone,Biden,#3B82F6,restrictive,high,3
2023-10-01,H-1B modernization rule proposed (NPRM published),agency_action,Biden,#3B82F6,expansive,medium,2
2024-03-06,FY 2024 H-1B lottery: record 780K+ registrations,data_milestone,Biden,#3B82F6,neutral,high,3
2025-01-17,H-1B Modernization Final Rule takes effect (3 days before inauguration),agency_action,Biden,#3B82F6,expansive,high,3
2025-01-20,Trump 2nd term Day One: 10 immigration EOs signed; border emergency declared,executive_action,Trump2,#DC2626,restrictive,critical,4
2025-01-20,EO 14160 -- attempts to end birthright citizenship (blocked by 4 federal judges),executive_action,Trump2,#DC2626,restrictive,high,3
2025-01-29,Laken Riley Act signed -- mandatory detention for certain immigrant crimes,legislation,Trump2,#DC2626,restrictive,high,3
2025-09-19,Presidential Proclamation: Restriction on Entry of Certain Nonimmigrant Workers,executive_action,Trump2,#DC2626,restrictive,critical,4
2025-09-21,$100K H-1B fee takes effect for new petitions (workers outside U.S.),executive_action,Trump2,#DC2626,restrictive,critical,4
2025-12-15,Enhanced social media vetting expanded to H-1B and H-4 applicants,agency_action,Trump2,#DC2626,restrictive,medium,2
2025-12-15,Family Reunification Parole programs terminated,executive_action,Trump2,#DC2626,restrictive,high,3
2025-12-23,Federal court upholds $100K H-1B fee as within executive authority,court_decision,Trump2,#DC2626,restrictive,critical,4
2026-01-15,State Dept pauses immigrant visa processing from 75 countries,agency_action,Trump2,#DC2626,restrictive,critical,4
```

**Sources:**
- Ballotpedia: https://ballotpedia.org/Donald_Trump%27s_executive_orders_on_immigration,_2025
- Wikipedia -- Immigration Policy Second Trump Admin: https://en.wikipedia.org/wiki/Immigration_policy_of_the_second_Trump_administration
- Wikipedia -- Trump Travel Bans: https://en.wikipedia.org/wiki/Travel_bans_under_the_Trump_administrations
- American Immigration Council -- Obama Legacy: https://www.americanimmigrationcouncil.org/blog/president-obamas-legacy-immigration/
- White House -- BAHA EO: https://trumpwhitehouse.archives.gov/presidential-actions/presidential-executive-order-buy-american-hire-american/
- White House -- Restriction on Entry Fact Sheet: https://www.whitehouse.gov/fact-sheets/2025/09/fact-sheet-president-donald-j-trump-suspends-the-entry-of-certain-alien-nonimmigrant-workers/

---

## Dataset 6: Green Card Wait Times by Category and Country

**Visualization:** Grouped bar chart. X = category, Y = wait years. Groups = India, China, ROW.

```csv
category,category_label,india_wait_years,china_wait_years,row_wait_years,india_priority_date,china_priority_date,as_of_date,total_backlog_pct_india
EB-1,Priority Workers / Extraordinary Ability,3.5,3.0,0,2022-03-01,2022-11-01,2025-12,
EB-2,Advanced Degree Professionals,12.5,4.5,0.5,2013-09-15,2021-12-01,2026-03,90
EB-3,Skilled Workers,11.5,4.0,0.5,2014-08-15,2022-01-01,2025-12,
EB-5,Immigrant Investors (post-RIA),0,0,0,current,current,2025-12,
```

**Supplementary backlog context:**

```csv
metric,value,unit,source
Total EB green card backlog,1800000,persons,Cato Institute 2024
India share of EB backlog,1100000,persons (63%),Cato Institute 2024
China share of EB backlog,250000,persons (14%),Cato Institute 2024
Annual EB visa cap,140000,visas,Immigration Act of 1990
Theoretical EB-2 India wait for new applicants,134,years,Boundless 2024
EB-1 India retrogression event,10+,years_backward,August 2023
Per-country cap,7,percent,INA Section 202(a)(2)
Total USCIS pending cases Q2 FY2025,11300000,cases,USCIS
PERM labor certification processing time,483,calendar_days,DOL mid-2025
```

**Sources:**
- Cato Institute: https://www.cato.org/blog/18-million-employment-based-green-card-backlog
- Boundless -- Visa Bulletin March 2026: https://www.boundless.com/blog/visa-bulletin
- Fragomen -- Green Card Backlogs 2025: https://www.fragomen.com/insights/green-card-backlogs-and-visa-bulletin-trends-what-employers-can-do-in-2025-and-beyond.html
- Boundless -- 134-Year Wait: https://www.boundless.com/blog/indians-face-134-year-wait-employment-based-green-card

---

## Dataset 7: Brain Drain Indicators (KPI Dashboard Cards)

**Visualization:** Large-number KPI cards with trend arrows and contextual labels.

```csv
metric_id,metric_label,value,unit,year,trend_direction,context,source_short,source_url
BD-1,Scientists considering leaving the U.S.,75,percent,2025,up,Nature poll of 1600 scientists; Europe and Canada top destinations,Nature 2025,https://www.statnews.com/2025/12/17/research-cuts-fuel-scientific-brain-drain-american-science-shattered/
BD-2,Employers who lost foreign workers to visa issues,82,percent,2023,up,Envoy Global employer survey; workers let go or reassigned,Envoy Global 2023,https://reason.com/2023/09/26/americas-immigrant-brain-drain/
BD-3,ERC grant applications from U.S. researchers,169,count,2026,up,Tripled from 60 (2024) to 116 (2025) to 169 (2026),Nature/ERC,https://itif.org/publications/2025/12/18/us-brain-drain-threatens-scientific-and-biopharmaceutical-leadership/
BD-4,Canada SUV permanent residents granted (record),5595,count,2024,up,7x processing growth from 2022; but Canada capping at 1000/yr by 2026,Canada IRCC,https://www.globalcitizensolutions.com/canada-startup-visa-record-high/
BD-5,Indian citizens renouncing citizenship (2024),206378,count,2024,up,Sustained above 200K since 2022; 1M+ in 6 years 2019-2024; primarily to US/UK/Australia/Canada,Indian MEA,https://www.visaverge.com/news/over-2-lakh-indians-renounced-citizenship-in-2024-govt-data-shows/
BD-6,Chinese-born PhD intent to stay in U.S.,77.5,percent,2023,down,Dropped from 81% in 2016; reflects both visa frustration and China opportunities,Survey data,https://ihe.bc.edu/pub/d6snhiz8
BD-7,Indian-born PhD intent to stay in U.S.,89,percent,2023,stable,High despite long waitlists; fewer scientific career options in India,Survey data,https://ihe.bc.edu/pub/d6snhiz8
BD-8,International scholars in U.S. vs 2018,82,percent_of_2018,2024,down,Down 18% from 2018 levels,Various,https://itif.org/publications/2025/12/18/us-brain-drain-threatens-scientific-and-biopharmaceutical-leadership/
BD-9,U.S. job seekers applying to Canada (YoY change),41,percent_increase,2025,up,Nature jobs board data; first months of 2nd Trump admin vs same period 2024,Nature,https://www.statnews.com/2025/12/17/research-cuts-fuel-scientific-brain-drain-american-science-shattered/
BD-10,Prominent Chinese scientists returning from U.S.,85,count,2025,up,Since Jan 2025; concentrated in AI and semiconductors,Various,https://ihe.bc.edu/pub/d6snhiz8
```

---

## Dataset 8: Indian Citizenship Renunciation (Time Series)

**Visualization:** Line chart or bar chart showing annual renunciations, with policy event annotations.

```csv
year,renunciations,policy_era,notable_event
2015,131489,Obama,
2016,141603,Obama,
2017,133049,Trump1,BAHA signed; Travel Ban 1.0
2018,134561,Trump1,Peak H-1B denial rate (24%)
2019,144017,Trump1,Pre-pandemic peak
2020,85256,Trump1,COVID-19 pandemic; embassy closures
2021,163370,Biden,Post-pandemic surge; embassies reopen
2022,225620,Biden,Record high; H-1B denial rate historic low
2023,216219,Biden,Near-record
2024,206378,Biden/Trump2,Sustained high level
```

**Source:** Statista: https://www.statista.com/statistics/1378071/india-number-of-people-renouncing-citizenship/

**Notes:**
- Renunciation of Indian citizenship is required when obtaining citizenship of another country (India does not permit dual citizenship).
- The 2020 dip reflects COVID-related embassy closures globally, not reduced intent.
- Not all renunciations are tech/startup-related; includes all sectors and all destination countries.
- Top destination countries for renunciants: U.S., UK, Australia, Canada.

---

## Dataset 9: Canada Start-Up Visa Program Growth

**Visualization:** Line or bar chart showing program growth and policy changes.

```csv
year,new_prs_granted,applications_in_system,processing_volume,incubator_refusal_rate_pct,policy_note
2020,,2000,,10,COVID disruption; minimal processing
2021,,,,,Post-pandemic recovery begins
2022,,5000,601,,Processing ramp-up
2023,,,,,Refusal rate ~10% (incubators)
2024,5595,18514,6000,,Record year; 7x volume growth from 2022
2025,,18000,,73,Cap reduced to 2000; refusal rate surges
2026,,,,,"Cap 1000; Canada developing new pilot program"
2027,,,,,"Cap 1000; continued restrictions"
```

**Source:** Global Citizen Solutions: https://www.globalcitizensolutions.com/canada-startup-visa-record-high/; Canada.ca: https://www.canada.ca/en/immigration-refugees-citizenship/corporate/reports-statistics/evaluations/evaluation-start-up-visa-program.html

---

## Dataset 10: H-1B Fee Comparison (Slope Chart)

**Visualization:** Slope chart or before/after comparison showing the magnitude of the fee change.

```csv
fee_component,pre_sept_2025_usd,post_sept_2025_usd,multiplier,notes
Base filing fee (I-129),460,460,1x,Unchanged
ACWIA fee (25 or fewer employees),750,750,1x,Unchanged
ACWIA fee (26+ employees),1500,1500,1x,Unchanged
Fraud prevention fee,500,500,1x,Unchanged
Asylum program fee,600,600,1x,Unchanged
Registration fee,215,215,1x,Unchanged
NEW: Proclamation surcharge fee,0,100000,new,For new petitions only; workers outside U.S.
Total for small employer (new petition),2525,102525,~41x,"Illustrative total for new H-1B, small employer"
Total for large employer (new petition),3275,103275,~32x,"Illustrative total for new H-1B, large employer"
Premium processing (optional),2805,2805,1x,Unchanged; expedited adjudication
```

**Source:** American Immigration Council: https://www.americanimmigrationcouncil.org/blog/uscis-implements-h1b-100000-fee/; Boundless: https://www.boundless.com/blog/trump-administration-to-propose-new-100000-fee-for-h-1b-visa-applications

---

## Dataset 11: Policy Era Comparison (Small Multiples)

**Visualization:** Four-column comparison grid. Each column = one policy era. Each row = one metric.

```csv
metric,metric_label,obama_2010_2016,trump1_2017_2020,biden_2021_2024,trump2_2025_present
denial_rate_range,H-1B Denial Rate Range,5-10%,13-24%,2-3.5%,2.8% (rising expected)
denial_rate_peak,Peak Denial Rate,10% (FY2016),24% (FY2018),3.5% (FY2023),TBD
rfe_rate_peak,Peak RFE Rate,~22%,40.2% (FY2019),10.5% (FY2023),TBD
h1b_new_petition_fee,H-1B New Petition Fee,$2K-$5K,$2K-$5K,$2K-$5K,$100K+
travel_visa_bans,Travel/Visa Restrictions,None,13+ countries banned,Bans rescinded,75 countries paused
stem_opt_expansion,STEM OPT Changes,Extended to 36 months,None,22 new fields added,None
ier_status,Intl Entrepreneur Rule,Published as final rule,Sabotaged (1 approval),Revived and updated,Status uncertain
h4_ead_status,H-4 Spouse Work Auth,Created (2015),Attempted rescission (failed),Preserved,Under review
key_executive_action,Signature Policy,DACA + STEM OPT,"BAHA + Travel Bans",H-1B Modernization,$100K Fee + Visa Pause
entrepreneur_policy_direction,Direction for Founders,Supportive,Hostile,Supportive,Hostile
green_card_backlog_eb2_india,EB-2 India Wait (approx),8-10 years,10-12 years,12-15 years,15-18 years (growing)
```

---

## Dataset 12: Slope Chart Data -- Before/After Key Policy Changes

**Visualization:** Connected slope lines showing metric changes around policy pivots.

```csv
policy_change,metric,before_label,before_value,after_label,after_value,change_direction,time_span
Buy American Hire American (Apr 2017),H-1B Denial Rate %,FY 2016,10.0,FY 2018 (peak),24.0,up,2 years
Buy American Hire American (Apr 2017),RFE Rate %,FY 2017,21.4,FY 2019 (peak),40.2,up,2 years
Biden Transition + ITServe (2020-2021),H-1B Denial Rate %,FY 2020,13.0,FY 2022,2.0,down,2 years
Biden Transition (2021),RFE Rate %,FY 2020,28.8,FY 2022,9.6,down,2 years
$100K Fee (Sept 2025),H-1B New Petition Cost,$,3275,$,103275,up,immediate
$100K Fee (Sept 2025),FY 2026 Lottery Registrations (unique),FY 2025,470000,FY 2026,336153,down,1 year
Canada SUV Growth (2022-2024),Annual Processing Volume,2022,601,2024,6000,up,2 years
Indian Citizenship Renunciation (COVID bounce),Annual Renunciations,2020,85256,2022,225620,up,2 years
```

---

## Era Band Definitions (for Background Bands on Charts)

```csv
era,era_label,start_fy,end_fy,color_hex,color_rgba_20pct,direction_label
Obama,Obama Administration,2010,2016,#3B82F6,"rgba(59,130,246,0.15)",Generally Expansive
Trump1,Trump First Term,2017,2020,#EF4444,"rgba(239,68,68,0.15)",Sharply Restrictive
Biden,Biden Administration,2021,2024,#3B82F6,"rgba(59,130,246,0.15)",Expansive / Modernizing
Trump2,Trump Second Term,2025,2026,#DC2626,"rgba(220,38,38,0.15)",Highly Restrictive
```

---

## Annotation Points for Denial Rate Chart

These annotations should appear as vertical lines or callout labels on the animated denial rate line chart (Dataset 1).

```csv
fiscal_year_position,label_short,label_full,y_offset_direction
2012,DACA,DACA announced (June 2012),above
2015,H-4 EAD,H-4 EAD rule finalized,above
2016,STEM OPT,STEM OPT extended to 36 months,above
2017,BAHA,Buy American Hire American EO (Apr 2017),below
2017.1,Travel Ban,Travel Ban 1.0 (Jan 2017),below
2018,Peak 24%,H-1B denial rate peaks at 24%,below
2020,ITServe,ITServe settlement -- key memo rescinded,above
2020.1,COVID Suspension,H-1B/L-1 entry suspended (June 2020),below
2021,PA-2021-05,USCIS restores deference to prior approvals,above
2022,Historic Low,Denial rate drops to 2% (historic low),above
2025,$100K Fee,$100K H-1B fee takes effect (Sept 2025),below
2026,75-Country Pause,State Dept pauses visa processing from 75 countries,below
```

---

## Data Quality and Caveats

1. **FY 2010-2016 denial rates**: Sourced from NFAP analysis of USCIS data. NFAP confirmed FY 2016 = 10%. FY 2010-2015 values (5-8%) from NFAP period reporting.
2. **FY 2017 denial rate**: NFAP reports 13%. Some sources report slightly different figures depending on how initial vs. continuing employment is counted.
3. **RFE rates pre-2017**: Estimated at ~22% based on available baselines. Exact figures for FY 2015-2016 not widely reported.
4. **Nationality breakdown pre-2019**: Based on Pew Research period average (2001-2015: India 50.5%, China 9.7%). Year-by-year figures interpolated.
5. **Green card wait times**: These are estimates based on current movement rates. Actual wait times depend on future filing volumes, visa availability, and potential legislative changes.
6. **Canada SUV data**: Program statistics are incomplete for some years. Processing volume vs. PRs granted are different metrics.
7. **Indian renunciation data**: Reflects all citizenship changes, not just tech/startup-sector departures.
8. **Brain drain surveys**: Self-reported intent (e.g., "considering leaving") does not equal actual departure. Nature poll is a convenience sample.
9. **Causal language**: This dataset supports descriptive visualization only. Temporal co-occurrence between policy changes and metric shifts should not be presented as causation without appropriate caveats.
