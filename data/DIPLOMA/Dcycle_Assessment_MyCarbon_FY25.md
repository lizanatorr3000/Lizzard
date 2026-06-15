# Diploma PLC — Assessment of MyCarbon FY25 Carbon Footprint

> **Client:** Diploma PLC · **Calc by:** MyCarbon (manual, non-software)
> **Period assessed:** FY25 (1 Oct 2024 – 30 Sep 2025) + FY22–FY24 rebaselined history
> **Author:** Liza Adova, Dcycle CS · **Date:** 2026-05-28
> **Purpose:** Input to the FY26 onboarding kickoff. Qualitative methodology assessment — no Dcycle restated numbers.

---

## Executive verdict

MyCarbon's FY25 inventory is **standards-aligned (GHG Protocol Corporate Standard + ISO 14064-1)** and complete across all 15 Scope 3 categories. **But ~90% of the Scope 3 footprint sits on spend-based estimates** — the lowest data-quality tier in the GHG Protocol hierarchy — and **three categories (Cat 1, Cat 4, Cat 11) carry material uncertainty** that Diploma's own governance framework (Pillar 5) already flags as HIGH/CRITICAL risk.

**FY26 migration to Dcycle is the right next move:** it tackles every HIGH-risk gap Diploma itself documented, replaces MyCarbon's "consistently flawed" manual templates, and lets the organisation move from spend → activity data on the categories that actually drive the footprint.

**SBTi trajectory flag:** the rebaseline anchored FY22 at **229,684 tCO2e**. The -30% Scope 3 target by FY30 implies ~160k tCO2e — but FY25 H1 (119,766) annualises to ~240k. The trajectory gap is real and worth surfacing internally.

---

## 1. Headline numbers — FY25 H1, market-based

| Scope | tCO2e | % | Notes |
|---|---:|---:|---|
| Scope 1 | 2,280 | 1.9% | Stationary combustion + company vehicles + refrigerants |
| Scope 2 (market) | 3,419 | 2.9% | Dual-reported; location-based = 2,811 |
| Scope 3 | 114,067 | 95.2% | 13 of 15 categories included |
| **Total** | **119,766** | 100% | Implied full-FY25 ≈ 240k tCO2e |

### Scope 3 breakdown (FY25 H1)

| Cat | Emission source | tCO2e | % S3 | Method |
|---|---|---:|---:|---|
| 1 | Purchased goods & services | **79,412** | **70%** | Spend-based |
| 4 | Upstream transportation & distribution | **22,660** | **20%** | Hybrid spend + activity |
| 7 | Employee commuting | 3,379 | 3% | FY24 survey extrapolated |
| 6 | Business travel | 3,172 | 3% | Spend-based |
| 2 | Capital goods | 1,553 | 1% | Spend-based |
| 8 | Upstream leased assets | 1,436 | 1% | Within S1/2 envelope |
| 3 | Fuel & energy-related (WTT) | 1,173 | 1% | Derived from S1/S2 |
| 11 | Use of sold products | 861 | <1% | Wattage × usage |
| 5 | Waste in operations | 399 | <1% | Activity (primary) + spend (secondary) |
| 12 | End-of-life of sold products | 20 | <1% | Material composition modelling |

**Cat 1 + Cat 4 = 90% of Scope 3.** The assessment focuses there.

---

## 2. Rebaselining snapshot

MyCarbon retrofitted FY22–FY24 to reflect newly acquired entities. Net effect:

| Year | Original total | Rebaselined total | Δ |
|---|---:|---:|---:|
| FY22 (base year) | 206,132 | **229,684** | **+11%** |
| FY23 | 161,047 | **271,201** | **+68%** |
| FY24 | n/a | 253,842 | — |

The FY23 jump is driven almost entirely by **Cat 1** (81k → 192k, +136%), which MyCarbon attributes to full-year extrapolation of mid-year-acquired sites backward into FY23/FY22.

**Defensible, but the baseline now moves.** SBTi (-50% S1+S2 / -30% S3 by FY30) is anchored to **229,684 tCO2e**, not 206,132. Each future acquisition reopens the math.

