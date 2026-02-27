# /data-sources — MASTER DATA REGISTRY
## THE SOVEREIGN FRAMEWORK™ | Official Sources and Free API Reference

**Purpose:** This registry is the single reference for all data verification across every SOVEREIGN Framework skill. Before using any figure in a government proposal, financial model, pitch, investment document, or implementation plan — consult this registry for the correct source.

**Access requirement:** All sources below are free to access unless marked 💰. No API key is required for World Bank, IMF, or FAO unless marked 🔑.

---

## SECTION 1 — THE BIG FIVE: HIGHEST-PRIORITY FREE GLOBAL APIs

These five sources cover 80% of all data needs across SOVEREIGN Framework deliverables.

---

### 1.1 WORLD BANK OPEN DATA API
**Access:** Free. No API key required.
**Base URL:** `https://api.worldbank.org/v2/`
**Format:** Add `?format=json&mrv=3` to get the 3 most recent values in JSON

**Query pattern:**
```
https://api.worldbank.org/v2/country/[ISO3]/indicator/[INDICATOR_CODE]?format=json&mrv=3
```

**ISO3 codes for key countries:**
| Country | ISO3 | Country | ISO3 |
|---|---|---|---|
| Ghana | GHA | Rwanda | RWA |
| Nigeria | NGA | Senegal | SEN |
| Kenya | KEN | Cameroon | CMR |
| South Africa | ZAF | Zambia | ZMB |
| Ethiopia | ETH | Zimbabwe | ZWE |
| Tanzania | TZA | Côte d'Ivoire | CIV |
| Uganda | UGA | Mozambique | MOZ |
| Malawi | MWI | Angola | AGO |

**Key Indicators — Economic:**
| Indicator | Code | API URL |
|---|---|---|
| GDP (current US$) | NY.GDP.MKTP.CD | `https://api.worldbank.org/v2/country/GHA/indicator/NY.GDP.MKTP.CD?format=json&mrv=3` |
| GDP per capita (current US$) | NY.GDP.PCAP.CD | `...NY.GDP.PCAP.CD?format=json&mrv=3` |
| GDP growth rate (annual %) | NY.GDP.MKTP.KD.ZG | `...NY.GDP.MKTP.KD.ZG?format=json&mrv=3` |
| GNI per capita (Atlas method) | NY.GNP.PCAP.CD | `...NY.GNP.PCAP.CD?format=json&mrv=3` |
| Inflation, consumer prices (annual %) | FP.CPI.TOTL.ZG | `...FP.CPI.TOTL.ZG?format=json&mrv=3` |
| Foreign direct investment, net inflows | BX.KLT.DINV.CD.WD | `...BX.KLT.DINV.CD.WD?format=json&mrv=3` |
| Trade (% of GDP) | NE.TRD.GNFS.ZS | `...NE.TRD.GNFS.ZS?format=json&mrv=3` |
| Tax revenue (% of GDP) | GC.TAX.TOTL.GD.ZS | `...GC.TAX.TOTL.GD.ZS?format=json&mrv=3` |
| Government expenditure (% of GDP) | GC.XPN.TOTL.GD.ZS | `...GC.XPN.TOTL.GD.ZS?format=json&mrv=3` |
| Exchange rate (LCU per US$) | PA.NUS.FCRF | `...PA.NUS.FCRF?format=json&mrv=3` |
| Personal remittances received (US$) | BX.TRF.PWKR.CD.DT | `...BX.TRF.PWKR.CD.DT?format=json&mrv=3` |

**Key Indicators — Labour and Employment:**
| Indicator | Code |
|---|---|
| Unemployment, total (% of labour force) | SL.UEM.TOTL.ZS |
| Unemployment, youth (% ages 15–24) | SL.UEM.1524.ZS |
| Unemployment, female (% of female labour force) | SL.UEM.TOTL.FE.ZS |
| Labour force participation rate, total | SL.TLF.ACTI.ZS |
| Labour force participation rate, female | SL.TLF.ACTI.FE.ZS |
| Employment in agriculture (% of total employment) | SL.AGR.EMPL.ZS |
| Employment in industry (% of total employment) | SL.IND.EMPL.ZS |
| Employment in services (% of total employment) | SL.SRV.EMPL.ZS |
| Vulnerable employment (% of total employment) | SL.EMP.VULN.ZS |

