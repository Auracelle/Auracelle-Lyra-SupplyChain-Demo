# Changelog — Auracelle Lyra · Checks and Balances

All notable changes to this build are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [2.1] — March 2026

### Nuclear Domain — Canonical E-AGPO-HT Alignment
- Replaced generic NUC_01–NUC_07 NOF labels with canonical E-AGPO-HT framework names
  from the Domain Specific Mathematical Intelligence specification
- Nuclear domain now contains 10 canonical NOFs (NUC_01–NUC_10):
  - NUC_01: Anomaly Detection Sensitivity (ADS-NUC) → BAC02
  - NUC_02: Declared-vs-Observed Consistency (DOC-NUC) → BAC02
  - NUC_03: Safeguards Coverage Completeness (SCC) → BAC01
  - NUC_04: Access Realism Index (ARI-NUC) → BAC01
  - NUC_05: Red-Team Evasion Robustness (RTER-NUC) → BAC03
  - NUC_06: Escalation Ladder Clarity (ELC-NUC) → BAC05
  - NUC_07: Credibility-Legitimacy Balance (CLB-NUC) → BAC06
  - NUC_08: Inspection Resource Adequacy (IRA-NUC) → BAC04
  - NUC_09: Technical Complexity Adaptation (TCA-NUC) → BAC07
  - NUC_10: Transport Chain & Recovery (TCTR-NUC) → BAC03 (new)
- Updated P3_STARTERS.Nuclear with all canonical indicator names and calibrated values
- Renamed transport NOF from NUC_08/TCA-NUC to NUC_10/TCTR-NUC to avoid
  collision with canonical TCA-NUC (Technical Complexity Adaptation)

### Scenario Library — 7th Scenario Added
- ITDB Transport Vulnerability (Nuclear · ITDB tag)
  - Scores TCTR-NUC (NUC_10) against IAEA ITDB March 2026 factsheet data
  - g-ARI delta: -0.094
  - 4-point reform pathway across all TCTR-NUC indicators
  - Aligned to IAEA International Conference on Safe and Secure Transport
    of Nuclear and Radioactive Material (Vienna, March 23-27, 2026)
  - Applicable to UNIDIR AISE26 submission

### Mathematical Intelligence
- All Nuclear NOF indicator names now match the canonical E-AGPO-HT taxonomy
  from the Domain Specific Mathematical Intelligence document (Jan 27, 2026)
- STI/SAD/ESI/NDM/SRA/IIC/ASI → BAC01–BAC07 mapping fully documented
- Oman Threshold scenario NOF vectors (DOC-NUC, ELC-NUC, IRA-NUC, CLB-NUC)
  now reference canonical indicator names

---

## [2.0] — March 2026

### Identity & Branding
- Header monogram updated from "AL" to Lyra 2.0
- File renamed to Auracelle_Lyra_Checks_and_Balances_Proprietary_Demo.html
- Repository established as standalone proprietary demo build

### Wargaming Demo Engine (P3)
- Complete P3 wargaming engine as primary Page 1 mode
- Seven tabs: Game State, Registry Scoring, BGC Engine, Governance Network,
  Compliance Convergence, Proliferation Pathways, Actions & Shocks
- Six domain selector: Nuclear, AI, Space, Biotech, Renewable, Quantum
- Three.js 3D Governance Neural Network per domain (7 actor nodes)
- Three.js 3D Compliance Convergence animation (20 real safeguards actors)
- g-GWC master strip with Stratum I to III scoring chain
- BGC Engine with 7 adjustable sliders (STI/SAD/ESI/NDM/SRA/IIC/ASI)
- Actions & Shocks panel: 8 governance interventions with cascade effects
- Proliferation Pathways: domain-specific weakness mapping

### Scenario Library — Oman Threshold (6th Scenario)
- Oman Threshold: Diplomatic Collapse & Nuclear Assurance Failure (Feb 2026)
  - Tag: Crisis · Live (sc-crisis, red)
  - g-ARI delta: -0.231 (largest negative impact in library)
  - Full NOF indicator vectors from open-source evidence (Feb 26-28, 2026)
  - Additive vs. multiplicative g-GAC comparison (0.412 vs. 0.089)
  - 12-point post-conflict verification architecture reform pathway

---

## [1.0] — Prior to March 2026

### Initial Build (auracelle_lyra_v3.html)
- Dual-page: E-AGPO (Policy Metrics) and E-AGSO (Assurance Stress-Test)
- Page 1: AI domain NOF Calculator, Results Table, Stratum View, Optimizer
- Page 1: Document upload with Anthropic API scoring integration
- Page 2: Audit Evasion, Assurance NOFs, CoK, Scenario Library (5 scenarios)
- Page 2: Country wargaming (8 countries), Regime comparison (6 regimes)
- Anthropic API integration for wargame and regime narrative generation

---

Auracelle AI Governance Labs · Copyright 2026 Grace-Alice Evans
