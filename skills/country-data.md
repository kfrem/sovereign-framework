# /country-data — Country-Specific Economic & Regulatory Intelligence

## Purpose
Produce a comprehensive country profile for any nation — economic indicators, business environment, regulatory requirements, market structure, cultural context, and practical operating intelligence. Replaces the need for country-specific data files by generating current, verified intelligence on demand for any country.

## Trigger
User says: /country-data [country name]
Also triggered automatically by `/solve` when a country is identified.

## Input Required
Country name. That's it. Examples:
- "Ghana"
- "Nigeria"
- "Kenya"
- "Rwanda"
- "Senegal"

## Skill Procedure

### STEP 1 — Macro-Economic Profile
Retrieve current data using `/data-verify` protocols:

```
COUNTRY ECONOMIC PROFILE: [COUNTRY]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Data Date: [Today]

POPULATION & GEOGRAPHY
┌──────────────────────────────────────────────────────┐
│ Total population:            [Source] [Year] [RATING]│
│ Population growth rate:      [Source] [Year] [RATING]│
│ Urban population %:          [Source] [Year] [RATING]│
│ Working age population %:    [Source] [Year] [RATING]│
│ Youth (15-24) population:    [Source] [Year] [RATING]│
│ Major cities and population:                         │
│   1.                                                 │
│   2.                                                 │
│   3.                                                 │
│ Administrative structure:                            │
│   (regions, districts, etc.)                         │
└──────────────────────────────────────────────────────┘

GDP & GROWTH
┌──────────────────────────────────────────────────────┐
│ GDP (current US$):           [Source] [Year] [RATING]│
│ GDP per capita:              [Source] [Year] [RATING]│
│ GDP growth rate:             [Source] [Year] [RATING]│
│ Sector breakdown:                                    │
│   Agriculture:     %         [Source] [Year]         │
│   Industry:        %         [Source] [Year]         │
│   Services:        %         [Source] [Year]         │
│ Informal economy estimate:   %                       │
└──────────────────────────────────────────────────────┘

EMPLOYMENT
┌──────────────────────────────────────────────────────┐
│ Unemployment rate:           [Source] [Year] [RATING]│
│ Youth unemployment:          [Source] [Year] [RATING]│
│ Female unemployment:         [Source] [Year] [RATING]│
│ Employment by sector:                                │
│   Agriculture:     %                                 │
│   Industry:        %                                 │
│   Services:        %                                 │
│ Vulnerable employment:       %                       │
│ Minimum wage:                [local currency]        │
│ Average wage (formal sector):[local currency]        │
└──────────────────────────────────────────────────────┘

MONETARY & FISCAL
┌──────────────────────────────────────────────────────┐
│ Currency:                    [Code]                   │
│ Exchange rate (today):       [vs USD]    [Source]     │
│ Inflation rate:              [Source] [Year] [RATING]│
│ Central bank policy rate:    %           [Source]     │
│ Commercial lending rate:     %           [Source]     │
│ Government debt (% GDP):    [Source] [Year] [RATING] │
│ Government revenue (% GDP): [Source] [Year]          │
│ Government expenditure (% GDP): [Source] [Year]      │
│ Tax revenue (% GDP):        [Source] [Year]          │
└──────────────────────────────────────────────────────┘

TRADE
┌──────────────────────────────────────────────────────┐
│ Top 5 exports:                                       │
│   1.            Value:          Share:    %           │
│   2.            Value:          Share:    %           │
│   3.            Value:          Share:    %           │
│   4.            Value:          Share:    %           │
│   5.            Value:          Share:    %           │
│                                                       │
│ Top 5 imports:                                       │
│   1.            Value:          Share:    %           │
│   2.            Value:          Share:    %           │
│   3.            Value:          Share:    %           │
│   4.            Value:          Share:    %           │
│   5.            Value:          Share:    %           │
│                                                       │
│ Trade balance:                                        │
│ FDI inflows:                [Source] [Year]           │
│ Remittances:                [Source] [Year]           │
└──────────────────────────────────────────────────────┘

INFRASTRUCTURE
┌──────────────────────────────────────────────────────┐
│ Access to electricity:       %           [Source]     │
│ Access to electricity (rural): %         [Source]     │
│ Internet users:              %           [Source]     │
│ Mobile subscriptions/100:                [Source]     │
│ Mobile money penetration:    %                       │
│ Road quality index:                                  │
│ Power reliability:                                   │
│   (Hours of outage per month)                        │
└──────────────────────────────────────────────────────┘
```

### STEP 2 — Business Environment Profile