**Key Indicators — Population and Demographics:**
| Indicator | Code |
|---|---|
| Population, total | SP.POP.TOTL |
| Population growth (annual %) | SP.POP.GROW |
| Population, ages 15–64 (working age %) | SP.POP.1564.TO.ZS |
| Population, ages 0–14 (% of total) | SP.POP.0014.TO.ZS |
| Urban population (% of total) | SP.URB.TOTL.IN.ZS |
| Rural population (% of total) | SP.RUR.TOTL.ZS |

**Key Indicators — Social and Infrastructure:**
| Indicator | Code |
|---|---|
| Mobile cellular subscriptions (per 100 people) | IT.CEL.SETS.P2 |
| Individuals using the Internet (% of population) | IT.NET.USER.ZS |
| Access to electricity (% of population) | EG.ELC.ACCS.ZS |
| Access to electricity, rural (%) | EG.ELC.ACCS.RU.ZS |
| People using safely managed drinking water | SH.H2O.SMDW.ZS |
| Hospital beds (per 1,000 people) | SH.MED.BEDS.ZS |
| Government health expenditure (% of GDP) | SH.XPD.CHEX.GD.ZS |
| Primary school enrollment (% gross) | SE.PRM.ENRR |
| Tertiary enrollment (% gross) | SE.TER.ENRR |
| Government education expenditure (% of GDP) | SE.XPD.TOTL.GD.ZS |

**Key Indicators — Agriculture:**
| Indicator | Code |
|---|---|
| Agricultural land (% of land area) | AG.LND.AGRI.ZS |
| Arable land (% of land area) | AG.LND.ARBL.ZS |
| Agriculture value added (% of GDP) | NV.AGR.TOTL.ZS |
| Food production index | AG.PRD.FOOD.XD |
| Cereal yield (kg per hectare) | AG.YLD.CREL.KG |

---

### 1.2 IMF DATAMAPPER API
**Access:** Free. No API key required.
**Base URL:** `https://www.imf.org/external/datamapper/api/v1/`

**Key queries:**
```
https://www.imf.org/external/datamapper/api/v1/NGDP_RPCH/[ISO2_COUNTRY_CODE]
```

**Common indicators:**
| Indicator | Code |
|---|---|
| Real GDP growth | NGDP_RPCH |
| Inflation (average consumer prices) | PCPIPCH |
| Unemployment rate | LUR |
| Current account balance (% of GDP) | BCA_NGDPD |
| General government net lending/borrowing (% GDP) | GGXCNL_NGDP |
| General government gross debt (% GDP) | GGXWDG_NGDP |

**World Economic Outlook data (annual release — April and October):**
`https://www.imf.org/en/Publications/WEO`

---

### 1.3 FAO (Food and Agriculture Organization) — FAOSTAT
**Access:** Free. No API key required.
**Portal:** `https://www.fao.org/faostat/en/`
**API base:** `https://fenixservices.fao.org/faostat/api/v1/en/data/`

**Key datasets:**
| Dataset | Code | What It Contains |
|---|---|---|
| Production — Crops and livestock | QCL | Commodity production volumes by country |
| Trade — Crops and livestock | TCL | Import/export volumes and values |
| Food Balance Sheets | FBS | Food supply per capita |
| Prices — Producer Prices | PP | Farm-gate prices by commodity and country |
| Employment (agriculture) | OEA | Agricultural employment statistics |
| Land use | RL | Agricultural land area by type |

**Quick access by commodity:**
`https://fenixservices.fao.org/faostat/api/v1/en/data/PP?area=59&item=27&element=5532&year=2022,2023,2024`
*(59 = Ghana, 27 = Wheat, 5532 = Producer Price — adjust as needed)*

**Country codes (FAO FAOSTAT):** Ghana = 59, Nigeria = 159, Kenya = 114, Ethiopia = 238, Tanzania = 215, South Africa = 202, Uganda = 226

---

### 1.4 UN COMTRADE — IMPORT/EXPORT DATA
**Access:** 250 free API calls/month (no key required for basic). Register for 500 calls/month (free).
**Portal:** `https://comtradeplus.un.org/`
**API:** `https://comtradeplus.un.org/TradeFlow`

**What it gives you:** Import/export volumes and values by commodity and country — essential for import substitution analysis, export market sizing, and trade gap identification.

**Key use in SOVEREIGN Framework:** Identifies what a country is importing that could be produced domestically (opportunity scan) and confirms export market value for community enterprise and agribusiness proposals.

**Note:** For single-country general trade summaries, the World Bank Trade (% of GDP) indicator is often sufficient. Use Comtrade for specific commodity-level detail.

---

