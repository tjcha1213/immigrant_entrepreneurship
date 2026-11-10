# Act 3 -- Visualization Data Tables

## Structured Data for Choropleth Maps, Sankey Diagrams, Heatmaps, Bubble Charts, Network Graphs, and Treemaps

**Purpose:** Data tables formatted for direct use in D3.js, Plotly, Scrollama, or similar visualization tools.
**Primary Data Sources:** NFAP 2022 (319 companies), AIC Fortune 500 2025 (231 companies)
**Secondary Sources:** CSET Georgetown, IFP, PitchBook, public market data

---

## Methodological Notes for Visualization

- **NFAP data** reflects companies identified as of May 2022. Valuations have been updated to early 2026 where public data is available.
- **Estimated values** (marked with "est") are derived from applying ratios or manual classification; they should be displayed with appropriate uncertainty indicators (e.g., lighter colors, dotted borders, or footnotes).
- **Lat/lng coordinates** are centroid approximations for countries and cities, suitable for map plotting but not precise to any specific address.
- **Flow weights** in Sankey data are relative measures (not absolute company counts) indicating the strength of origin-destination-industry connections, scaled 1-40.
- **Heatmap scores** are on a 0-5 scale reflecting concentration/dominance, not absolute counts.

---

## TABLE 1: World Choropleth Map -- Country of Origin Data

**Visualization type:** World choropleth map (color intensity = number of companies)
**Source:** NFAP 2022 (319 billion-dollar companies from 57 countries)

| country_code | country_name | lat | lng | num_billion_dollar_companies | pct_of_319_total | region | sub_region |
|-------------|--------------|-----|-----|------------------------------|-----------------|--------|-----------|
| IN | India | 20.5937 | 78.9629 | 66 | 20.7 | Asia | South Asia |
| IL | Israel | 31.0461 | 34.8516 | 54 | 16.9 | Middle East | Western Asia |
| GB | United Kingdom | 55.3781 | -3.4360 | 27 | 8.5 | Europe | Northern Europe |
| CA | Canada | 56.1304 | -106.3468 | 22 | 6.9 | North America | Northern America |
| CN | China | 35.8617 | 104.1954 | 21 | 6.6 | Asia | East Asia |
| FR | France | 46.2276 | 2.2137 | 18 | 5.6 | Europe | Western Europe |
| DE | Germany | 51.1657 | 10.4515 | 15 | 4.7 | Europe | Western Europe |
| RU | Russia | 61.5240 | 105.3188 | 11 | 3.4 | Europe/Asia | Eastern Europe |
| UA | Ukraine | 48.3794 | 31.1656 | 10 | 3.1 | Europe | Eastern Europe |
| IR | Iran | 32.4279 | 53.6880 | 8 | 2.5 | Middle East | Western Asia |
| AU | Australia | -25.2744 | 133.7751 | 7 | 2.2 | Oceania | Oceania |
| RO | Romania | 45.9432 | 24.9668 | 6 | 1.9 | Europe | Eastern Europe |
| IT | Italy | 41.8719 | 12.5674 | 6 | 1.9 | Europe | Southern Europe |
| PL | Poland | 51.9194 | 19.1451 | 6 | 1.9 | Europe | Eastern Europe |
| NG | Nigeria | 9.0820 | 8.6753 | 6 | 1.9 | Africa | West Africa |
| KR | South Korea | 35.9078 | 127.7669 | 5 | 1.6 | Asia | East Asia |
| NZ | New Zealand | -40.9006 | 174.8860 | 5 | 1.6 | Oceania | Oceania |
| PK | Pakistan | 30.3753 | 69.3451 | 5 | 1.6 | Asia | South Asia |
| AR | Argentina | -38.4161 | -63.6167 | 5 | 1.6 | South America | South America |
| BR | Brazil | -14.2350 | -51.9253 | 5 | 1.6 | South America | South America |
| TW | Taiwan | 23.6978 | 120.9605 | 5 | 1.6 | Asia | East Asia |
| ES | Spain | 40.4637 | -3.7492 | 4 | 1.3 | Europe | Southern Europe |
| PT | Portugal | 39.3999 | -8.2245 | 4 | 1.3 | Europe | Southern Europe |
| DK | Denmark | 56.2639 | 9.5018 | 4 | 1.3 | Europe | Northern Europe |
| IE | Ireland | 53.1424 | -7.6921 | 3 | 0.9 | Europe | Northern Europe |
| ZA | South Africa | -30.5595 | 22.9375 | 3 | 0.9 | Africa | Southern Africa |
| LB | Lebanon | 33.8547 | 35.8623 | 2 | 0.6 | Middle East | Western Asia |
| SE | Sweden | 60.1282 | 18.6435 | 2 | 0.6 | Europe | Northern Europe |
| TR | Turkey | 38.9637 | 35.2433 | 2 | 0.6 | Middle East | Western Asia |
| SG | Singapore | 1.3521 | 103.8198 | 2 | 0.6 | Asia | Southeast Asia |