**Recommendation:** lock an explicit rebaseline trigger (SBTi's 5% threshold rule is the standard) before FY26.

---

## 3. What's methodologically sound

- **Standards alignment** — GHG Protocol Corporate Standard, ISO 14064-1, operational control boundary.
- **Scope 2 dual reporting** — Location (IEA / EPA eGRID) + Market with proper residual-mix hierarchy (RECs → AIB Europe / Green-e USA → fallback to location).
- **Refrigerants** — Mass-of-gas with DEFRA FY25 GWPs.
- **District heating** — Geography-aware EF prioritisation (DEFRA / EEA / UBA Germany).
- **Scope 3 completeness** — All 15 categories formally reviewed; exclusions (Cat 10, 13, 14, 15) documented with audit-grade justifications.
- **End-of-life refinement** — Update from 100% landfill → 50/50 metal/plastic + 80/20 recycle/landfill is an improvement reflecting modern industrial waste streams.
- **Cat 9 consolidation into Cat 4** — Acceptable per GHG Protocol when freight is paid by the reporting entity; avoids double counting (though it reduces transparency).

---

## 4. Material weaknesses — by category

### 🔴 Cat 1 — Purchased Goods & Services (70% of S3) — HIGH RISK

- **100% spend-based**, no supplier-specific factors.
- Per kickoff with Quresh Mukadam (FB&A, 2026-05-05): HFM consolidation system has **no supplier-level detail** for most spend; only ~50% of spend maps to "key suppliers" (~13 for Windy City Wire alone).
- Remaining 50% mapped via generic product categories (O-rings, seals, wire/cable, adhesives) or generic OPEX buckets.
- Manual exclusions ("intangible purchases, account adjustments, depreciation, stock provisions") applied without a documented rule set — auditability gap.
- **Inconsistent typology between BUs:** Life Sciences (Somagen, Vantage) report packaging/consumables as *supplier names*, while Controls/Seals report as *product types*. EF mapping is not directly comparable across the group.

> **Diploma's own Pillar 5 (Data Quality & Gaps) flags this verbatim:** *"Spend categories currently don't provide enough granularity and consistency of use — HIGH risk. Move to a primary data approach for category one as quickly as possible."*

### 🔴 Cat 4 — Upstream Transport & Distribution (20% of S3) — HIGH RISK

- **65% Air / 35% Road mode-split assumption** applied to *general freight spend*. For a global industrial distributor mixing wire, seals, and medical consumables, the real air share is almost certainly far below 65%. This single assumption likely **materially inflates Cat 4**.
- WCW (largest entity) has **no UPS data** for FY25 — forward-extrapolated from FY24 × WCW revenue growth.
- "Netting out" of expenditure for WCW + Dicsa Spain where detailed activity data exists creates a **double-counting risk** (Pillar 5 flags this as HIGH).

### 🔴 Cat 11 — Use of Sold Products — HIGH RISK

- **Single hardcoded usage profile:** `Wattage × 7 hrs/day × 365 days × 10 years` applied uniformly to ALL machines.
- A diagnostic analyser used 1 hr/day in a hospital and a continuous monitoring device differ by 10×+ in real usage. This averages everything into a single (uncertain) number.
- Somagen Canada FY25 data unavailable → extrapolated from FY24 × Somagen revenue growth.

> **Pillar 5:** *"Machinery data suffers from oversimplified assumptions and lack of granularity — all machines defaulted to 7 hrs/day. HIGH risk."*

### 🟡 Cat 12 — End of Life — MEDIUM RISK

- Only Australia has individual product weight data. Canada extrapolated from FY24.
- **All other entities use a proxy of a proxy:** a "weight of sold products intensity" derived from `outbound weight ÷ outbound logistics spend`, then applied back to logistics spend to *estimate weight*. Compounding uncertainty.
- 50/50 metal/plastic + 80/20 recycle/landfill = single global assumption across all regions and product types (consumer-grade vs. industrial waste streams treated identically).

### 🟡 Cat 6 — Business Travel — MEDIUM RISK

- Pure spend-based across Air / Rail / Other.
- Decentralised travel booking (per Quresh: *"each business does it their own way"*) — no consolidated PNR or distance data feasible without primary collection.

### 🟡 Cat 7 — Employee Commuting — MEDIUM RISK

- FY24 survey response, per-employee intensity carried forward to FY25 headcount; response ratio scaled per site.
- Response bias in the original survey is now baked into FY25. Survey should be re-run for FY26.

### 🔴 Cross-cutting — Pillar 5 CRITICAL flags

> Direct quotes from Diploma's own governance framework:
> - *"Centralised calculation templates are consistently flawed (formulas break, wrong emission factors are applied). High risk of incorrect final CO2e tonnage; requires annual manual intervention."*
> - *"Inconsistent spending data across tabs undermines trust; need a single source of truth. Negative spend present. CRITICAL: directly affects validity of the total Scope 3 calculation."*

This is the strongest argument for migration: **Diploma already documented these gaps internally.** Dcycle's value proposition is operationalising fixes to issues they've already named.

---

## 5. Dcycle migration roadmap

### Lane 1 — FY25 parallel comparison *(in flight)*

Agreed in the 2026-05-05 kickoff with Lia / Tai / Quresh. Run Cat 1 + Cat 4 (~90% of S3) through Dcycle alongside MyCarbon's FY25 figures.

- [ ] Receive raw HFM extract + HFM-to-business code map from Quresh
- [ ] Load Cat 1 supplier-named spend (50% of value) via supplier-based matching with SIC codes
- [ ] Load remaining Cat 1 spend via Dcycle's product-category / CapEx-style flow
- [ ] Load Cat 4 freight spend split by HFM account (`PL11310` Freight Out, `PL11410` Freight In) with explicit mode flags where available — challenge the 65/35 air/road assumption
- [ ] Deliver delta-vs-MyCarbon report by category, BU, and EF source

### Lane 2 — FY26 full migration *(with rebaseline)*

- [ ] **Cat 1:** primary data per Diploma's own Pillar 2.1 plan — material-specific (weight × EF) for raw materials, supplier EFs where obtained
- [ ] **Cat 4:** replace mode assumption with weight × mode × distance from carrier reports (UPS / DHL / FedEx exports — already exists for WCW)
- [ ] **Cat 11:** collect machine-level usage hours from sales / service records; default profiles per machine class instead of single global default
- [ ] **Cat 7:** rerun the commuting survey for FY26 — do not extrapolate twice
- [ ] **Scope 1 & 2:** centralise on Dcycle to retire MyCarbon's "consistently flawed" template (resolves Pillar 5 CRITICAL action)

### Lane 3 — Governance hardening *(independent of platform)*

- [ ] Lock an acquisition rebaseline trigger (SBTi 5% rule)
- [ ] Implement Pillar 3 Data Validation Checklist before the FY26 collection cycle
- [ ] Single source of truth for spend reconciliation between HFM and the Scope 3 ledger (resolves Pillar 5 CRITICAL)
- [ ] Mandate consistent product-category typology across all BUs (especially Life Sciences vs. Seals/Controls)

---

## 6. Appendix — Per-category card (weak categories only)

| Cat | MyCarbon approach | Risk | Dcycle approach |
|---|---|---|---|
| 1 | Spend-based, manual ledger exclusions, no supplier EFs | 🔴 HIGH | Supplier-name matching (SIC + country EFs) for known suppliers, product-category EFs for the rest, primary-data flow when raw materials available |
| 4 | 65/35 air/road on general freight spend; WCW extrapolated; netting risk | 🔴 HIGH | Weight × mode × distance from carrier reports; per-shipment mode capture; eliminates the air-mode assumption |
| 11 | Wattage × 7 hrs × 365 × 10 yrs uniform | 🔴 HIGH | Per-SKU usage profile by machine class; usage hours from service/install data |
| 12 | Australia: actual weight. Others: weight-from-spend proxy. Global 50/50, 80/20 | 🟡 MED | Per-product material composition + region-specific EoL fate (EU WEEE vs US vs APAC) |
| 6 | Spend on Air / Rail / Other | 🟡 MED | T&E system integration (distance-based per trip); fallback to spend only for unconsolidated BUs |
| 7 | FY24 survey × FY25 headcount | 🟡 MED | Annual rerun via Dcycle commuting survey module; live response ratio scaling |

---

## Source artefacts

Located at `/Users/lizaadova/Code/Lizzard/data/DIPLOMA/`:

1. `Diploma Methodology FY25.pdf` — MyCarbon methodology manual (9 pp)
2. `Diploma (all) Scope 3 Data - FY25 - 14.10.2025 - Copy.xlsx` — HFM raw extract (13 sheets, 478×315 max)
3. `Final_v2_Diploma Rebaselining - Summary (1).xlsx` — FY22–FY25 H1 rebaselined totals
4. `Diploma Carbon Data Governance Framework & Action Plan.xlsx` — 8-pillar internal governance framework (the source of every Pillar 5 quote above)

**Fathom context calls:**
- Kickoff with Quresh, Lia, Tai (2026-05-05): `fathom.video/calls/660008342`
- Internal handover Jonathan → Cecilia (2026-01-08): `fathom.video/calls/525879962`

**HubSpot:** Diploma Plc, ID `20652458506` — Tier 1, lifecycle = customer, owner = Lucia Mosquera, contract Jan 2026 → Jan 2027 (£40,105 TCV, 1 open deal £51,935 pipeline).
