# /supply-chain — Supply Chain & Operations Design

## Purpose
Design end-to-end supply chains and daily operational systems for any enterprise — from a single farmer moving produce to market, to a government ministry managing national commodity flows. Eliminates the chaos of "buy cheap, sell dear" without logistics, storage, quality control or supplier relationships.

## Trigger
User says: /supply-chain [description of what they produce or want to produce]

## What This Skill Solves
- **No structured procurement** — buying inputs at random prices from random sources
- **Post-harvest / post-production losses** — up to 40% of African agricultural output is lost to poor handling, storage and transport
- **No quality control** — inconsistent product quality destroys customer trust and pricing power
- **Transport chaos** — no route planning, no load optimisation, no cost tracking
- **No inventory management** — either stockouts or wasteful oversupply
- **Supplier dependency** — single-source risk with no negotiating leverage
- **No cold chain or preservation** — perishables rot before reaching market
- **Middleman extraction** — value captured by intermediaries, not producers

## Doctrine Alignment
- **Asset-first**: Maps every physical asset (vehicles, storage, equipment, roads) before designing the chain
- **Revenue-before-funding**: Designs chains that work with existing transport and storage before requiring investment
- **Three-population**: Identifies who supplies, who operates, who buys at every node

## Input Required
ONE sentence minimum. Examples:
- "I grow tomatoes in Tamale and sell in Accra"
- "Our cooperative processes shea butter for export"
- "The district wants to set up a school feeding programme using local farms"
- "I buy second-hand clothes in bales and sell in the market"

## Skill Procedure

### STEP 1 — Map the Current Chain (or Design from Zero)
From the user's description, identify or design:

```
SUPPLY CHAIN MAP
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

INPUT SOURCES
┌─────────────────────────────────────────────────────┐
│ What is sourced:                                     │
│ From whom:                                           │
│ Current price / unit:                                │
│ Alternative sources (at least 2):                    │
│ Seasonality / availability pattern:                  │
│ Quality grade available:                             │
│ Payment terms (cash, credit, advance):               │
│ Distance from operation:                             │
│ Reliability score (1-5):                             │
└─────────────────────────────────────────────────────┘

INBOUND LOGISTICS
┌─────────────────────────────────────────────────────┐
│ How inputs arrive:                                   │
│ Transport mode:                                      │
│ Cost per trip / per unit:                            │
│ Time from source to operation:                       │
│ Loss rate during transport:          %               │
│ Who bears transport cost:                            │
│ Storage on arrival (where, capacity, condition):     │
└─────────────────────────────────────────────────────┘

TRANSFORMATION / PROCESSING
┌─────────────────────────────────────────────────────┐
│ What happens to inputs:                              │
│ Equipment / tools used:                              │
│ Labour required (number, skills):                    │
│ Processing time per batch:                           │
│ Output per batch:                                    │
│ Waste / by-product generated:                        │
│ Quality control point:                               │
│ Bottleneck (slowest step):                           │
└─────────────────────────────────────────────────────┘

STORAGE / INVENTORY
┌─────────────────────────────────────────────────────┐
│ Finished goods storage:                              │
│ Capacity (units / kg / litres):                     │
│ Shelf life of product:                               │
│ Current stock level:                                 │
│ Optimal stock level:                                 │
│ Reorder point:                                       │
│ Storage cost per day:                                │
│ Temperature / humidity requirements:                 │
└─────────────────────────────────────────────────────┘

OUTBOUND LOGISTICS
┌─────────────────────────────────────────────────────┐
│ How product reaches customer:                        │
│ Transport mode:                                      │
│ Cost per delivery:                                   │
│ Delivery time:                                       │
│ Loss rate during delivery:           %               │
│ Delivery schedule (daily, weekly, on-demand):        │
│ Return / rejection handling:                         │
└─────────────────────────────────────────────────────┘

CUSTOMER / END MARKET
┌─────────────────────────────────────────────────────┐
│ Who buys:                                            │
│ Where they buy:                                      │
│ How much they buy per period:                        │
│ What price they pay:                                 │
│ Payment terms:                                       │
│ Competing products available:                        │
│ Customer satisfaction issues:                        │
└─────────────────────────────────────────────────────┘
```

### STEP 2 — Loss & Leakage Analysis
Calculate value destroyed at each node:

```
LOSS & LEAKAGE REGISTER
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Node              | Loss Type        | % Lost | Value Lost/Month | Cause              | Fix Available Now?
─────────────────────────────────────────────────────────────────────────────────────────────────────────
Input sourcing    |                  |        |                  |                    |
Inbound transport |                  |        |                  |                    |
Receiving/storage |                  |        |                  |                    |
Processing        |                  |        |                  |                    |
Finished storage  |                  |        |                  |                    |
Outbound delivery |                  |        |                  |                    |
Customer returns  |                  |        |                  |                    |
─────────────────────────────────────────────────────────────────────────────────────────────────────────
TOTAL MONTHLY LOSS|                  |        |                  |                    |
```

**Rule**: Any loss above 5% at any node triggers a mandatory intervention design.

### STEP 3 — Supplier Strategy
Design procurement that eliminates single-source dependency:

```
SUPPLIER MATRIX
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

For each key input:
┌──────────────────────────────────────────────────────┐
│ Input:                                                │
│                                                       │
│ PRIMARY SUPPLIER                                      │
│   Name / location:                                    │
│   Price:              Quality:          Reliability:   │
│   Payment terms:                                      │
│   Share of supply:        %                           │
│                                                       │
│ BACKUP SUPPLIER 1                                     │
│   Name / location:                                    │
│   Price:              Quality:          Reliability:   │
│   Payment terms:                                      │
│   Activation trigger:                                 │
│                                                       │
│ BACKUP SUPPLIER 2                                     │
│   Name / location:                                    │
│   Price:              Quality:          Reliability:   │
│   Payment terms:                                      │
│   Activation trigger:                                 │
│                                                       │
│ NEGOTIATION LEVERAGE:                                 │
│ (What do you offer suppliers that competitors don't?) │
│   □ Guaranteed volume    □ Prompt payment              │
│   □ Collection service   □ Long-term contract          │
│   □ Market information   □ Input financing             │
└──────────────────────────────────────────────────────┘
```

