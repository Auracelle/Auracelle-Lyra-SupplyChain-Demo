# Auracelle Lyra — Sprint Plan
## Checks and Balances · Proprietary Development Roadmap

**Auracelle AI Governance Labs · Director G.A. Evans**
**Framework: E-AGPO-HT / E-AGSO-HT**
**Current Build: v2.1.1 · March 27, 2026**

---

## Current State Snapshot (v2.1.1)

| Component | Status |
|---|---|
| File | `Auracelle_Lyra_Checks_and_Balances_Proprietary_Demo.html` |
| Pages | 2 (E-AGPO Policy Metrics · E-AGSO Assurance Stress-Test) |
| P3 Wargaming Domains | 6 (Nuclear, AI, Space, Biotech, Renewable, Quantum) |
| Nuclear NOFs | 10 canonical (NUC_01–NUC_10, E-AGPO-HT aligned) |
| Scenario Library | 7 scenarios (6 stress-test + 1 live crisis) |
| Three.js visualisations | GNN 3D Actor Graph · Compliance Convergence |
| API integration | Anthropic Claude (wargame analysis · document extraction) |
| GitHub repo | `auracelle-lyra-checks-balances` (private) |
| CHANGELOG | v1.0 → v2.0 → v2.1 → v2.1.1 |

### Scenario Library (v2.1.1)
| ID | Tag | Title | g-ARI Δ |
|---|---|---|---|
| ai_nuclear | Cross-Domain | AI-Assisted Nuclear Facility: Assurance Continuity Break | −0.094 |
| audit_shopping | Nuclear | Regime Arbitrage: Audit-Shopping Under Dual Oversight | −0.071 |
| capacity_strain | Nuclear | Inspector Capacity Strain: 40% Shortage | −0.082 |
| standards_diverge | AI Domain | Standards Fragmentation: EU AI Act vs. US NIST vs. ISO | −0.068 |
| integrated_reform | Reform | Integrated Safeguards Reform: Additional Protocol Expansion | +0.118 |
| oman_threshold | Crisis · Live | Oman Threshold: Diplomatic Collapse (Feb 2026) | −0.231 |
| transport_security | Nuclear · ITDB | ITDB Transport Vulnerability: 55% of Thefts in Transit | −0.094 |

### Nuclear NOF Registry (v2.1.1 — E-AGPO-HT Canonical)
| ID | Acronym | Name | BAC |
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

---

## Identified Gaps (from ITDB + Thematic Audit)

Five residual gaps identified against the IAEA ITDB March 2026 factsheet
and the Frontier Technology Governance thematic framework:

| Gap | Description | Priority |
|---|---|---|
| G-1 | Physical package design / SSR-6 compliance (shipment protection) | High |
| G-2 | In-transit emergency response protocol (NUC_10 extension) | High |
| G-3 | ITDB participation incentive pathway (23% → 145 states model) | Medium |
| G-4 | Scrap metal / disused source disposal (cross-domain NUC/EN lifecycle) | Medium |
| G-5 | Quantum-enabled tracking for transport (cross-domain QTM/NUC) | Low |

---

## Sprint 1 — In Progress
### NUC_10 Expansion & Physical Protection Layer
**Target version: v2.2**
**Status: 🔄 In Progress**
**Conference alignment: IAEA Safeguards Symposium 2026 (November) · UNIDIR AISE26 (June)**

**Objective:** Extend TCTR-NUC (NUC_10) to address gaps G-1 and G-2,
and add a cross-domain NUC/EN scrap metal proliferation pathway (G-4).

#### Sprint 1 Tasks

**S1-T1 · NUC_10 Indicator Expansion** `[G-1, G-2]`
Add two new indicators to the TCTR-NUC indicator vector (expand from 4 to 6):
- `package_design_compliance` — SSR-6 / IAEA TDL-series conformance rate
  - Baseline: 0.48 (estimated from conference proceedings)
- `in_transit_emergency_response` — protocol existence, drill frequency,
  response time to transit incident, coordination with national authorities
  - Baseline: 0.40 (low — conference identified as a gap)

Update `P3_STARTERS.Nuclear` with the two new indicators.
Update `NUC_10` in `P3_REG` to include both new `inds` entries.

**S1-T2 · NUC_11 · ITDB Participation Architecture (ITPAC-NUC)** `[G-3]`
Add new NOF to Nuclear domain mapped to BAC05 (Interoperability & Conformance):
- `NUC_11`: ITDB Participation Architecture (ITPAC-NUC)
- Indicators: `voluntary_to_mandatory_pathway`, `poc_network_coverage`,
  `reporting_timeliness`, `itdb_data_quality_score`
