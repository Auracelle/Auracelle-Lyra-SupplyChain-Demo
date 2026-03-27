# Auracelle Lyra — Checks and Balances
### Proprietary Demonstration Build · v2.1.1

**Auracelle AI Governance Labs · Director G.A. Evans**
**© 2026 Grace-Alice Evans. All rights reserved.**

---

## What This Is

Auracelle Lyra is a multi-domain governance assurance simulation platform built on the proprietary **E-AGPO-HT** (Evans Accelerated Governance Policy Optimization — Hierarchical Theory) and **E-AGSO-HT** (Evans Accelerated Governance Standards Optimization — Hierarchical Theory) frameworks. This build — *Checks and Balances* — is the active proprietary demonstration version used for institutional briefings, doctoral research, and policy engagement with IAEA, UNIDIR, NATO, and academic audiences.

The platform addresses five intersecting thematic domains:

- **Frontier Technology Governance** — AI, Nuclear, Space, BioTech, Energy, Quantum
- **Cybersecurity** — embedded cyber resilience indicators across all domains
- **Multilateralism** — treaty-based verification regimes, cross-border cooperation, institutional capacity
- **Computational Decision Science** — three-stratum hierarchical scoring, logistic sigmoid aggregation, weighted multiplicative formulation
- **Wargaming** — role-based game state, 3D governance network, scenario stress-testing, cascade effects

It is a single self-contained HTML file. No installation, no server. Open in any modern browser.

---

## Architecture

The simulation operates across two pages and three strata.

**Page 1 — E-AGPO · Policy Metrics**
Evaluates governance policy performance for the AI domain using 10 canonical Narrow Operational Factors (NOFs) mapped across the seven Broad Governance Capabilities (STI · SAD · ESI · NDM · SRA · IIC · ASI). Supports document upload for automated Claude AI scoring, and country-level comparative wargaming across 8 country profiles.

**Page 1 — Wargaming Demo (primary mode)**
Full multi-domain simulation sandbox. Six domains selectable (Nuclear, AI, Space, Biotech, Renewable, Quantum). Seven tabs:

| Tab | Function |
|---|---|
| Game State | Role, standard, and country configuration. Policy/Actor/Compliance/Verification/Risk state vector |
| Registry Scoring | Live indicator → NOF → BAC → g-GACn scoring chain with adjustable sliders |
| BGC Engine | Seven Bounded Governance Capability sliders with real-time g-GWC computation |
| Governance Network | Three.js 3D actor graph — domain-specific institutional nodes, auto-rotating |
| Compliance Convergence | Three.js 3D animation — 20 real safeguards actors converging toward target compliance |
| Proliferation Pathways | Domain-specific governance failure pathways with BGC weakness mapping |
| Actions & Shocks | Eight governance interventions with cascade effects through the state vector |

**Page 2 — E-AGSO · Assurance Stress-Test**
Tests whether governance standards can be verified, audited, and enforced under real-world conditions. Four tabs: Audit Evasion surface modeling, Assurance NOF Calculator, Continuity of Knowledge (CoK) degradation timeline, and the Scenario Library.

**Three-Stratum Scoring Architecture**

```
Stratum I  — NOF (Narrow Operational Factors): indicator-level measurement
Stratum II — BAC (Broad Assurance Capabilities): aggregated capability scores
Stratum III — g-GACn / g-GWC: global governance assurance composite score
```

Two aggregation models are available and compared throughout the simulation:
- **Additive** (weighted sum): reveals partial governance strength
- **Multiplicative (weakest-link)**: collapses when any single capability fails — the analytically correct model for assurance systems

---

## Nuclear Domain — Canonical E-AGPO-HT NOFs

The Nuclear domain implements 10 canonical NOFs aligned to the Domain Specific E-AGPO-HT Mathematical Intelligence specification. Each NOF has a four-indicator measurement vector normalized to [0,1].