### 1.5 AFRICAN DEVELOPMENT BANK — OPEN DATA
**Access:** Free. No API key required.
**Portal:** `https://dataportal.opendataforafrica.org/`
**Direct API:** `https://api.opendataforafrica.org/`

**Key datasets:**
- African Economic Outlook — country-by-country economic projections
- African Development Fund programme data
- Infrastructure investment data by country
- Gender and social statistics

**Also useful:** AfDB Country Strategy Papers (CSPs) — available on the AfDB website for every active programme country. These contain the most current government priorities and budget allocations for each country, updated every 3–5 years.

---

## SECTION 2 — COUNTRY-SPECIFIC OFFICIAL SOURCES

For government proposals and client pitches, always prefer the country's own official statistics over international estimates. Ministers know their own data.

---

### GHANA

| Source | Data | URL |
|---|---|---|
| **Ghana Statistical Service (GSS)** | Population, employment, poverty, business census | `https://statsghana.gov.gh` |
| **Bank of Ghana** | Exchange rate (daily), lending rates, mobile money, monetary policy | `https://bog.gov.gh` |
| **Ministry of Finance** | Budget statements, MTEF, public accounts | `https://mofep.gov.gh` |
| **Ghana Revenue Authority (GRA)** | Tax rates, VAT, corporate tax, registration requirements | `https://gra.gov.gh` |
| **National Development Planning Commission (NDPC)** | Development plans, district growth data | `https://ndpc.gov.gh` |
| **Ghana Health Service** | Health statistics, facility data, workforce | `https://ghshealthservice.org` |
| **Ghana Education Service** | School enrollment, teacher data, district education | `https://ges.gov.gh` |
| **COCOBOD** | Cocoa prices, farmer data | `https://cocobod.gh` |
| **EPA Ghana** | Environmental permits, land classification | `https://epa.gov.gh` |
| **Registrar General's Department** | Business registration, cooperative data | `https://rgd.gov.gh` |

**Key documents to search before any Ghana deliverable:**
- Ghana Budget Statement (current year) — Ministry of Finance
- Ghana Statistical Service Labour Force Report (latest)
- Bank of Ghana Monetary Policy Committee statement (latest)

---

### NIGERIA

| Source | Data | URL |
|---|---|---|
| **National Bureau of Statistics (NBS)** | GDP, employment, inflation, trade, business statistics | `https://nigerianstat.gov.ng` |
| **Central Bank of Nigeria (CBN)** | Exchange rate, lending rates, monetary policy | `https://cbn.gov.ng` |
| **Federal Ministry of Finance** | Budget, fiscal policy | `https://finance.gov.ng` |
| **Federal Inland Revenue Service (FIRS)** | Tax rates, VAT, corporate tax | `https://firs.gov.ng` |
| **National Population Commission** | Census data | `https://nationalpopulation.gov.ng` |
| **NAFDAC** | Food and drug regulation, product registration | `https://nafdac.gov.ng` |

---

### KENYA

| Source | Data | URL |
|---|---|---|
| **Kenya National Bureau of Statistics (KNBS)** | Population, employment, GDP, CPI | `https://knbs.or.ke` |
| **Central Bank of Kenya (CBK)** | Exchange rate, lending rates, mobile money | `https://centralbank.go.ke` |
| **National Treasury** | Budget statements, development plans | `https://treasury.go.ke` |
| **Kenya Revenue Authority (KRA)** | Tax rates, VAT, compliance | `https://kra.go.ke` |
| **Kenya National Land Commission** | Land data, registration | `https://landcommission.go.ke` |

---

### SOUTH AFRICA

| Source | Data | URL |
|---|---|---|
| **Stats SA** | All national statistics | `https://statssa.gov.za` |
| **South African Reserve Bank (SARB)** | Exchange rate, monetary policy, financial sector | `https://resbank.co.za` |
| **National Treasury** | Budget, MTEF | `https://treasury.gov.za` |
| **SARS** | Tax rates | `https://sars.gov.za` |

---

### ETHIOPIA

| Source | Data | URL |
|---|---|---|
| **Central Statistical Agency (CSA)** | Population, prices, agriculture | `https://statsethiopia.gov.et` |
| **National Bank of Ethiopia** | Exchange rate, monetary policy | `https://nbe.gov.et` |
| **Ministry of Finance** | Budget | `https://mof.gov.et` |

---

### TANZANIA

| Source | Data | URL |
|---|---|---|
| **National Bureau of Statistics** | All national statistics | `https://nbs.go.tz` |
| **Bank of Tanzania** | Exchange rate, monetary policy | `https://bot.go.tz` |
| **Ministry of Finance** | Budget documents | `https://mof.go.tz` |