**Notes:**
- China count (21) includes some founders born in mainland China who may have spent formative years in Taiwan or Hong Kong. NFAP does not always distinguish.
- Taiwan listed separately with 5 companies based on cross-referencing (NVIDIA's Jensen Huang, Yahoo's Jerry Yang, AMD's Lisa Su, etc.), but there is overlap with the China count in some sources.
- Total countries represented: 57. Countries with 1 company each (not listed individually): ~27 countries.
- Data current to May 2022. New unicorns since then are not captured.

---

## TABLE 2: Country x Industry Heatmap Matrix

**Visualization type:** Heatmap matrix (rows = countries, columns = industries)
**Scale:** 0 = no presence, 1 = minimal, 2 = moderate, 3 = notable, 4 = strong, 5 = dominant/world-leading
**Derivation:** Scores assigned based on number of identified companies per country-industry pair, cross-referenced with NFAP company list and public data. These are qualitative assessments, not precise counts.

| country_name | country_code | software_saas | ai_ml | cybersecurity | fintech | biotech_pharma | hardware_semi | ecommerce | space_defense | cloud_infra |
|-------------|-------------|---------------|-------|---------------|---------|----------------|---------------|-----------|---------------|-------------|
| India | IN | 5 | 5 | 2 | 4 | 2 | 2 | 3 | 1 | 4 |
| Israel | IL | 4 | 3 | 5 | 2 | 1 | 2 | 1 | 4 | 3 |
| China/Taiwan | CN/TW | 2 | 3 | 1 | 1 | 1 | 5 | 3 | 1 | 2 |
| United Kingdom | GB | 3 | 4 | 2 | 3 | 2 | 1 | 1 | 1 | 2 |
| Canada | CA | 3 | 2 | 2 | 2 | 1 | 1 | 1 | 1 | 3 |
| France | FR | 2 | 2 | 1 | 2 | 4 | 1 | 1 | 1 | 1 |
| Germany | DE | 2 | 1 | 1 | 3 | 1 | 1 | 1 | 3 | 1 |
| Russia | RU | 2 | 3 | 2 | 2 | 1 | 1 | 1 | 1 | 1 |
| Ukraine | UA | 2 | 1 | 1 | 2 | 1 | 1 | 1 | 1 | 1 |
| Iran | IR | 1 | 3 | 1 | 3 | 1 | 1 | 4 | 1 | 2 |
| Ireland | IE | 1 | 1 | 1 | 5 | 1 | 1 | 1 | 1 | 1 |
| South Africa | ZA | 1 | 1 | 1 | 2 | 1 | 1 | 1 | 5 | 1 |
| Lebanon | LB | 1 | 1 | 1 | 1 | 5 | 1 | 1 | 1 | 1 |
| South Korea | KR | 2 | 2 | 1 | 1 | 1 | 3 | 2 | 1 | 1 |
| Nigeria | NG | 2 | 1 | 1 | 3 | 1 | 1 | 1 | 1 | 1 |

**Interpretation guide for visualization tooltip:**
- 5 = "World-leading concentration" (e.g., Israel in cybersecurity, India in AI/SaaS)
- 4 = "Strong presence" (multiple major companies)
- 3 = "Notable presence" (several companies or one dominant player)
- 2 = "Moderate presence" (a few companies)
- 1 = "Minimal or no identified companies"
- 0 = "No presence identified"

**Caveat:** Scores are based on the NFAP dataset and publicly known companies. Smaller, less visible startups may not be captured.

---

## TABLE 3: SVG U.S. Map -- State-Level Data

**Visualization type:** SVG U.S. map with state fill colors

### 3A: NFAP Unicorn Data by State (2018 subset, N=50)

| state_code | state_name | num_immigrant_billion_dollar_cos | pct_of_subset | data_source |
|-----------|------------|----------------------------------|--------------|-------------|
| CA | California | 33 | 66.0 | NFAP 2018 |
| NY | New York | 8 | 16.0 | NFAP 2018 |
| MA | Massachusetts | 5 | 10.0 | NFAP 2018 |
| IL | Illinois | 2 | 4.0 | NFAP 2018 |
| FL | Florida | 1 | 2.0 | NFAP 2018 |
| WA | Washington | 1 | 2.0 | NFAP 2018 |

*Caveat: This is from the 50-company 2018 NFAP report, not the full 319-company 2022 dataset. State-level data for the full 2022 dataset is not publicly available.*

### 3B: AIC Fortune 500 Immigrant-Founded Companies by State (2025)

| state_code | state_name | num_fortune500_immigrant_cos | combined_revenue_billions | employees_worldwide | data_source |
|-----------|------------|------------------------------|--------------------------|--------------------|----|
| NY | New York | 34 | 1383 | 1889949 | AIC 2025 |
| CA | California | 30 | 1673 | 1686087 | AIC 2025 |
| TX | Texas | 22 | 807 | 1029253 | AIC 2025 |
| IL | Illinois | 15 | -- | -- | AIC 2025 (est) |
| FL | Florida | 12 | -- | -- | AIC 2025 (est) |
| VA | Virginia | 10 | -- | -- | AIC 2025 (est) |
| PA | Pennsylvania | 8 | -- | -- | AIC 2025 (est) |
| OH | Ohio | 7 | -- | -- | AIC 2025 (est) |
| GA | Georgia | 6 | -- | -- | AIC 2025 (est) |
| MN | Minnesota | 5 | -- | -- | AIC 2025 (est) |

*Note: Only NY, CA, and TX have confirmed counts and revenue figures from the AIC report. IL through MN counts are estimated based on partial data in AIC press materials and the overall Fortune 500 distribution.*

---

## TABLE 4: U.S. Metro-Area Bubble Overlay Data

**Visualization type:** Bubble overlay on U.S. SVG map (bubble size = number of companies or total valuation)

| city | state | lat | lng | total_unicorns_all | immigrant_founded_est | total_valuation_est_billions | primary_industries | notable_companies |
|------|-------|-----|-----|--------------------|-----------------------|------------------------------|--------------------|----|
| San Francisco | CA | 37.7749 | -122.4194 | 211 | 116 | 800 | Fintech, AI, SaaS | Stripe, Databricks, Cloudflare |
| San Jose / Silicon Valley | CA | 37.3382 | -121.8863 | 60 | 33 | 3500 | Semiconductors, AI, Enterprise SW | NVIDIA, Palo Alto Networks, Zoom |
| New York City | NY | 40.7128 | -74.0060 | 124 | 68 | 250 | Fintech, Media, Cybersecurity | Wiz, various |
| Boston / Cambridge | MA | 42.3601 | -71.0589 | 25 | 14 | 80 | Biotech, AI, EdTech | Moderna, Coursera |
| Los Angeles | CA | 34.0522 | -118.2437 | 37 | 20 | 100 | Media, Entertainment, AI | Snap, various |
| Seattle | WA | 47.6062 | -122.3321 | 12 | 7 | 60 | Cloud, AI, E-commerce | (Microsoft/Amazon ecosystem) |
| Austin | TX | 30.2672 | -97.7431 | 16 | 9 | 1100 | EVs, Enterprise SW | Tesla (HQ) |
| Chicago | IL | 41.8781 | -87.6298 | 14 | 8 | 30 | Enterprise SW, Fintech | Various |
| Miami | FL | 25.7617 | -80.1918 | 8 | 4 | 15 | Fintech, Crypto | Emerging hub |
| Washington DC / NoVA | DC | 38.9072 | -77.0369 | 8 | 4 | 30 | Defense Tech, Cybersecurity | Various |
| Denver | CO | 39.7392 | -104.9903 | 8 | 4 | 260 | Data Analytics | Palantir (HQ) |
| Houston | TX | 29.7604 | -95.3698 | 5 | 3 | 20 | Energy Tech | Various |
| Starbase / Brownsville | TX | 25.9975 | -97.1560 | 1 | 1 | 350 | Aerospace | SpaceX (HQ) |
| San Mateo / South SF | CA | 37.5585 | -122.2711 | 8 | 4 | 170 | SaaS, Fintech | Stripe, Freshworks |

**Notes:**
- "Total unicorns all" based on StartupBlink/Failory data for all unicorns (not just immigrant-founded).
- "Immigrant founded est" applies the 55% NFAP ratio as an approximation. Actual ratios vary by city.
- Austin's high valuation reflects Tesla HQ relocation. Denver's high valuation reflects Palantir HQ.
- San Jose/Silicon Valley valuation dominated by NVIDIA ($3T+).

---

## TABLE 5: Sankey / Alluvial Diagram -- Origin Country to U.S. City to Industry

**Visualization type:** Sankey diagram with three columns: Origin Country | U.S. City | Industry
**Flow weight:** Relative measure (1-40 scale) indicating strength of connection. NOT absolute company counts.

| origin_country | us_destination | industry | flow_weight | example_company |
|---------------|---------------|----------|-------------|-----------------|
| India | Silicon Valley | AI/SaaS | 40 | Freshworks, Eightfold.ai |
| India | Silicon Valley | Enterprise SW | 25 | AppDynamics |
| India | Seattle | Cloud/AI | 15 | (Microsoft/Amazon ecosystem) |
| India | New York | Fintech | 10 | Various |
| India | San Francisco | AI/Recruitment | 8 | Mercor |
| India | Boston | Biotech | 5 | Various |
| India | Houston | Fintech/SW | 3 | HighRadius |
| Israel | Silicon Valley | Cybersecurity | 30 | Palo Alto Networks, Check Point |
| Israel | New York | Cybersecurity/AI | 15 | Wiz, Cyera |
| Israel | Silicon Valley | Enterprise SW | 10 | Houzz, various |
| Israel | Austin | InsurTech | 5 | Hippo Insurance |
| Israel | Silicon Valley | Defense Tech | 8 | Various |
| China/Taiwan | Silicon Valley | Semiconductors | 30 | NVIDIA, Marvell, AMD |
| China/Taiwan | Silicon Valley | Internet/AI | 15 | Yahoo, various |
| China/Taiwan | San Jose | Video/Comms | 10 | Zoom |
| China/Taiwan | San Francisco | Food Delivery | 10 | DoorDash |
| Iran | San Jose | E-commerce | 15 | eBay |
| Iran | San Francisco | AI/Data | 15 | Databricks |
| Iran | San Francisco | Cloud/SaaS | 10 | Dropbox |
| Ireland | San Francisco | Fintech | 25 | Stripe |
| Russia | Mountain View | Internet/AI | 25 | Google/Alphabet |
| Russia | Silicon Valley | AI | 5 | Various |
| Ukraine | Silicon Valley | Fintech | 12 | PayPal (Max Levchin) |
| Ukraine | Menlo Park | Messaging | 10 | WhatsApp (Jan Koum) |
| South Africa | Starbase TX | Aerospace | 20 | SpaceX |
| South Africa | Austin TX | EVs/Energy | 15 | Tesla |
| Germany | Silicon Valley | Fintech | 10 | PayPal (Peter Thiel) |
| Germany | Denver | Data Analytics | 10 | Palantir |
| France | Boston/Cambridge | Biotech | 15 | Moderna (Bancel) |
| France | Silicon Valley | AI | 5 | Various |
| Canada | San Francisco | Cloud/SaaS | 15 | Slack, Cloudflare |
| Canada | New York | Media | 10 | Vice Media |
| Lebanon | Boston/Cambridge | Biotech | 12 | Moderna (Afeyan) |
| UK | Silicon Valley | AI | 10 | Various |
| UK | New York | Fintech | 8 | Various |
| UK | Boston | AI/Research | 5 | Various |
| Nigeria | Silicon Valley | AI Hardware | 5 | SambaNova Systems |
| Nigeria | New York | Fintech | 4 | Various |
| South Korea | Silicon Valley | Hardware/AI | 5 | Various |

**Notes:**
- Flow weights are relative and proportional; the highest weight (40) represents the strongest identified connection (India -> Silicon Valley -> AI/SaaS).
- "Various" indicates multiple smaller companies rather than a single iconic example.
- This data is derived from the NFAP company list and public company headquarters data, not from a systematic flow survey.

---

## TABLE 6: Bubble Chart -- Top 30 Immigrant-Founded Companies

**Visualization type:** Bubble chart (x = industry category, y = log(valuation), color = origin country, size = log(employees))

| company | founder | origin_country | origin_code | industry | industry_category | us_city | us_state | city_lat | city_lng | valuation_billions | year_founded | status | employees_est |
|---------|---------|---------------|-------------|----------|-------------------|---------|----------|---------|---------|-------------------|--------------|--------|---------------|
| NVIDIA | Jensen Huang | Taiwan | TW | Semiconductors/AI | Hardware/Semi | Santa Clara | CA | 37.3541 | -121.9552 | 3000 | 1993 | Public | 30000 |
| Alphabet/Google | Sergey Brin | Russia | RU | Internet/AI | AI/ML | Mountain View | CA | 37.3861 | -122.0839 | 2200 | 1998 | Public | 180000 |
| Tesla | Elon Musk | South Africa | ZA | EVs/Energy | Space/Defense | Austin | TX | 30.2672 | -97.7431 | 1100 | 2003 | Public | 140000 |
| SpaceX | Elon Musk | South Africa | ZA | Aerospace | Space/Defense | Starbase | TX | 25.9975 | -97.1560 | 350 | 2002 | Private | 13000 |
| Palantir | Peter Thiel | Germany | DE | Data Analytics | AI/ML | Denver | CO | 39.7392 | -104.9903 | 250 | 2003 | Public | 3800 |
| Stripe | Patrick & John Collison | Ireland | IE | Fintech/Payments | Fintech | South San Francisco | CA | 37.6547 | -122.4077 | 159 | 2010 | Private | 7000 |
| Palo Alto Networks | Nir Zuk | Israel | IL | Cybersecurity | Cybersecurity | Santa Clara | CA | 37.3541 | -121.9552 | 130 | 2005 | Public | 15000 |
| Marvell Technology | Weili Dai | China | CN | Semiconductors | Hardware/Semi | Wilmington | DE | 39.7459 | -75.5466 | 80 | 1995 | Public | 6000 |
| PayPal | Peter Thiel, Max Levchin | Germany/Ukraine | DE/UA | Fintech | Fintech | San Jose | CA | 37.3382 | -121.8863 | 80 | 1998 | Public | 27000 |
| DoorDash | Tony Xu | China | CN | Food Delivery | E-commerce | San Francisco | CA | 37.7749 | -122.4194 | 75 | 2013 | Public | 20000 |
| Databricks | Ali Ghodsi | Iran/Sweden | IR | AI/Data | AI/ML | San Francisco | CA | 37.7749 | -122.4194 | 62 | 2013 | Private | 8000 |
| Cloudflare | Michelle Zatlyn | Canada | CA | Cloud/CDN | Cloud/Infra | San Francisco | CA | 37.7749 | -122.4194 | 40 | 2009 | Public | 4000 |
| Wiz | Assaf Rappaport | Israel | IL | Cloud Security | Cybersecurity | New York | NY | 40.7128 | -74.0060 | 32 | 2020 | Acquired | 1800 |
| eBay | Pierre Omidyar | Iran/France | IR | E-commerce | E-commerce | San Jose | CA | 37.3382 | -121.8863 | 30 | 1995 | Public | 12000 |
| Slack | Stewart Butterfield | Canada | CA | Enterprise Comms | Software/SaaS | San Francisco | CA | 37.7749 | -122.4194 | 27.7 | 2009 | Acquired | 2500 |
| Zoom | Eric Yuan | China | CN | Video Comms | Software/SaaS | San Jose | CA | 37.3382 | -121.8863 | 25 | 2011 | Public | 8500 |
| WhatsApp | Jan Koum | Ukraine | UA | Messaging | Software/SaaS | Menlo Park | CA | 37.4530 | -122.1817 | 19 | 2009 | Acquired | 50 |
| Moderna | Noubar Afeyan | Lebanon | LB | Biotech/Pharma | Biotech/Pharma | Cambridge | MA | 42.3736 | -71.1097 | 15 | 2010 | Public | 5000 |
| Mercor | Varun Vummadi | India | IN | AI/Recruitment | AI/ML | San Francisco | CA | 37.7749 | -122.4194 | 10 | 2023 | Private | 200 |
| Dropbox | Arash Ferdowsi | Iran | IR | Cloud Storage | Cloud/Infra | San Francisco | CA | 37.7749 | -122.4194 | 10 | 2007 | Public | 2800 |
| Cyera | Yotam Segev | Israel | IL | Cybersecurity/AI | Cybersecurity | New York | NY | 40.7128 | -74.0060 | 9 | 2021 | Private | 500 |
| Freshworks | Girish Mathrubootham | India | IN | SaaS/CRM | Software/SaaS | San Mateo | CA | 37.5630 | -122.3255 | 5 | 2010 | Public | 5500 |
| Vice Media | Shane Smith | Canada | CA | Media | Other | Brooklyn | NY | 40.6782 | -73.9442 | 5.7 | 1994 | Acquired | 1500 |
| SambaNova Systems | Kunle Olukotun | Nigeria | NG | AI Hardware | Hardware/Semi | Palo Alto | CA | 37.4419 | -122.1430 | 5 | 2017 | Private | 500 |
| Cato Networks | Shlomo Kramer | Israel | IL | Cybersecurity/SASE | Cybersecurity | New York | NY | 40.7128 | -74.0060 | 5 | 2015 | Private | 1000 |
| Yahoo | Jerry Yang | Taiwan | TW | Internet | Software/SaaS | Sunnyvale | CA | 37.3688 | -122.0363 | 5 | 1994 | Acquired | 8000 |
| Houzz | Adi Tatarko | Israel | IL | E-commerce/Home | E-commerce | Palo Alto | CA | 37.4419 | -122.1430 | 4 | 2009 | Private | 1500 |
| AppDynamics | Jyoti Bansal | India | IN | Enterprise SW | Software/SaaS | San Francisco | CA | 37.7749 | -122.4194 | 3.7 | 2008 | Acquired | 2000 |
| Coursera | Daphne Koller | Israel | IL | EdTech | Software/SaaS | Mountain View | CA | 37.3861 | -122.0839 | 2.5 | 2012 | Public | 1200 |
| Eightfold.ai | Ashutosh Garg | India | IN | AI/HR Tech | AI/ML | Santa Clara | CA | 37.3541 | -121.9552 | 2.1 | 2016 | Private | 800 |

**Notes:**
- Valuations are approximate: public companies use market cap (fluctuates daily); private companies use last known funding round valuation.
- WhatsApp valued at acquisition price ($19B by Meta, 2014).
- Slack valued at acquisition price ($27.7B by Salesforce, 2021).
- Employee counts are estimates from LinkedIn, company filings, and news reports.

---

## TABLE 7: Industry Treemap Data

**Visualization type:** Treemap (size = number of companies, color intensity = total valuation)
**Source:** Estimated from NFAP 2022 dataset, manually classified

| industry_sector | num_companies_est | pct_of_319 | total_valuation_est_billions | avg_valuation_billions | top_origin_countries | flagship_company |
|----------------|-------------------|-----------|------------------------------|----------------------|---------------------|------------------|
| Software/SaaS/Cloud | 112 | 35.1 | 400 | 3.6 | India, Israel, Canada | Slack, Freshworks |
| AI/Machine Learning | 48 | 15.0 | 600 | 12.5 | India, China, UK, Russia | Google, Databricks |
| Fintech/Payments | 38 | 11.9 | 350 | 9.2 | Ireland, India, Germany | Stripe, PayPal |
| Healthcare/Biotech | 32 | 10.0 | 100 | 3.1 | France, Lebanon, India | Moderna |
| Cybersecurity | 26 | 8.2 | 200 | 7.7 | Israel, Russia | Palo Alto Networks, Wiz |
| E-commerce/Marketplace | 22 | 6.9 | 120 | 5.5 | Iran, China, India | eBay, DoorDash |
| Hardware/Semiconductors | 16 | 5.0 | 3200 | 200.0 | Taiwan, China, Israel | NVIDIA, Marvell |
| Space/Defense Tech | 10 | 3.1 | 650 | 65.0 | South Africa, Israel, Germany | SpaceX, Palantir |
| Other (Media, Food, Logistics) | 15 | 4.7 | 50 | 3.3 | Various | Vice Media |

**Notes:**
- Hardware/Semiconductors has disproportionately high total valuation due to NVIDIA ($3T+) and average valuation is skewed.
- Space/Defense has disproportionately high valuation due to SpaceX (~$350B) and Palantir (~$250B).
- AI/ML is the fastest-growing category: 65% of Forbes AI 50 founded by immigrants (NFAP 2023).
- These are ESTIMATED sector shares. NFAP does not publish an official industry breakdown.

---

## TABLE 8: AIC Fortune 500 by Industry (Grouped Bar Chart Data)

**Visualization type:** Grouped bar chart (immigrant-founded vs total by industry)
**Source:** AIC Fortune 500 2025 Report

| industry_sector | total_fortune_500_in_sector | immigrant_founded_count | pct_founded_by_immigrants_or_children |
|----------------|---------------------------|------------------------|--------------------------------------|
| Professional & Other Services | 10 | 8 | 80.0 |
| Manufacturing | 61 | 40 | 65.6 |
| Information | 40 | 23 | 57.5 |
| Entertainment, Accommodations & Food | 20 | 11 | 55.0 |
| Retail | 36 | 19 | 52.8 |
| Finance/Insurance | 80 | 36 | 45.0 |
| Healthcare | 45 | 18 | 40.0 |
| Transportation | 30 | 11 | 36.7 |
| Energy | 40 | 14 | 35.0 |
| Other | 138 | 51 | 37.0 |

**Notes:**
- "Founded by immigrants or children" includes both first-generation immigrants and their children of immigrants. This is a broader definition than the NFAP dataset.
- Professional Services (80%), Manufacturing (65.6%), Information (57.5%), Entertainment (55%), and Retail (52.8%) figures are directly from the AIC 2025 report.
- Finance, Healthcare, Transportation, Energy, and Other are estimated from partial AIC data and should be displayed with lower visual confidence.
- Total: 231 of 500 (46.2%) = $8.6 trillion in FY2024 revenue.

---

## TABLE 9: University Network Graph Data

**Visualization type:** Network graph (nodes = universities + companies, edges = founder connections)
**Source:** NFAP 2022, PitchBook, public biographical data

### Node List (Universities)

| node_id | node_type | label | lat | lng | total_funded_founders | notable_stat |
|---------|-----------|-------|-----|-----|-----------------------|-------------|
| stanford | university | Stanford University | 37.4275 | -122.1697 | 3710 | $166B raised by grad alumni |
| mit | university | MIT | 42.3601 | -71.0942 | 2459 | Dominant in biotech, AI |
| harvard | university | Harvard University | 42.3770 | -71.1167 | 3222 | $173.5B raised by grad alumni |
| berkeley | university | UC Berkeley | 37.8719 | -122.2585 | 1500 | Rising in recent rankings |
| upenn | university | UPenn / Wharton | 39.9522 | -75.1932 | 1200 | Strong MBA pipeline |
| cmu | university | Carnegie Mellon | 40.4433 | -79.9436 | 800 | AI/Robotics focus |
| columbia | university | Columbia University | 40.8075 | -73.9626 | 700 | NYC ecosystem |
| uiuc | university | University of Illinois | 40.1020 | -88.2272 | 500 | Enterprise SW, AI |
| gatech | university | Georgia Tech | 33.7756 | -84.3963 | 400 | Engineering focus |
| iit_system | university | IIT System (India) | 28.5456 | 77.1926 | N/A | Major feeder to US grad programs |
| purdue | university | Purdue University | 40.4237 | -86.9212 | 400 | Engineering pipeline |

### Edge List (University-to-Company connections via immigrant founders)

| source_node | target_node | founder_name | origin_country | relationship |
|------------|------------|-------------|---------------|-------------|
| stanford | google | Sergey Brin | Russia | PhD student |
| stanford | yahoo | Jerry Yang | Taiwan | PhD student |
| stanford | nvidia | Jensen Huang | Taiwan | MS student |
| mit | moderna | Noubar Afeyan | Lebanon | PhD student |
| mit | dropbox | (MIT ecosystem) | -- | Ecosystem connection |
| harvard | cloudflare | Michelle Zatlyn | Canada | MBA (HBS) |
| upenn | spacex | Elon Musk | South Africa | BS Physics, Wharton |
| cmu | duolingo | Various | Various | AI/NLP research |
| iit_system | mercor | Varun Vummadi | India | IIT Kharagpur undergrad |
| iit_system | google_ceo | Sundar Pichai | India | IIT Kharagpur undergrad |
| purdue | aviatrix | Sherry Wei | China | PhD EE |
| berkeley | samsara | Various | Various | IoT/hardware |
| stanford | coursera | Daphne Koller | Israel | Professor |

**Key Statistics (from NFAP 2022):**
- 25% of billion-dollar startups have a founder who attended a U.S. university as an international student
- 143 of 582 billion-dollar companies founded by former international students
- >75% of VC-backed immigrant entrepreneurs obtained post-secondary education in the U.S.
- ~40% of US-educated immigrant founders start a company in the state of their alma mater

**Caveat:** University-specific immigrant founder percentages are not systematically available. The edge list above contains only well-documented connections and is not comprehensive.

---

## TABLE 10: Visa Pathway Data (Pie Chart / Bar Chart)

**Visualization type:** Pie chart or horizontal bar chart
**Source:** CSET Georgetown (2019 AI study), NFAP 2022, NFAP 2025

### IMPORTANT CAVEAT FOR VISUALIZATION

These percentages come from **small-sample studies with survivorship bias**. They describe only successful founders and may not represent the broader immigrant founder population. Individual visa pathway data is NOT systematically available. Display these figures with explicit uncertainty indicators (e.g., error bars, footnotes, or a prominent caveat label).

### Aggregate Entry Pathway Estimates (AI Sector -- CSET Georgetown)

| pathway | pct_est | description | source | sample_context |
|---------|---------|-------------|--------|----------------|
| F-1 (Student Visa) | 72 | Most common initial pathway for AI founders | CSET Georgetown 2019 | Forbes AI 50 founders only |
| H-1B (Work Visa) | 15 | Specialty occupation; highly restrictive | NFAP aggregate | General estimate |
| Family/Other | 5 | Family reunification or other categories | Estimate | Not from specific study |
| O-1 (Extraordinary Ability) | 3 | For individuals with extraordinary ability | Estimate | Not from specific study |
| EB-1 (Employment Green Card) | 3 | Direct permanent residency path | Estimate | Not from specific study |
| L-1 (Intracompany Transfer) | 2 | Intracompany transferee | Estimate | Not from specific study |

### System-Level Visa Statistics (Context)

| metric | value | source |
|--------|-------|--------|
| H-1B annual cap | 85,000 | USCIS statutory |
| H-1B FY2025 registrations | 442,000 | USCIS |
| H-1B new application approval rate | ~20% | NFAP 2025 |
| Unicorn founders who came as international students | 22-25% | NFAP 2022 |
| Billion-dollar cos founded by former intl students | 143 of 582 | NFAP 2022 |

**Notes:**
- The 72% F-1 figure is specifically from CSET's study of Forbes AI 50 founders (2019). It should NOT be generalized to all immigrant founders.
- Only the NFAP unicorn statistics (22-25% international students, 143 of 582) and H-1B system statistics are from larger samples.
- Categories labeled "Estimate" are rough approximations to complete the pie chart; they are not from specific studies.

---

## TABLE 11: Time Series -- Growth of Immigrant-Founded Unicorns

**Visualization type:** Line chart or area chart (year on x-axis)
**Source:** NFAP reports (2016, 2018, 2022)

| year | total_us_unicorns | immigrant_founded | pct_immigrant | data_quality | source |
|------|-------------------|-------------------|---------------|-------------|--------|
| 2016 | 44 | 23 | 51 | High (NFAP report) | NFAP 2016 |
| 2018 | 91 | 50 | 55 | High (NFAP report) | NFAP 2018 |
| 2022 | 582 | 319 | 55 | High (NFAP report) | NFAP 2022 |

*Note: Only 2016, 2018, and 2022 have direct NFAP data points. Do NOT interpolate or extrapolate beyond these years without marking estimated points differently. The previous version of this file included interpolated 2019, 2020, 2021, and 2024 data points; those have been removed as they were not based on actual NFAP counts.*

---

## TABLE 12: AI Sector Deep Dive

**Visualization type:** Donut chart or stacked bar for immigrant vs. non-immigrant AI founders

### AI Company Immigrant Founder Rates (Multiple Studies)

| year | study | total_companies | us_based | immigrant_founded | pct_immigrant |
|------|-------|-----------------|----------|-------------------|---------------|
| 2019 | Forbes AI 50 (CSET) | 50 | 50 | 33 | 66 |
| 2023 | Forbes AI 50 (NFAP) | 50 | 43 | 28 | 65 |
| 2025 | Forbes AI (IFP) | 50 | 42 | 25 | 60 |

### AI Founder Country of Origin (IFP 2025 -- Forbes AI List)

| origin_country | num_ai_founders | notes |
|---------------|-----------------|-------|
| India | 9 | Largest group |
| China | 8 | Second largest |
| France | 3 | |
| Australia | 2 | |
| UK | 2 | |
| Canada | 2 | |
| Israel | 2 | |
| Romania | 2 | |
| Chile | 2 | |
| Other (14 countries) | 14 | 1 founder each |

**Source:** [IFP: Most Top AI Companies Founded by Immigrants](https://ifp.org/most-of-americas-top-ai-companies-were-founded-by-immigrants/)

---

## TABLE 13: Country of Origin Coordinates (Full Reference Table)

**Visualization type:** Reference table for geo-encoding all origin countries
**Purpose:** Provides lat/lng for every country in the dataset for use in arc maps, choropleth rendering, and tooltips

| country_code | country_name | lat | lng | num_companies | display_label |
|-------------|-------------|-----|-----|---------------|---------------|
| IN | India | 20.5937 | 78.9629 | 66 | India (66) |
| IL | Israel | 31.0461 | 34.8516 | 54 | Israel (54) |
| GB | United Kingdom | 55.3781 | -3.4360 | 27 | UK (27) |
| CA | Canada | 56.1304 | -106.3468 | 22 | Canada (22) |
| CN | China | 35.8617 | 104.1954 | 21 | China (21) |
| FR | France | 46.2276 | 2.2137 | 18 | France (18) |
| DE | Germany | 51.1657 | 10.4515 | 15 | Germany (15) |
| RU | Russia | 61.5240 | 105.3188 | 11 | Russia (11) |
| UA | Ukraine | 48.3794 | 31.1656 | 10 | Ukraine (10) |
| IR | Iran | 32.4279 | 53.6880 | 8 | Iran (8) |
| AU | Australia | -25.2744 | 133.7751 | 7 | Australia (7) |
| RO | Romania | 45.9432 | 24.9668 | 6 | Romania (6) |
| IT | Italy | 41.8719 | 12.5674 | 6 | Italy (6) |
| PL | Poland | 51.9194 | 19.1451 | 6 | Poland (6) |
| NG | Nigeria | 9.0820 | 8.6753 | 6 | Nigeria (6) |
| KR | South Korea | 35.9078 | 127.7669 | 5 | S. Korea (5) |
| NZ | New Zealand | -40.9006 | 174.8860 | 5 | New Zealand (5) |
| PK | Pakistan | 30.3753 | 69.3451 | 5 | Pakistan (5) |
| AR | Argentina | -38.4161 | -63.6167 | 5 | Argentina (5) |
| BR | Brazil | -14.2350 | -51.9253 | 5 | Brazil (5) |
| TW | Taiwan | 23.6978 | 120.9605 | 5 | Taiwan (5) |
| ES | Spain | 40.4637 | -3.7492 | 4 | Spain (4) |
| PT | Portugal | 39.3999 | -8.2245 | 4 | Portugal (4) |
| DK | Denmark | 56.2639 | 9.5018 | 4 | Denmark (4) |
| IE | Ireland | 53.1424 | -7.6921 | 3 | Ireland (3) |
| ZA | South Africa | -30.5595 | 22.9375 | 3 | S. Africa (3) |
| LB | Lebanon | 33.8547 | 35.8623 | 2 | Lebanon (2) |
| SE | Sweden | 60.1282 | 18.6435 | 2 | Sweden (2) |
| TR | Turkey | 38.9637 | 35.2433 | 2 | Turkey (2) |
| SG | Singapore | 1.3521 | 103.8198 | 2 | Singapore (2) |

---

## TABLE 14: U.S. Destination Coordinates (Full Reference Table)

**Visualization type:** Reference table for plotting U.S. destination points

| city | state | state_code | lat | lng | role_in_ecosystem |
|------|-------|-----------|-----|-----|-------------------|
| San Francisco | California | CA | 37.7749 | -122.4194 | Primary tech hub: Fintech, AI, SaaS |
| San Jose / Silicon Valley | California | CA | 37.3382 | -121.8863 | Primary tech hub: Semiconductors, Enterprise SW |
| Mountain View | California | CA | 37.3861 | -122.0839 | Google/Alphabet HQ area |
| Palo Alto | California | CA | 37.4419 | -122.1430 | VC and startup cluster |
| Santa Clara | California | CA | 37.3541 | -121.9552 | NVIDIA, Palo Alto Networks HQ |
| South San Francisco | California | CA | 37.6547 | -122.4077 | Stripe HQ, biotech |
| San Mateo | California | CA | 37.5630 | -122.3255 | Freshworks HQ |
| Sunnyvale | California | CA | 37.3688 | -122.0363 | Yahoo legacy, enterprise |
| Menlo Park | California | CA | 37.4530 | -122.1817 | Meta/VC cluster |
| New York City | New York | NY | 40.7128 | -74.0060 | Fintech, Media, Cybersecurity |
| Brooklyn | New York | NY | 40.6782 | -73.9442 | Media, emerging tech |
| Boston | Massachusetts | MA | 42.3601 | -71.0589 | Biotech, AI, EdTech |
| Cambridge | Massachusetts | MA | 42.3736 | -71.1097 | MIT/Harvard ecosystem, Moderna HQ |
| Seattle | Washington | WA | 47.6062 | -122.3321 | Cloud, AI, Amazon/Microsoft ecosystem |
| Austin | Texas | TX | 30.2672 | -97.7431 | Tesla HQ, emerging tech hub |
| Starbase | Texas | TX | 25.9975 | -97.1560 | SpaceX HQ |
| Houston | Texas | TX | 29.7604 | -95.3698 | Energy tech, HighRadius |
| Chicago | Illinois | IL | 41.8781 | -87.6298 | Enterprise SW, Fintech |
| Miami | Florida | FL | 25.7617 | -80.1918 | Emerging: Fintech, Crypto |
| Washington DC | DC | DC | 38.9072 | -77.0369 | Defense Tech, Cybersecurity |
| Denver | Colorado | CO | 39.7392 | -104.9903 | Palantir HQ, Data Analytics |
| Wilmington | Delaware | DE | 39.7459 | -75.5466 | Marvell Technology HQ |
| Los Angeles | California | CA | 34.0522 | -118.2437 | Media, Entertainment, AI |

---

## SUMMARY STATISTICS (Dashboard KPIs)

**Visualization type:** Top-level KPI cards in scrollytelling dashboard

| metric | value | source | confidence |
|--------|-------|--------|-----------|
| Total US unicorns (2022) | 582 | NFAP 2022 | High |
| Immigrant-founded unicorns | 319 | NFAP 2022 | High |
| Pct immigrant-founded | 55% | NFAP 2022 | High |
| Countries of origin | 57 | NFAP 2022 | High |
| Collective value (2022) | $1.2 trillion | NFAP 2022 | High |
| Fortune 500 immigrant-founded | 231 of 500 (46.2%) | AIC 2025 | High |
| Fortune 500 revenue (FY2024) | $8.6 trillion | AIC 2025 | High |
| Fortune 500 employees | 15.4 million | AIC 2025 | High |
| AI startups with immigrant founder | 60-66% | CSET/NFAP/IFP | High (multiple studies) |
| Most common origin (companies) | India (66) | NFAP 2022 | High |
| Top 4 US unicorns all immigrant-led | SpaceX, Stripe, Instacart, Databricks | NFAP 2022 | High |
| Immigrants as % of US population | ~14-15% | Census | High |
| Unicorns founded by former intl students | 143 of 582 (25%) | NFAP 2022 | High |
| Growth: unicorns 2018 to 2022 | 500%+ increase (50 to 319) | NFAP | High |
| Pct arrived on student visa (AI only) | ~72% | CSET Georgetown | Low (small sample, AI only) |
| H-1B annual cap | 85,000 | USCIS | High (statutory) |
| H-1B approval rate | ~20% | NFAP 2025 | High |

---

## DATA QUALITY LEGEND

For use in visualization tooltips and footnotes:

| confidence_level | description | visual_encoding_suggestion |
|-----------------|-------------|---------------------------|
| High | Direct from NFAP/AIC primary reports with documented methodology | Solid colors, full opacity |
| Medium | Derived from primary data via calculation or cross-referencing | Slightly reduced opacity, dashed borders |
| Low | Small-sample estimates, survivorship bias, or rough approximations | Low opacity, dotted borders, explicit "estimated" label |
| Estimated | Not from a specific study; gap-filled for visualization completeness | Hatched fill pattern, footnote marker |