| ID | Acronym | Name | Capability |
|---|---|---|---|
| NUC_01 | ADS-NUC | Anomaly Detection Sensitivity | BAC02 |
| NUC_02 | DOC-NUC | Declared-vs-Observed Consistency | BAC02 |
| NUC_03 | SCC | Safeguards Coverage Completeness | BAC01 |
| NUC_04 | ARI-NUC | Access Realism Index | BAC01 |
| NUC_05 | RTER-NUC | Red-Team Evasion Robustness | BAC03 |
| NUC_06 | ELC-NUC | Escalation Ladder Clarity | BAC05 |
| NUC_07 | CLB-NUC | Credibility-Legitimacy Balance | BAC06 |
| NUC_08 | IRA-NUC | Inspection Resource Adequacy | BAC04 |
| NUC_09 | TCA-NUC | Technical Complexity Adaptation | BAC07 |
| NUC_10 | TCTR-NUC | Transport Chain & Recovery | BAC03 |

NUC_10 (TCTR-NUC) was added in v2.1 specifically to address the IAEA ITDB March 2026 transport security findings. Its four indicators are calibrated directly to the ITDB factsheet data.

---

## The Oman Threshold Scenario

**Where to find it:** Page 2 → Assurance Stress-Test → Scenario Library → *Crisis · Live* (red tag)

The Oman Threshold is the simulation's live real-world calibration case. It models the governance failure sequence of **February 26–28, 2026** — the period in which Omani-mediated US–Iran nuclear negotiations approached a reported breakthrough before US-Israel strikes began on February 28.

### What It Demonstrates

The scenario stress-tests four NOFs simultaneously using indicator values derived from open-source evidence:

| NOF | Indicator Collapse | Score |
|---|---|---|
| DOC-NUC · Declared-vs-Observed Consistency | Declaration disputed between Oman and US envoy; material balance unverifiable | 0.32 ❌ |
| ELC-NUC · Escalation Ladder Clarity | Trigger clarity absent; diplomatic timeline compressed to zero; Israeli veto operative | 0.28 ❌ |
| IRA-NUC · Inspection Resource Adequacy | IAEA access suspended post-strike; inspector-hours per facility near-zero | 0.07 ❌ collapse |
| CLB-NUC · Credibility-Legitimacy Balance | Action condemned by Oman, globally contested; diplomatic fallout maximal | 0.24 ❌ |

### The Key Mathematical Finding

The scenario validates the multiplicative (weakest-link) g-GAC formulation as analytically correct for assurance system failures:

| Model | g-GAC Score | Interpretation |
|---|---|---|
| Additive (weighted sum) | **0.412** | Masks failure — partially intact BACs compensate |
| Multiplicative (weakest-link) | **0.089** | Correctly identifies collapse — IRA-NUC → 0.07 drives product to near-zero |
| g-ARI impact | **−0.231** | Largest negative delta in the scenario library |

**The implication:** When IRA-NUC collapsed (IAEA access suspended), the entire assurance architecture failed regardless of the state of other capabilities. One broken verification leg collapses the system. This is the core argument for the multiplicative formulation — and it is now a live empirically-grounded case, not a theoretical proposition.

### Post-Conflict Architecture

The scenario includes a 12-point post-conflict verification architecture reform pathway, structured as a future "Iran Verification Architecture" modelled on Chemical Weapons Convention inspection protocols. It is designed as a calibration baseline for scoring future post-conflict governance recovery — directly applicable to the IAEA Safeguards Symposium 2026 submission.

---

## IAEA ITDB Transport Report — Gaps Addressed

The IAEA Incident and Trafficking Database (ITDB) factsheet released March 23, 2026 identified transport as the dominant nuclear security vulnerability. The simulation addresses these findings through the TCTR-NUC (NUC_10) indicator set and the **ITDB Transport Vulnerability** scenario.

### ITDB Key Findings vs. Simulation Coverage

| ITDB Finding | Indicator | Baseline Score |
|---|---|---|
| 55% of thefts occur during authorized transport | `multi_handler_coc_continuity` | 0.42 ⚠ |
| 59% of transport-stolen material never recovered | `in_transit_detection_capability` | 0.38 ❌ |
| Only 34 of 145 states actively report (23%) | `cross_border_handoff_protocol` | 0.35 ❌ |
| Partial carrier security coverage across member states | `carrier_security_certification` | 0.45 ⚠ |
| Rising trend: 70% of thefts during transport in last decade | TCTR-NUC aggregate | 0.40 ❌ |