---

### UGANDA

| Source | Data | URL |
|---|---|---|
| **Uganda Bureau of Statistics (UBOS)** | All national statistics | `https://ubos.org` |
| **Bank of Uganda** | Exchange rate, monetary policy | `https://bou.or.ug` |
| **Ministry of Finance, Planning and Economic Development** | Budget | `https://finance.go.ug` |

---

## SECTION 3 — COMMODITY AND MARKET PRICE SOURCES

For financial models involving agricultural commodities, construction materials, or energy costs.

| Source | What It Covers | Access |
|---|---|---|
| **World Bank Commodity Price Data (Pink Sheet)** | International commodity prices — cocoa, coffee, gold, oil, maize, etc. | Free: `https://worldbank.org/en/research/commodity-markets` |
| **FAO GIEWS (Food Price Monitoring)** | Domestic food prices in African markets — specific city-level data | Free: `https://www.fao.org/giews/` |
| **Reuters/Bloomberg commodity feeds** | Real-time international commodity prices | Subscription 💰 |
| **COCOBOD (Ghana)** | Ghana cocoa producer price — official, published seasonally | Free: `https://cocobod.gh` |
| **East Africa Exchange (EAX)** | Grain prices in East Africa | `https://eax.rw` |
| **Global Petrol Prices** | Current fuel prices by country | Free: `https://globalpetrolprices.com` — critical for transport cost modelling |

---

## SECTION 4 — DEVELOPMENT PARTNER AND AID FLOW DATA

For market development targeting, pitch context, and competitive landscape analysis.

| Source | What It Covers | Access |
|---|---|---|
| **OCHA Financial Tracking Service (FTS)** | All humanitarian aid and development flows by country and project | Free: `https://fts.unocha.org` |
| **AidData** | Development finance database — who is funding what in which country | Free: `https://aiddata.org` |
| **IATI Registry** | All IATI-registered development project data | Free: `https://iatiregistry.org` |
| **OECD DAC** | Official development assistance statistics | Free: `https://stats.oecd.org` |
| **UNDP Country Offices** | Country-level development programme data | Free: individual country UNDP websites |
| **World Bank Projects** | Active World Bank lending portfolio by country | Free: `https://projects.worldbank.org` |

---

## SECTION 5 — FINANCIAL SECTOR DATA

For financial models, interest rate projections, and loan/credit analysis.

| Data Need | Source |
|---|---|
| Central bank policy rates | Each country's central bank website (see Section 2) |
| Commercial bank lending rates | World Bank: `PA.INT.PREM.NS.ZS` (interest rate spread) |
| Microfinance rates | MIX Market (Microfinance Information Exchange): `https://mixmarket.org` |
| Mobile money transaction data | Bank of Ghana quarterly reports / each country's telco regulator |
| Stock exchange data | African Securities Exchanges Association: `https://www.african-exchanges.org` |
| Credit rating by country | Moody's, S&P (subscription 💰) — Free summaries: `https://tradingeconomics.com` |

---

## SECTION 6 — BUSINESS REGISTRATION AND REGULATORY DATA

For startup cost estimates, compliance requirements, and investment climate analysis.

| Source | What It Covers | Access |
|---|---|---|
| **World Bank Doing Business** | Registration costs, time, procedures by country | Note: Discontinued 2021; use Doing Business historical data with caveat; verify current fees with national registry |
| **World Bank Business Ready (B-READY)** | Successor to Doing Business — new methodology | Free: `https://businessready.worldbank.org` |
| **International Finance Corporation (IFC)** | Investment climate, SME data | Free: `https://ifc.org` |
| **Each country's business registry** | Actual current registration fees (always verify; fees change) | See Section 2 for country-specific links |

---

## SECTION 7 — EXCHANGE RATE SOURCES (CURRENT RATES — CHECK SAME DAY)

For any financial model or pitch document, exchange rates must be checked on the day of production. African currencies fluctuate significantly.