- Baseline values calibrated to 34/145 participation rate:
  `voluntary_to_mandatory_pathway: 0.25` (no treaty obligation)
  `poc_network_coverage: 0.23` (34/145 = 23%)
  `reporting_timeliness: 0.45`
  `itdb_data_quality_score: 0.50`
- Starter: 0.36 aggregate — marks this as a structural governance failure

**S1-T3 · Proliferation Pathways: Scrap Metal Cross-Domain** `[G-4]`
Add scrap metal / disused source pathway to the P3 Proliferation Pathways tab.
Currently the pathways tab only shows per-domain pathways; add a cross-domain
entry spanning Nuclear + Renewable:
- Title: "Disused Source Disposal Failure"
- Desc: "Radioactive sources from medical, industrial, or energy applications
  enter scrap metal supply chains undetected. ITDB: rising trend 2024–2025."
- Example: "Contaminated pipes / steel reported at recycling facilities, Northern Europe"
- BGC weakness tags: [IIC, ASI]
- Domain: Nuclear × Renewable (cross-domain entry)

**S1-T4 · Scenario 8 · Physical Protection Gap** `[G-1, G-2]`
Add eighth scenario to the Scenario Library:
- Key: `transit_protection_gap`
- Tag: `nuclear` · Label: `Nuclear · SSR-6`
- Title: Physical Protection Gap: Package Design & Emergency Response Failure
- ariDelta: −0.078
- Scenario models a state that meets transport licensing requirements but fails
  on physical protection (SSR-6 non-conformance) and has no tested emergency
  response protocol for in-transit incidents
- Reform pathway: 4 steps aligned to IAEA Nuclear Security Series No. 9-G

**S1-T5 · Registry Scoring Tab Label Update**
Update the Registry Scoring tab subtitle for Nuclear domain to display:
`"NUC_01–NUC_11 · E-AGPO-HT Canonical · ITDB-calibrated"`
Replace "NUC_01–NUC_10" reference.

**S1-T6 · CHANGELOG v2.2 Entry**
Document all Sprint 1 changes with indicator baseline sources cited.

---

## Sprint 2 — Planned
### Quantum-Nuclear Cross-Domain & g-GAC Time-Series
**Target version: v2.3**
**Status: 📋 Planned**
**Conference alignment: Geneva Cyber Week 2026 (May) — Note: Orion presenting, Lyra as reference**

**Objective:** Address G-5 (quantum tracking technologies) and implement
the g-GAC time-series scoring capability for the Oman Threshold scenario —
enabling T+0 / T+1 / T+30 / T+180 governance recovery trajectory visualisation.

#### Sprint 2 Tasks

**S2-T1 · QTM/NUC Cross-Domain NOF: Quantum Transport Tracking (QTT)** `[G-5]`
Add a cross-domain entry bridging Quantum and Nuclear domains:
- Models quantum-sensor-based tamper detection and quantum-encrypted chain
  of custody for Category 1–3 radioactive shipments
- Maps to TCA-NUC (NUC_09) as a forward-looking capability upgrade
- Indicator: `quantum_sensor_readiness`, `qkd_chain_of_custody`,
  `pqc_transport_protocol`, `cross_modal_interop`
- Baseline: 0.15–0.25 (nascent technology, no deployed standards)

**S2-T2 · g-GAC Time-Series Panel**
Add a Time-Series tab to the P3 wargaming engine for the Nuclear domain.
Three time-points pre-loaded for the Oman Threshold scenario:
- T+0 (Feb 26, 2026): Pre-strike snapshot — g-GACn: 0.412 (additive) / 0.089 (multiplicative)
- T+1 (Feb 28, 2026): Strikes begin, IRA-NUC collapses — g-GACn: 0.089
- T+30 (Mar 27, 2026): Current state — IRA-NUC partially recovering, ELC-NUC still collapsed
- T+180 (Aug 2026): Hypothetical post-conflict regime — modelled reform scenario
Visualisation: animated line chart (Chart.js) showing additive vs. multiplicative
g-GAC trajectories across time-points, with scenario annotations.

**S2-T3 · Oman Threshold: Post-Conflict Verification Architecture**
Extend the `oman_threshold` scenario with a fourth section:
"T+180 Post-Conflict Architecture Requirements"
Pre-populate NUC indicator values for a hypothetical Iran Verification
Architecture modelled on CWC inspection protocols.
This directly supports the IAEA Safeguards Symposium November 2026 abstract.

**S2-T4 · AI Domain: DCSF NOF Addition**
The PDF mathematical intelligence document specifies a second ESI factor:
`DCSF` (Deployment Context Simulation Fidelity) that is currently missing
from the Page 1 AI NOF calculator (which has ESC but not DCSF).
Add DCSF as a second ESI NOF with indicators:
`simulation_of_sector_contexts`, `human_in_loop_realism`,
`threat_actor_diversity`, `environment_variability`

