# Equity Research Coverage Initiation — Project README

**Project type:** Sell-side workflow documentation and LLM capability analysis  
**Scope:** Full initiation lifecycle, from coverage trigger to ongoing maintenance  
**Steps:** 86 work steps · 5 decisions · 7 phases · 8 professional roles · ~8–10 weeks  
**Regulatory framework:** FINRA Rule 2241 · Reg AC · SEC Reg FD  

---

## Contents

1. [Project Overview](#1-project-overview)
2. [Workflow Summary — 7 Phases](#2-workflow-summary--7-phases)
3. [Step Inventory by Phase](#3-step-inventory-by-phase)
4. [Roles and Responsibilities](#4-roles-and-responsibilities)
5. [LLM Capability Classification](#5-llm-capability-classification)
6. [Quality Gates](#6-quality-gates)
7. [Regulatory Reference](#7-regulatory-reference)
8. [Color Palette — Master Reference](#8-color-palette--master-reference)
9. [Deliverables Index](#9-deliverables-index)
10. [Key Terms Glossary](#10-key-terms-glossary)

---

## 1. Project Overview

Equity research initiation is the formal process by which a sell-side analyst launches coverage on a public company, producing a comprehensive initiation report that includes a rating (Buy / Hold / Sell), a 12-month price target, an investment thesis, detailed financial model, and risk factors.

The process is heavily regulated. FINRA Rule 2241 governs all aspects of sell-side research, mandating IB firewall separation, supervisory review before publication, Reg AC independence certification, and simultaneous equal-access distribution to all clients. No step in the process — from the initial conflict check to the final distribution — can bypass the compliance framework.

This project documents the full initiation process as a structured workflow: 86 numbered steps across 7 phases, mapped to 8 professional roles in a RACI matrix, rendered as interactive flowcharts, and classified for LLM capability.

---

## 2. Workflow Summary — 7 Phases

| # | Phase | Steps | Weeks | Primary Owner |
|---|-------|-------|-------|---------------|
| P1 | Approval & Scoping | 8 | 1–2 | Lead Analyst + Research Director + Compliance |
| P2 | Research & Due Diligence | 16 | 2–6 | Lead Analyst + Associate |
| P3 | Financial Modeling | 16 | 4–7 | Lead Analyst + Associate |
| P4 | Report Writing | 11 | 6–9 | Lead Analyst |
| P5 | Review & Compliance | 13 | 8–10 | Supervisory Analyst + Compliance |
| P6 | Publication & Distribution | 8 | 10 | Production + Compliance + Sales |
| P7 | Post-Publication & Maintenance | 14 | Ongoing | Lead Analyst + Sales Force |
| — | **Total** | **86** | **~8–10 weeks** | — |

> **Note:** Steps include 4 formal decision nodes (IB conflict screen, rating committee pre-approval, rating committee final vote, and annual coverage continuation decision) and 1 milestone (coverage trigger). The 82 remaining are action steps.

---

## 3. Step Inventory by Phase

### Phase 1 — Approval & Scoping (Steps 1–8)

| # | Node ID | Type | Description |
|---|---------|------|-------------|
| 1 | Milestone_CoverageTrigger | MILESTONE | Coverage opportunity identified by analyst |
| 2 | Analyst_SubmitCoverageRequest | ACTION | Analyst submits formal coverage request to Research Director |
| 3 | Compliance_InitiateWallCheck | ACTION | Compliance initiates IB conflict and restricted list screen |
| 4 | Decision_IBConflict | DECISION | IB conflict determination — proceed or block |
| 5 | RD_ApproveCoverage | ACTION | Research Director approves sector, company, analyst assignment |
| 6 | Compliance_RegisterCoverage | ACTION | Analyst and associate registered; trading restrictions applied |
| 7 | Analyst_DefineCoverageScope | ACTION | Coverage universe defined; peer group of 8–15 names selected |
| 8 | RD_AllocateBudgetTimeline | ACTION | Budget allocated; 8–10 week timeline set |

### Phase 2 — Research & Due Diligence (Steps 9–24)

| # | Node ID | Type | Description |
|---|---------|------|-------------|
| 9 | Assoc_DownloadSECFilings | ACTION | Download all SEC filings — 10-K, 10-Q, 8-K, proxy |
| 10 | Assoc_BuildTranscriptLibrary | ACTION | Compile earnings call transcript library — 5+ years |
| 11 | Assoc_CompilePriorResearch | ACTION | Compile any prior sell-side coverage |
| 12 | Assoc_GatherIndustryData | ACTION | Aggregate third-party industry reports (Gartner, IBISWorld) |
| 13 | Analyst_IntroCallWithIR | ACTION | Introductory call with Investor Relations |
| 14 | Analyst_RequestMgmtMeeting | ACTION | Request C-suite management meeting |
| 15 | Analyst_ConductCSuiteMeeting | ACTION | CEO / CFO / COO deep-dive meeting |
| 16 | Analyst_SegmentHeadMeetings | ACTION | Segment head meetings for business unit detail |
| 17 | Compliance_PreClearExpertCalls | ACTION | Compliance pre-clears expert calls — MNPI screen |
| 18 | Analyst_ConductExpertCalls | ACTION | GLG / Gerson Lehrman expert calls — former executives |
| 19 | Assoc_ConductChannelChecks | ACTION | Channel checks — distributors, customers, competitors |
| 20 | Analyst_AttendConferences | ACTION | Industry conference one-on-one meetings |
| 21 | Assoc_PortersFiveForces | ACTION | Porter's Five Forces framework |
| 22 | Assoc_MarketSizing | ACTION | TAM / SAM / SOM market sizing model |
| 23 | Analyst_MoatAnalysis | ACTION | Economic moat and competitive advantage analysis |
| 24 | Assoc_PeerBenchmarking | ACTION | Peer group benchmarking — 8–15 comparable companies |

### Phase 3 — Financial Modeling (Steps 25–40)

| # | Node ID | Type | Description |
|---|---------|------|-------------|
| 25 | Assoc_CreateMasterWorkbook | ACTION | Associate creates master Excel workbook structure |
| 26 | Assoc_BuildHistoricalIS | ACTION | 5-year historical income statement extraction |
| 27 | Assoc_BuildHistoricalBS | ACTION | Balance sheet extraction — 5 years |
| 28 | Assoc_BuildHistoricalCF | ACTION | Cash flow statement extraction — 5 years |
| 29 | Analyst_NormalizeOneTimeItems | ACTION | Non-GAAP normalization and one-time item adjustments |
| 30 | Analyst_BuildRevenueProjections | ACTION | Revenue projection model — segment-level drivers |
| 31 | Analyst_BuildMarginProjections | ACTION | Margin projection model — gross, EBITDA, net |
| 32 | Assoc_BuildFCFModel | ACTION | Free cash flow model with capex and working capital |
| 33 | Analyst_PopulateSectorKPIs | ACTION | Sector-specific KPI model (depends on industry) |
| 34 | Analyst_BuildDCF | ACTION | DCF model with WACC and terminal value |
| 35 | Assoc_BuildTradingComps | ACTION | EV/EBITDA and P/E trading comps table |
| 36 | Assoc_BuildPrecedentTransactions | ACTION | Precedent transaction multiples table |
| 37 | Analyst_BuildSensitivityAnalysis | ACTION | Sensitivity analysis — Bull / Base / Bear scenarios |
| 38 | Analyst_DerivePriceTarget | ACTION | Price target derivation and methodology memo |
| 39 | RD_AssignRating | ACTION | Research Director assigns provisional rating |
| 40 | Decision_RatingCommittee | DECISION | Rating committee pre-approval — proceed to report writing |

### Phase 4 — Report Writing (Steps 41–51)

| # | Node ID | Type | Description |
|---|---------|------|-------------|
| 41 | Assoc_WriteCompanyOverview | ACTION | Company overview and business model section |
| 42 | Assoc_WriteIndustrySection | ACTION | Industry and market structure section |
| 43 | Analyst_WriteCompetitivePositioning | ACTION | Competitive positioning and moat analysis section |
| 44 | Assoc_WriteHistoricalFinancials | ACTION | Historical financials exhibit and narrative |
| 45 | Analyst_WriteForwardFinancials | ACTION | Forward financial estimates section |
| 46 | Analyst_WriteValuationSection | ACTION | Valuation methodology and price target section |
| 47 | Analyst_WriteInvestmentThesis | ACTION | Investment thesis — variant view vs consensus |
| 48 | Analyst_WriteCatalysts | ACTION | Catalyst map — near-term and long-term events |
| 49 | Analyst_WriteRiskFactors | ACTION | Risk factors — regulatory, operational, financial |
| 50 | Assoc_BuildAllExhibits | ACTION | All charts, tables, comp tables, and valuation bridges |
| 51 | Analyst_WriteExecutiveSummary | ACTION | Executive summary — rating, PT, thesis synopsis |

### Phase 5 — Review & Compliance (Steps 52–64)

| # | Node ID | Type | Description |
|---|---------|------|-------------|
| 52 | Analyst_SubmitDraftForReview | ACTION | Complete draft submitted to Supervisory Analyst |
| 53 | SupAn_LineByLineReview | ACTION | Line-by-line factual accuracy review — FINRA 2241(b)(1) |
| 54 | SupAn_ModelAudit | ACTION | Model audit — assumptions and arithmetic checked |
| 55 | SupAn_RatingConsistencyCheck | ACTION | Rating and PT consistency with model verified |
| 56 | Compliance_ReScreenIBWall | ACTION | IB wall re-screened prior to publication |
| 57 | Compliance_GenerateDisclosures | ACTION | FINRA 2241 disclosures generated |
| 58 | Analyst_RegACCertification | ACTION | Reg AC certification signed by analyst |
| 59 | Compliance_FINRA2241Checklist | ACTION | Full FINRA 2241 compliance checklist completed |
| 60 | RD_ConveneRatingCommittee | ACTION | Research Director convenes rating committee |
| 61 | RD_ChallengeSession | ACTION | Formal challenge session on thesis and rating |
| 62 | RD_FormalVote | ACTION | Formal rating vote recorded |
| 63 | Decision_RatingApproved | DECISION | Rating approved — proceed to publication |
| 64 | Analyst_FactualReviewWithIR | ACTION | Factual review with Company IR — thesis/rating not disclosed |

### Phase 6 — Publication & Distribution (Steps 65–72)

| # | Node ID | Type | Description |
|---|---------|------|-------------|
| 65 | SupAn_SubmitToProduction | ACTION | Supervisory Analyst submits approved draft to Production |
| 66 | Prod_FormatReport | ACTION | Production team applies firm template and formatting |
| 67 | Compliance_AppendBoilerplate | ACTION | Legal boilerplate, disclosures, and Reg AC appended |
| 68 | Prod_FinalPDFQC | ACTION | Final PDF quality control pass |
| 69 | Prod_SimultaneousDistribution | ACTION | Simultaneous equal-access distribution — Bloomberg / Refinitiv / FactSet |
| 70 | Assoc_IBESEstimateUpload | ACTION | IBES / consensus estimate upload |
| 71 | Compliance_RegulatoryFilings | ACTION | FINRA regulatory filings if required |
| 72 | Analyst_SalesMorningCall | ACTION | Analyst presents on sales force morning call |

### Phase 7 — Post-Publication & Maintenance (Steps 73–86)

| # | Node ID | Type | Description |
|---|---------|------|-------------|
| 73 | Sales_DistributeSalesMemo | ACTION | Sales force distributes sales memo and talking points |
| 74 | Analyst_SalesDeskCalls | ACTION | Analyst takes sales desk calls and Q&A |
| 75 | Sales_ArrangeRoadshow | ACTION | Sales arranges client NDR / roadshow logistics |
| 76 | Analyst_PMOneonOneMeetings | ACTION | Portfolio manager one-on-one meetings |
| 77 | Analyst_GroupPresentations | ACTION | Group calls and conference presentations |
| 78 | Analyst_EarningsPreviewNote | ACTION | Earnings preview note — pre-quarter |
| 79 | Analyst_EarningsDayFlash | ACTION | Earnings day flash note — same day |
| 80 | Assoc_PostEarningsModelUpdate | ACTION | Post-earnings model update |
| 81 | Analyst_CatalystNote | ACTION | Catalyst-driven note on material events |
| 82 | Analyst_RatingChange | ACTION | Rating or price target change — full compliance re-cycle |
| 83 | Analyst_SectorUpdateNote | ACTION | Sector or industry update note |
| 84 | RD_AnnualCoverageReview | ACTION | Annual coverage review by Research Director |
| 85 | Decision_ContinueCoverage | DECISION | Continue or discontinue coverage decision |
| 86 | Analyst_DropCoverageNote | ACTION | Coverage discontinuation note published |

---

## 4. Roles and Responsibilities

Eight professional roles participate in the initiation process. Colors are from the CBF (colour-blind-friendly) scientific palette and are consistent across all project deliverables.

| Role | Hex | Steps (R) | Primary Responsibilities |
|------|-----|-----------|--------------------------|
| Lead Analyst | `#0072B2` | 36 | Investment thesis, valuation, report authoring, client-facing |
| Associate | `#E69F00` | 21 | Data gathering, model build, exhibit construction, section drafts |
| Research Director | `#56B4E9` | 7 | Coverage approval, rating committee, sign-off authority |
| Supervisory Analyst | `#009E73` | 4 | FINRA 2241 line review, model audit, production handoff |
| Compliance | `#F0E442` | 10 | IB wall checks, FINRA 2241 checklist, Reg AC, disclosures |
| Sales Force | `#D55E00` | 2 | NDR logistics, client distribution, morning call support |
| Production / Layout | `#CC79A7` | 3 | Formatting, PDF production, boilerplate append |
| Portfolio Mgr (Client) | `#667085` | 0 | Recipient of research; NDR meetings; feedback channel |

> **RACI convention:** R = Responsible (does the work) · A = Accountable (owns the outcome) · C = Consulted · I = Informed. The step counts above reflect R assignments only.

---

## 5. LLM Capability Classification

Each step is classified into one of four categories based on whether an LLM can fully execute it, needs human oversight, requires human judgment, or depends on external parties.

| Category | Count | % | Definition |
|----------|-------|---|------------|
| 🟢 **GREEN — Fully LLM-Capable** | 30 | 35% | Extraction, verification, calculation, standard formatting. LLM can execute autonomously with minimal review. |
| 🟡 **YELLOW — Hybrid** | 28 | 33% | Analysis, projection modeling, narrative drafting. LLM produces draft; analyst reviews and takes ownership. |
| 🟠 **ORANGE — Human-Required** | 18 | 21% | Management meetings, expert calls, investment judgment calls, regulatory certifications. Cannot be delegated to LLM. |
| ⬜ **GRAY — External / Regulatory** | 10 | 11% | Distribution platforms, FINRA filings, client actions, trading restriction enrollment. Governed by third-party systems. |

**LLM leverage is highest in Phases 2, 3, and 4** — research aggregation, model build, and exhibit construction. It is lowest in Phase 5 (compliance and review) and Phase 7 (client relationship management), where human judgment and regulatory accountability are non-delegable.

---

## 6. Quality Gates

Four formal gates exist in the workflow. No phase may proceed without the preceding gate being cleared.

| Gate | Location | Cleared By | Condition |
|------|----------|------------|-----------|
| **Gate 1 — IB Wall Confirmed** | P1 → P2 | Compliance + Research Director | No active mandate conflict; analyst registered; trading restrictions applied |
| **Gate 2 — Model Sign-Off** | P3 → P4 | Research Director | Model logic, scenario assumptions, and PT methodology approved |
| **Gate 3 — Compliance Sign-Off** | P5 → P6 | Supervisory Analyst + Compliance | FINRA 2241 checklist complete; Reg AC signed; rating committee vote recorded |
| **Gate 4 — Distribution Confirmed** | P6 → P7 | Compliance | Simultaneous equal-access distribution to all clients verified per FINRA 2241(b)(2)(D) |

---

## 7. Regulatory Reference

| Rule / Regulation | Issuing Body | Key Requirement |
|-------------------|-------------|-----------------|
| **FINRA Rule 2241** | FINRA | Governs all sell-side research. Mandates IB firewall separation, supervisory review, Reg AC, equal-access distribution, and rating disclosure. |
| **Reg AC** | SEC | Analyst must certify in writing that report reflects their independent views. No pre-release to banking, IR, or subject company. |
| **SEC Reg FD** | SEC | Prohibits selective disclosure. Applies to management meetings — no material non-public information may be transmitted from company to analyst. |
| **MNPI rules** | SEC | Material Non-Public Information cannot be used in research. Expert call compliance pre-clearance required at most firms. |
| **Exchange Act §15** | SEC | Establishes IB firewall requirements between research and investment banking. |
| **IBES / Consensus upload** | LSEG / Refinitiv | Associate uploads estimate model to IBES for consensus tracking post-publication. |

---

## 8. Color Palette — Master Reference

All colors are consistent across the PPTX slide, RACI matrix, and all HTML files.

### Phase Colors

| Phase | Color Name | Hex | Usage |
|-------|-----------|-----|-------|
| P1 — Approval & Scoping | Dark Navy | `#1F3864` | Phase tab, left border, header badge |
| P2 — Research & DD | Dark Forest | `#1A4D3A` | Phase tab, left border, header badge |
| P3 — Financial Modeling | Dark Amber | `#7B4F00` | Phase tab, left border, header badge |
| P4 — Report Writing | Dark Purple | `#3D1A66` | Phase tab, left border, header badge |
| P5 — Review & Compliance | Dark Crimson | `#6B0E1E` | Phase tab, left border, header badge |
| P6 — Publication | Dark Teal | `#004D4D` | Phase tab, left border, header badge |
| P7 — Post-Publication | Dark Slate | `#2D3748` | Phase tab, left border, header badge |

### Role Colors (CBF Scientific Palette)

| Role | Hex | Notes |
|------|-----|-------|
| Lead Analyst | `#0072B2` | CBF Blue |
| Associate | `#E69F00` | CBF Orange |
| Research Director | `#56B4E9` | CBF Sky Blue |
| Supervisory Analyst | `#009E73` | CBF Teal |
| Compliance | `#F0E442` | CBF Yellow |
| Sales Force | `#D55E00` | CBF Vermilion |
| Production / Layout | `#CC79A7` | CBF Pink |
| Portfolio Mgr (Client) | `#667085` | Slate Gray |

> **Design principle:** Phase colors and role colors are deliberately distinct palettes. In the original draft, the PPTX reused role colors for phase tabs, causing visual ambiguity. The v2 documents separated them completely.

---

## 9. Deliverables Index

### Core Documents

| File | Format | Description |
|------|--------|-------------|
| `ER_flowchart_slide_v2.pptx` | PowerPoint | Single-slide summary: flowchart, role legend, LLM opportunity bars, phase tabs, key terms. For deck embedding and presentations. |
| `ER_matrix_v2.xlsx` | Excel | Full 86-step RACI matrix with phase headers, role columns (R/A/C/I), and color-coded headers. |
| `ER_html_v2.html` | HTML | Comprehensive reference document: tabbed interface with master flowchart, phase-level Mermaid diagrams, regulatory reference table, deliverable cards, and compliance checklist. |

### Workflow Chart Files

| File | Format | Description |
|------|--------|-------------|
| `ER_workflow_charts.html` | HTML | All 8 Mermaid charts in one file — Overview + P1 through P7 — with stats bar, legend, TOC, and copy-to-clipboard on each chart. Matches Maple 10K template structure. |
| `ER_P1_Approval_Scoping.html` | HTML | Standalone P1 chart with phase nav bar linking to P2–P7. |
| `ER_P2_Research_DD.html` | HTML | Standalone P2 chart with phase nav bar. |
| `ER_P3_Financial_Modeling.html` | HTML | Standalone P3 chart with phase nav bar. |
| `ER_P4_Report_Writing.html` | HTML | Standalone P4 chart with phase nav bar. |
| `ER_P5_Review_Compliance.html` | HTML | Standalone P5 chart with phase nav bar. |
| `ER_P6_Publication.html` | HTML | Standalone P6 chart with phase nav bar. |
| `ER_P7_Post_Publication.html` | HTML | Standalone P7 chart with phase nav bar. |

### Earlier Versions (superseded)

| File | Notes |
|------|-------|
| `eq_research_flowchart_slide.pptx` | v1 PPTX — phase tabs reused role colors |
| `equity_research_raci.xlsx` | v1 RACI — phase headers in gray, Portfolio Mgr in black |
| `ER_html_v2.html` / `equity_research_initiation_fixed.html` | Earlier HTML versions — role colors not CBF-aligned |

---

## 10. Key Terms Glossary

| Term | Definition |
|------|-----------|
| **Initiation** | Formal analyst coverage launch producing a rated research report with price target |
| **Reg AC** | SEC Rule 501–502 requiring analyst to certify report reflects their independent views |
| **FINRA 2241** | FINRA rule governing sell-side research analyst conflicts of interest |
| **DCF** | Discounted Cash Flow — intrinsic valuation model using projected free cash flows and WACC |
| **EV/EBITDA** | Enterprise Value to EBITDA — standard relative valuation multiple for most sectors |
| **WACC** | Weighted Average Cost of Capital — discount rate used in the DCF |
| **Reg FD** | SEC Regulation Fair Disclosure — prohibits selective disclosure of material information |
| **MNPI** | Material Non-Public Information — cannot be used in research; Reg FD and insider trading rules apply |
| **Flash note** | Rapid research update published same trading day as a material event |
| **NDR** | Non-Deal Roadshow — analyst and sales force accompany portfolio managers for one-on-one meetings with company management; no capital raise involved |
| **Buy / Hold / Sell** | Standard three-tier sell-side rating scale (some firms use Overweight / Equal-weight / Underweight) |
| **Comp table** | Comparable company trading multiples table — EV/EBITDA, P/E, P/FCF for peer group |
| **IB wall** | Information barrier between investment banking and research; required by FINRA 2241(b)(2) |
| **IBES** | Institutional Brokers' Estimate System (LSEG/Refinitiv) — consensus earnings estimate database |
| **Football field** | Multi-methodology valuation summary chart showing range of values across DCF, comps, and precedents |
| **Series 86/87** | FINRA qualification required for research analysts; 87 permits supervisory sign-off |