| Country | Official Rate Source | Interbank Rate |
|---|---|---|
| Ghana (GHS) | Bank of Ghana: `bog.gov.gh` — daily forex rates | XE.com, OANDA |
| Nigeria (NGN) | Central Bank of Nigeria: `cbn.gov.ng` — daily rates | XE.com (note: parallel/official rate gap — specify which rate you use) |
| Kenya (KES) | Central Bank of Kenya: `centralbank.go.ke` | XE.com, OANDA |
| South Africa (ZAR) | SARB: `resbank.co.za` | XE.com, Bloomberg |
| Ethiopia (ETB) | National Bank of Ethiopia: `nbe.gov.et` | XE.com |
| Tanzania (TZS) | Bank of Tanzania: `bot.go.tz` | XE.com |
| Uganda (UGX) | Bank of Uganda: `bou.or.ug` | XE.com |
| Multi-country | World Bank annual average: `PA.NUS.FCRF` | Not for same-day use — annual average only |

**⚠️ NIGERIA SPECIFIC WARNING:** Nigeria has operated with multiple exchange rate windows. Always specify whether you are using the official CBN rate or the parallel market rate — and always state the date. These have differed by 30–100% at various points. Use the CBN official window rate for government proposals.

---

## SECTION 8 — QUICK REFERENCE: SKILL → PRIMARY DATA SOURCE

| Skill | Primary Data Needed | First Source to Check |
|---|---|---|
| `/opportunity-scan` | Unemployment, GDP, sector growth, import values | World Bank API + UN Comtrade |
| `/financial-model` | Exchange rate, inflation, tax rates, wages | Central bank (same-day) + World Bank API |
| `/gov-proposal` | Government budget, unemployment, population | National statistical service + Ministry of Finance |
| `/crowd-fund` | GDP per capita, remittances, FDI, mobile money | World Bank API (`BX.TRF.PWKR.CD.DT`) |
| `/business-rescue` | Lending rates, inflation, fuel prices, sector data | Central bank + globalpetrolprices.com |
| `/asset-audit` | Exchange rate, construction costs, property values | Central bank + local quotation |
| `/social-value` | GDP per capita, health/education expenditure | World Bank API + national ministry reports |
| `/human-capital-profile` | Unemployment, wages, enrollment, mobile money | World Bank API + national bureau of statistics |
| `/workforce-engine` | Sector wages, minimum wage, civil service rates | National bureau of statistics + Ministry of Labour |
| `/grad-bridge` | Graduate unemployment, entry-level salaries | WebSearch + national statistical service |
| `/community-enterprise` | Commodity prices, local wages, mobile money | FAO GIEWS + central bank |
| `/idea-engine` | Sector market size, competitor pricing, wages | WebSearch + national bureau of statistics |
| `/pitch` | Ministry budget, unemployment, GDP, population | National statistical service + Ministry of Finance |
| `/proposal-trainer` | Consultancy rates, government payment norms | WebSearch + practitioner consultation |

---

## SECTION 9 — DATA FRESHNESS STANDARD

Apply these standards consistently across all skills:

| Vintage | Rating | Usage Rule |
|---|---|---|
| 2025–2026 | 🟢 | Use freely — no caveat required |
| 2023–2024 | 🟡 | Use with stated source year; apply 10–15% variance buffer in financial models |
| 2021–2022 | 🔴 | Flag prominently; COVID altered most economic indicators; verify before any contract use |
| Pre-2021 | ❌ | Do not use; replace entirely before any deliverable |

**Special cases:**
- **Exchange rates**: Never older than the same business day for financial models; 7-day maximum for narrative documents
- **Commodity prices**: Never older than 30 days for agricultural production proposals; international prices change weekly
- **Government budget figures**: Must be current fiscal year; previous year's budget is 🔴 for any proposal presented to a ministry
- **Population data**: National census data is valid until the next census; use with stated census year

---

## SECTION 10 — WHEN DATA IS NOT AVAILABLE

Apply this five-level hierarchy when official data cannot be found:

| Level | Data Quality | Approach | Disclosure Required |
|---|---|---|---|
| **1** | Official current (2025–2026) | Use directly | State source and year |
| **2** | Official but dated (2023–2024) | Use with variance buffer | State source, year, and buffer applied |
| **3** | Proxy from comparable country | Use if same income level and geography | Disclose proxy methodology |
| **4** | Expert estimate (practitioner consultation) | Use if 3+ practitioners agree | Disclose as "practitioner estimate" |
| **5** | Calculated estimate (stated methodology) | Last resort | Disclose fully as estimate with methodology |

**Never use Level 5 for:** exchange rates, tax rates, government budget figures, or any figure that appears in the financial case of a government proposal or investor document.

---

*This registry is a living document. Update it when:*
- *A new free API source is identified*
- *A country-specific source URL changes*
- *A data source is discontinued (e.g. World Bank Doing Business in 2021)*
- *A new country enters the SOVEREIGN Framework operating geography*

*Last verified: 2026*