**S2-T5 · IP Sanitisation Review (Pre-Geneva)**
Full audit of all visible labels, formulas, and taxonomy strings.
Ensure all public-facing tabs conform to descriptive-only labelling policy.
Remove any remaining stratum labels, BGC acronyms, or formula weights
visible to a conference audience.

---

## Sprint 3 — Backlog
### UNIDIR AISE26 & IAEA Safeguards Submission Package
**Target version: v3.0**
**Status: 📋 Backlog**
**Conference alignment: UNIDIR AISE26 (June) · IAEA Safeguards Symposium (November)**

#### Sprint 3 Tasks

**S3-T1 · Full Canonical NOF Alignment — All 5 Domains**
Apply canonical E-AGPO-HT indicator names (from Domain Specific Mathematical
Intelligence document) to AI, Space, Biotech, and Energy domains in P3_REG,
matching what was done for Nuclear in v2.1. This ensures all 6 domains use
the published framework names, not the generic BAC structural names.

**S3-T2 · Page 1 AI Domain: Remaining PDF NOFs**
The PDF specifies 11 AI NOFs; Page 1 currently implements 10.
Add the missing `DCSF` NOF (carried from Sprint 2, S2-T4) and add
a second ESI slider grouping in the NOF Calculator.

**S3-T3 · Scenario 9 · UNIDIR AISE26 Demonstration Scenario**
Purpose-build a scenario for the UNIDIR demo:
- Title: "AI Governance Fragmentation: Three-Regime Divergence"
- Models simultaneous fragmentation across EU AI Act, US NIST, and China's
  AI governance framework — with cross-domain implications for Nuclear AI
  systems (linking standards_diverge and ai_nuclear scenarios)
- This is a compound entanglement scenario, aligned with the BLIND EYE /
  SILENT VECTOR seed scenarios from the Auracelle compound domain portfolio

**S3-T4 · Wargaming Demo: Iran 2026 Country Profile**
Add "Iran (Oman Threshold 2026)" as a named country profile in the
Nuclear domain country selector, with NOF values pre-seeded from
the Oman Threshold scenario indicator vectors:
- DOC-NUC: 0.32, ELC-NUC: 0.28, IRA-NUC: 0.07, CLB-NUC: 0.24
This enables live country comparison (e.g. Iran vs Generic State)
in the wargaming panel, demonstrating governance gap quantification.

**S3-T5 · SAS-219 Integration Layer**
Add a NATO SAS-219 Winter Storm 2030 scenario to the Scenario Library:
- Aligned with R5 (Digitally Wargaming) and R6 (Wargaming Definition)
  subgroup contributions
- Models High North governance failure scenarios for AI-enabled
  decision-making under Arctic conditions
- Governance capacity as through-line connecting all sub-scenarios

**S3-T6 · Export-Controlled Version Flag**
Add a build flag to generate two versions:
- `_proprietary_demo.html` — full IP (current)
- `_public_demo.html` — sanitised for conference/public display
  with descriptive labels only, no taxonomy acronyms, no formula weights

---

## Institutional Alignment Summary

| Sprint | Version | Target Deadline | Conference |
|---|---|---|---|
| Sprint 1 | v2.2 | April 2026 | IAEA Safeguards 2026 (abstract) |
| Sprint 2 | v2.3 | May 2026 | Geneva Cyber Week (Orion presenting) |
| Sprint 3 | v3.0 | June 2026 | UNIDIR AISE26 · GESDA Science Diplomacy Week |
| Post-v3 | TBD | October 2026 | IAEA Safeguards Symposium (November) |

---

## Version History Reference

| Version | Date | Key Addition |
|---|---|---|
| v1.0 | Pre-Mar 2026 | Base dual-page E-AGPO/E-AGSO instrument |
| v2.0 | Mar 2026 | P3 wargaming engine · Oman Threshold scenario · Lyra 2.0 |
| v2.1 | Mar 2026 | Canonical E-AGPO-HT Nuclear NOFs (NUC_01–NUC_10) · TCTR-NUC · ITDB scenario |
| v2.1.1 | Mar 27, 2026 | JS SyntaxError fix · State Formula IP removal |
| **v2.2** | **Apr 2026** | **Sprint 1 — NUC_11 · Package Protection · Scrap Metal Pathway** |
| v2.3 | May 2026 | Sprint 2 — Time-series · QTM/NUC cross-domain · DCSF |
| v3.0 | Jun 2026 | Sprint 3 — UNIDIR package · Full canonical alignment · SAS-219 |

---

*Auracelle AI Governance Labs · Director G.A. Evans*
*E-AGPO-HT / E-AGSO-HT Framework · Proprietary IP · All rights reserved*
*BSU Doctoral Research · NATO STO SAS-219 · UC Berkeley CLTC*