The ITDB Transport Vulnerability scenario (Page 2 → Scenario Library, *Nuclear · ITDB* tag) embeds the full factsheet data in the scenario output panel and provides a four-point reform pathway with quantified improvement targets.

**Where to find it:** Page 2 → Assurance Stress-Test → Scenario Library → *Nuclear · ITDB*

### Supply Chain Issues Addressed

The simulation models the supply chain as a multi-layer governance failure domain, spanning four interconnected failure modes:

**1. Multi-handler chain-of-custody fragmentation**
Radioactive material transits through road, rail, air, and waterway carriers with no unified chain-of-custody standard. Each handoff between handlers represents a break point. The `multi_handler_coc_continuity` indicator (NUC_10) scores this at 0.42 — critical. The Continuity of Knowledge tab (Page 2) models how chain-of-custody breaks accumulate into exploitable assurance gaps over a 12-month inspection cycle.

**2. Detection gap: material leaves the governance perimeter undetected**
With 59% of transport-stolen material unrecovered, the simulation models `in_transit_detection_capability` as a BAC03 (Auditability & Traceability) degradation factor. The absence of unified radiation portal monitoring across transport modes — road, rail, maritime, air — is the primary driver of the low baseline score.

**3. Disused source disposal entering industrial supply chains**
The ITDB flagged a rising trend of manufactured goods contaminated with radioactive material appearing at metal recycling facilities. This cross-domain failure — nuclear sources entering the industrial/energy supply chain — is modelled in the Biotech domain under `dual_use_risk_controls` and in the Energy/Renewable domain under `supply_chain_resilience`. The Proliferation Pathways tab in the Wargaming Demo surfaces this as a domain-specific failure pathway.

**4. Carrier certification and regulatory fragmentation**
The voluntary nature of the ITDB reporting system (34/145 states) reflects the same structural weakness as voluntary carrier certification — governance that depends on opt-in participation fails at scale. The `carrier_security_certification` indicator scores this at 0.45, and `cross_border_handoff_protocol` at 0.35 — the lowest indicator in the Nuclear domain. The Energy/Renewable domain models the equivalent problem through `noncompliance_response_strength` and `regulatory_reporting_quality`.

---

## Scenario Library

**Page 2 → Assurance Stress-Test → Scenario Library** — 7 pre-loaded scenarios.

| Scenario | Domain Tag | g-ARI Δ | What It Models |
|---|---|---|---|
| AI-Assisted Nuclear Facility | Cross-Domain | −0.094 | AI facility management breaks IAEA safeguards designed for physical accountancy |
| Audit-Shopping Under Dual Oversight | Nuclear | −0.071 | State exploits IAEA/Euratom jurisdictional overlap |
| Inspector Capacity Strain: 40% Shortage | Nuclear | −0.082 | SMR expansion outpaces IAEA inspector capacity |
| Standards Fragmentation: EU/US/ISO | AI Domain | −0.068 | Three AI governance frameworks diverge; cross-jurisdictional equivalence collapses |
| Integrated Safeguards Reform | Reform | +0.118 | Additional Protocol expansion — the only positive scenario |
| **Oman Threshold (Feb 2026)** | **Crisis · Live** | **−0.231** | **Real-world diplomatic collapse; multiplicative g-GAC collapse case** |
| ITDB Transport Vulnerability | Nuclear · ITDB | −0.094 | 55% transport theft rate scored against TCTR-NUC indicator set |

---

## Sprint 2 — What Comes Next

The following additions are scoped for v2.2 (April 2026) and v2.3 (May 2026), addressing residual gaps identified in the ITDB audit and thematic framework review.

### Residual Gaps Identified