```
BUSINESS ENVIRONMENT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

REGISTRATION & SETUP
┌──────────────────────────────────────────────────────┐
│ Business registration body:                           │
│ Registration cost:                                    │
│ Registration time:          days                      │
│ Online registration available: □ Yes □ No             │
│ Business structures available:                        │
│   □ Sole proprietorship                               │
│   □ Partnership                                       │
│   □ Limited liability company                         │
│   □ Cooperative                                       │
│   □ NGO / Social enterprise                           │
│ Foreign ownership rules:                              │
│ Minimum capital requirements:                         │
└──────────────────────────────────────────────────────┘

TAX SYSTEM
┌──────────────────────────────────────────────────────┐
│ Tax authority:                   Website:              │
│ Corporate tax rate:              %                    │
│ Personal income tax (top rate):  %                    │
│ VAT rate:                        %                    │
│ VAT threshold:                   [local currency]     │
│ Withholding tax:                 %                    │
│ Social security (employer):      %                    │
│ Social security (employee):      %                    │
│ Capital gains tax:               %                    │
│ Tax incentives available:                             │
│   □ Free zone / export processing zone               │
│   □ Agricultural sector exemptions                   │
│   □ Youth enterprise incentives                      │
│   □ Regional/rural incentives                        │
│   □ Technology / innovation incentives               │
│ Filing deadlines:                                     │
│ Payment methods:                                      │
└──────────────────────────────────────────────────────┘

FINANCIAL SERVICES
┌──────────────────────────────────────────────────────┐
│ Major banks:                                          │
│ Microfinance institutions:                            │
│ Mobile money operators:                               │
│   (Operator, market share, merchant setup process)   │
│ Typical SME loan interest rate: %                    │
│ Typical microfinance rate: %                         │
│ Community savings systems:                            │
│   (Name, how it works, typical amounts)              │
│ Credit bureau exists: □ Yes □ No                      │
│ Collateral requirements:                              │
└──────────────────────────────────────────────────────┘

LABOUR LAWS
┌──────────────────────────────────────────────────────┐
│ Minimum wage:                [local currency/period] │
│ Maximum working hours:       per week                │
│ Overtime rules:                                       │
│ Leave entitlement:           days/year               │
│ Maternity leave:             weeks                   │
│ Termination notice:          weeks/months            │
│ Severance requirements:                               │
│ Social security registration: □ Mandatory □ Optional │
│ Employment contract: □ Required □ Recommended         │
│ Foreign worker permits:                               │
└──────────────────────────────────────────────────────┘
```

### STEP 3 — Sector Opportunities

```
KEY ECONOMIC SECTORS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

For each major sector:
┌──────────────────────────────────────────────────────┐
│ SECTOR: [Agriculture / Manufacturing / Services /    │
│          Mining / Technology / etc.]                  │
│                                                       │
│ Contribution to GDP:        %                        │
│ Employment share:           %                        │
│ Growth trend: □ Growing □ Stable □ Declining          │
│ Government priority: □ Yes □ No                       │
│ Key sub-sectors:                                      │
│ Key players:                                          │
│ Import substitution opportunities:                    │
│ Value addition opportunities:                         │
│ Export opportunities:                                  │
│ Government incentives:                                │
│ Main constraints:                                     │
└──────────────────────────────────────────────────────┘
```

### STEP 4 — Cultural & Practical Operating Intelligence

```
OPERATING REALITY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

CULTURAL CONTEXT
┌──────────────────────────────────────────────────────┐
│ Major languages:                                      │
│ Business language:                                    │
│ Religious calendar considerations:                    │
│ Market days / trading patterns:                       │
│ Traditional authority structure:                      │
│ Gender dynamics in business:                          │
│ Age/seniority in business relationships:              │
│ Gift-giving / hospitality norms:                      │
│ Negotiation style:                                    │
│ Payment culture (prompt vs delayed):                  │
└──────────────────────────────────────────────────────┘

PRACTICAL CONSIDERATIONS
┌──────────────────────────────────────────────────────┐
│ Power supply reliability:                             │
│   Average outage hours/month:                        │
│   Generator/solar needed: □ Yes □ No                  │
│   Generator fuel cost/month:                         │
│ Water supply:                                         │
│ Internet reliability:                                 │
│   Best providers:                                     │
│   Data cost (1GB):                                    │
│ Transport:                                            │
│   Major routes:                                       │
│   Transport costs:                                    │
│   Road conditions:                                    │
│ Security:                                             │
│   General assessment:                                 │
│   Business-specific risks:                            │
│ Corruption index (Transparency International):        │
│ Common corruption points for business:                │
│ Climate / weather considerations:                     │
│ Agricultural seasons:                                 │
└──────────────────────────────────────────────────────┘

KEY CONTACTS & RESOURCES
┌──────────────────────────────────────────────────────┐
│ Business registration:        [Name, website, phone] │
│ Tax authority:                [Name, website, phone] │
│ Central bank:                 [Name, website]        │
│ Statistics office:            [Name, website]        │
│ Investment promotion agency:  [Name, website]        │
│ Chamber of commerce:          [Name, website]        │
│ SME support agency:           [Name, website]        │
│ Cooperative department:       [Name, website]        │
│ Environmental agency:         [Name, website]        │
│ Standards authority:          [Name, website]        │
└──────────────────────────────────────────────────────┘
```

## Data Sources
Use `/data-verify` APIs:
- World Bank API for macro indicators
- IMF DataMapper for fiscal/monetary data
- WebSearch for current regulatory information
- Country-specific official sources listed in `/data-verify`

## Output Format
Deliver a complete country intelligence brief. Use current verified data with source citations and freshness ratings. Mark any data requiring verification with [VERIFY].

## Connects To
- `/data-verify` — data sourcing and verification
- `/solve` — country context feeds into every solution
- `/legal-setup` — registration and regulatory detail
- `/financial-model` — tax rates, exchange rates, inflation feed into projections
- `/opportunity-scan` — sector data identifies opportunities
- `/stakeholder-map` — cultural context informs stakeholder engagement