### STEP 4 — Daily Operations Schedule
Produce the actual daily workflow:

```
DAILY OPERATIONS PROTOCOL
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[TIME]    TASK                           WHO           CHECKLIST
──────────────────────────────────────────────────────────────────
05:00     Open facility / inspection      Supervisor    □ Check storage temps
                                                        □ Verify overnight stock
                                                        □ Equipment check
05:30     Receive incoming supplies       Receiving     □ Count / weigh
                                                        □ Quality check
                                                        □ Record in log
                                                        □ Reject sub-standard
06:00     Begin processing / production   Production    □ Follow recipe/spec
                                                        □ Track waste
                                                        □ Mid-process QC
...       [Continue for full day]
17:00     End-of-day reconciliation       Manager       □ Units produced vs target
                                                        □ Inputs used vs budget
                                                        □ Cash reconciliation
                                                        □ Tomorrow's prep list
```

### STEP 5 — Quality Control System
Design quality gates that require NO expensive equipment:

```
QUALITY CONTROL PROTOCOL
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

INCOMING QUALITY (Inputs)
┌──────────────────────────────────────────────────────┐
│ Test 1:           Method:            Pass/Fail:       │
│ Test 2:           Method:            Pass/Fail:       │
│ Rejection protocol: [what happens to failed inputs]   │
│ Record: [date, supplier, batch, result]               │
└──────────────────────────────────────────────────────┘

IN-PROCESS QUALITY
┌──────────────────────────────────────────────────────┐
│ Check point:      Frequency:         Standard:        │
│ Who checks:       Tool needed:       Record method:   │
│ Corrective action if fail:                            │
└──────────────────────────────────────────────────────┘

FINAL PRODUCT QUALITY
┌──────────────────────────────────────────────────────┐
│ Appearance:       Standard:          Check method:    │
│ Weight/volume:    Tolerance:         Check method:    │
│ Packaging:        Standard:          Check method:    │
│ Labelling:        Required info:     Check method:    │
│ Sample retention: [keep 1 from each batch, 30 days]   │
└──────────────────────────────────────────────────────┘

CUSTOMER FEEDBACK LOOP
┌──────────────────────────────────────────────────────┐
│ How feedback is collected:                            │
│ Who reviews:              Frequency:                  │
│ How it feeds back into QC:                            │
│ Complaint resolution process:                         │
│ Target: Zero repeat complaints                        │
└──────────────────────────────────────────────────────┘
```

### STEP 6 — Inventory Management Rules

```
INVENTORY RULES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Item          | Min Stock | Max Stock | Reorder Point | Reorder Qty | Lead Time | Storage Location
──────────────────────────────────────────────────────────────────────────────────────────────────
[Input 1]     |           |           |               |             |           |
[Input 2]     |           |           |               |             |           |
[Packaging]   |           |           |               |             |           |
[Finished]    |           |           |               |             |           |

COUNTING SCHEDULE:
- Daily: High-value / fast-moving items
- Weekly: Medium-value items
- Monthly: Full physical count of everything

VARIANCE PROTOCOL:
- Variance < 2%: Record and monitor
- Variance 2-5%: Investigate same day
- Variance > 5%: Stop operations, full audit, report to owner/board
```

### STEP 7 — Cost-Per-Unit Tracking
The most important metric most African enterprises never calculate:

```
COST-PER-UNIT CALCULATOR
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

                                    Per Unit    Per Batch    Per Month
                                    ─────────   ──────────   ──────────
Raw materials
Packaging
Direct labour
Transport (inbound)
Transport (outbound)
Storage / utilities
Equipment maintenance
Waste / loss allowance
─────────────────────────────────────────────────────────────────────
TOTAL COST PER UNIT
─────────────────────────────────────────────────────────────────────
Selling price per unit
MARGIN PER UNIT
MARGIN %
─────────────────────────────────────────────────────────────────────

BREAK-EVEN VOLUME:          units per [period]
CURRENT VOLUME:             units per [period]
SAFETY MARGIN:              %

RULE: If margin < 15%, redesign the chain before scaling.
```

### STEP 8 — Resilience & Risk Plan

```
SUPPLY CHAIN RISKS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Risk                  | Likelihood | Impact  | Mitigation                    | Trigger to Activate
─────────────────────────────────────────────────────────────────────────────────────────────────
Supplier failure      |            |         |                               |
Transport disruption  |            |         |                               |
Power outage          |            |         |                               |
Seasonal shortage     |            |         |                               |
Price spike (inputs)  |            |         |                               |
Equipment breakdown   |            |         |                               |
Key staff absence     |            |         |                               |
Market demand drop    |            |         |                               |
Regulatory change     |            |         |                               |
Theft / pilferage     |            |         |                               |
```

## Output Format
Deliver all 8 steps as a single operational document. Use real numbers where user provides data; use realistic estimates with [VERIFY] tags where data is missing.

## Connects To
- `/asset-audit` — identifies physical assets available for the chain
- `/solve` — initial business design that this skill operationalises
- `/execute` — daily tracking of the operations designed here
- `/market-intel` — customer and competitor data feeding into outbound design
- `/financial-model` — cost-per-unit data feeds directly into financial projections
- `/diagnose` — identifies supply chain failures in existing operations