| Gap | Description |
|---|---|
| G-1 | Physical package design / SSR-6 compliance not yet scored |
| G-2 | In-transit emergency response protocol not yet a distinct indicator |
| G-3 | ITDB participation incentive pathway (why 111 states don't report) not modelled |
| G-4 | Scrap metal / disused source disposal lacks a dedicated cross-domain proliferation pathway |
| G-5 | Quantum-enabled tracking technologies for transport not yet in QTM/NUC cross-domain |

### v2.2 Additions (Sprint 1 — April 2026)

**NUC_10 Expansion** — Two new indicators added to the TCTR-NUC vector, closing G-1 and G-2:
- `package_design_compliance` — SSR-6 / IAEA TDL-series conformance rate (baseline: 0.48)
- `in_transit_emergency_response` — protocol existence, drill frequency, national coordination (baseline: 0.40)

**NUC_11 · ITDB Participation Architecture (ITPAC-NUC)** — New NOF addressing G-3. Models the structural failure that keeps 111 of 145 ITDB member states from actively reporting. Indicators: `voluntary_to_mandatory_pathway` (0.25), `poc_network_coverage` (0.23, calibrated to 34/145), `reporting_timeliness`, `itdb_data_quality_score`. Aggregate baseline: 0.36 — structural governance failure.

**Scrap Metal Cross-Domain Proliferation Pathway** — G-4. New pathway entry spanning Nuclear × Renewable domains in the Proliferation Pathways tab, explicitly modelling the ITDB-flagged rising trend of contaminated manufactured goods in industrial supply chains.

**Scenario 8 · Physical Protection Gap** — Scenario scoring a state that meets transport licensing requirements but fails on physical protection (SSR-6 non-conformance) and has no tested in-transit emergency response protocol. Aligned to IAEA Nuclear Security Series No. 9-G. g-ARI Δ: −0.078.

### v2.3 Additions (Sprint 2 — May 2026)

**g-GAC Time-Series Panel** — Animates the Oman Threshold governance failure and recovery trajectory across four time-points (T+0 Feb 26, T+1 Feb 28, T+30 current, T+180 hypothetical post-conflict regime). Additive vs. multiplicative g-GAC lines compared. Directly supports the IAEA Safeguards Symposium 2026 abstract.

**QTM/NUC Cross-Domain NOF** — Quantum-sensor-based tamper detection and quantum-encrypted chain of custody for Category 1–3 radioactive shipments. Closes G-5. Baseline: 0.15–0.25 (nascent — no deployed standards).

**Oman Threshold T+180 Extension** — Post-conflict verification architecture pre-populated with hypothetical Iran Verification Architecture indicator values. Enables live scoring of what a functional post-conflict regime would need to achieve.

**AI Domain DCSF NOF** — Adds the missing Deployment Context Simulation Fidelity factor specified in the Domain Specific Mathematical Intelligence document. Completes the canonical 11-NOF AI specification.

---

## Institutional Context

This simulation supports:

- **Doctoral research** — Bath Spa University (supervisor: Dr. John Curry). Thesis: *Testing Public Policy Outcomes through War Gaming Methodologies for Strengthening AI Governance*
- **NATO STO SAS-219** — High North Scenarios for Wargaming and Analysis (Winter Storm 2030). Standard Role Member representing the United States. Contributions to R5 (Digitally Wargaming) and R6 (Wargaming Definition) subgroups
- **UC Berkeley CLTC** — Non-Resident Senior Fellow. Published: Cleaveland, Evans et al. (2021)
- **Geneva Cyber Week 2026** — May (Auracelle Orion presenting)
- **UNIDIR AISE26** — June (Auracelle Lyra / Charlie demonstration)
- **GESDA Geneva Science Diplomacy Week** — June 22–26
- **IAEA Safeguards Symposium 2026** — November (abstract submitted, Auracelle Lyra)

---

## Technical Notes

- Single-file HTML/CSS/JS — no build process, no dependencies beyond CDN
- Three.js r128 (via Cloudflare CDN) for 3D visualisations
- Anthropic Claude API integration for document scoring and comparative analysis
- All scoring computed client-side; no data transmitted except via explicit Claude API calls
- Tested: Chrome, Firefox, Safari (desktop)
- Three.js 3D features require WebGL-capable browser

---

## Intellectual Property Notice

This simulation, all underlying frameworks, scoring architectures, indicator taxonomies, mathematical formalizations, and scenario content are the proprietary intellectual property of **Auracelle AI Governance Labs** and **Grace-Alice Evans**. See LICENSE for terms. Unauthorized reproduction, adaptation, or use is strictly prohibited.

For licensing or institutional access: **Auracelle AI Governance Labs**

---

*Auracelle AI Governance Labs · auracelle.ai*
*E-AGPO-HT / E-AGSO-HT Framework · © 2026 Grace-Alice Evans*
