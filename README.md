# NovaStar-Tech-Internal-Audit-Report | FY2025 Final Portfolio Deliverable

> A complete mock internal audit of the NovaStar Tech GRC programme (Projects 1–6), covering 10 controls, documented findings with severity ratings, a consolidated remediation tracker, and a 2-page audit report — the capstone deliverable of the full GRC portfolio.

---

## 📋 Overview

This repository is the **final deliverable** of NovaStar Tech's GRC lab series. It performs a self-audit of all six previous projects — ISO 27001 Control Matrix, Risk Register, Vendor Assessment, IR Plan, SOC 2 AWS Mapping, and Compliance Dashboard — evaluating each for design effectiveness, operating effectiveness, and documentation quality.

**Audit Opinion: NEEDS IMPROVEMENT**
3 Non-Conformances (2 High, 1 Critical) require mandatory remediation before ISO 27001 certification can be pursued.

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| [novastar_internal_audit.xlsx](https://github.com/user-attachments/files/26394041/novastar_internal_audit.xlsx) | Audit workbook — 10-control checklist + scorecard + remediation tracker |
| [novastar_internal_audit_report.docx](https://github.com/user-attachments/files/26394044/novastar_internal_audit_report.docx) | 2-page Audit Report (final portfolio deliverable) |

---

## 📊 Audit Workbook — Tab Breakdown

### 1. Audit Checklist
10 controls tested with full audit trail:

| Column | Contents |
|--------|----------|
| Audit Ref | Unique finding reference (AUD-001 to AUD-010) |
| Source Project | Which of Projects 1–6 the control comes from |
| Control / Requirement | What was tested |
| Framework Ref | ISO 27001:2022 Annex A / NIST / SOC 2 citation |
| Audit Procedure | Step-by-step testing methodology |
| Evidence Collected | Specific files, tabs, and artefacts reviewed |
| Finding Type | Non-Conformance / Minor Finding / Observation / Best Practice |
| Severity | Critical / High / Medium / Low / Info |
| Finding Details | What was found during audit |
| Action Plan | Specific remediation steps |
| Owner | Accountable role |
| Target Date | Remediation deadline |

### 2. Audit Scorecard
- Finding summary table (counts and % by type)
- Per-project effectiveness rating: Needs Work / Acceptable / Good / Excellent
- Consolidated 10-item remediation action tracker with status and owners

---

## 📄 Audit Report — Section Breakdown

| Section | Contents |
|---------|----------|
| 1. Executive Summary | Overall opinion, finding counts, verdict box |
| 2. Scope & Methodology | 10 controls selected, testing approach, findings table |
| 3. Key Findings | Deep dives on Critical/High findings + positive findings |
| 4. Overall Assessment | Audit opinion, ISO 27001 readiness trajectory |
| 5. Lessons Learned | 5 programme-wide insights |
| 6. Sign-Off | Management acknowledgement and commitment |

---

## 🔎 Audit Findings Summary

| Ref | Control | Project | Finding | Severity |
|-----|---------|---------|---------|----------|
| AUD-001 | IS Policy (A.5.1) | Project 1 | Not approved or distributed | 🔴 High |
| AUD-002 | Privileged Access (A.8.2) | Project 1 | PAM not deployed; legacy admin accounts without MFA | 🔴 Critical |
| AUD-003 | Risk Assessment (A.5.3) | Project 2 | No management sign-off on residual risks | 🟡 Medium |
| AUD-004 | Incident Response (A.5.24) | Project 2 | BCP/DRP document does not exist | 🟡 Medium |
| AUD-005 | Third-Party Risk (A.5.19) | Project 3 | Only 1 vendor assessed; no VRM programme | 🟡 Medium |
| AUD-006 | GDPR Compliance (Art. 28) | Project 3 | No ROPA; no retention schedule; no DPIA | 🔴 High |
| AUD-007 | Business Continuity (A.5.29) | Project 4 | BCP/DRP not written; backups not formally tested | 🔴 High |
| AUD-008 | SIEM / Logging (CC7.3) | Project 5 | 8-min latency vs 2-min target; log retention only 90 days | 🟡 Medium |
| AUD-009 | Vulnerability Mgmt (CC7.1) | Project 5 | No annual penetration test; no Medium CVE SLA | 🟢 Low |
| AUD-010 | Compliance Monitoring (A.5.36) | Project 6 | **Best Practice** — exceeds standard for company size | ℹ️ Info |

---

## 🏆 Project Ratings

| Project | Controls Audited | Rating | Key Strength |
|---------|-----------------|--------|-------------|
| Project 1 — ISO 27001 Controls | 2 | ❌ Needs Work | Documentation exists; deployment lags |
| Project 2 — Risk Register | 2 | ⚠️ Acceptable | Comprehensive register; needs mgmt sign-off |
| Project 3 — Vendor Assessment | 2 | ❌ Needs Work | Strong methodology; GDPR gaps |
| Project 4 — IR Plan | 2 | ⚠️ Acceptable | IRP solid; tabletop 78%; BCP missing |
| Project 5 — SOC 2 AWS | 2 | ✅ Good | Strong technical controls; SIEM latency gap |
| Project 6 — Dashboard | 1 | ⭐ Excellent | Exceeds expectations for company maturity |

---

## 🗓️ Remediation Roadmap

```
Immediate (< 30 days)
  ├── REM-001  Revoke legacy admin accounts without MFA (48h)
  └── REM-005  Fix Kinesis Firehose buffer → reduce SIEM latency

Q3 2025 (< 90 days)
  ├── REM-002  IS Policy Board approval + all-staff distribution
  ├── REM-004  Develop BCP/DRP document + DR exercise
  └── REM-007  Expand vendor risk programme to 5 critical vendors

Q4 2025
  ├── REM-003  Create GDPR ROPA + data retention schedule
  ├── REM-008  Conduct annual external penetration test
  └── REM-010  Q4 tabletop exercise — target score ≥80%

Q1 2026
  └── ISO 27001 Stage 1 Readiness Assessment (all NCs resolved)
```

---

## 📚 Audit Standards Applied

- [ISO/IEC 27001:2022 — Clause 9.2 Internal Audit](https://www.iso.org/standard/27001)
- [ISO 19011:2018 — Guidelines for Auditing Management Systems](https://www.iso.org/standard/70017.html)
- [NIST SP 800-53 Rev. 5 — Assessment Procedures](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final)
- [AICPA SOC 2 Trust Services Criteria 2017](https://www.aicpa.org/resources/landing/system-and-organization-controls-soc-suite-of-services)
- [GDPR Article 30 — Records of Processing Activities](https://gdpr-info.eu/art-30-gdpr/)

---

## 🔗 Full GRC Portfolio — All 7 Projects

| # | Project | Key Deliverable |
|---|---------|-----------------|
| 1 | ISO 27001 / NIST Control Matrix | [novacloud_compliance.xlsx](https://github.com/user-attachments/files/26394074/novacloud_compliance.xlsx) + [novacloud_compliance_summary.docx](https://github.com/user-attachments/files/26394066/novacloud_compliance_summary.docx)  |
| 2 | Risk Register (CloudNova) | [cloudnova_risk_register.xlsx](https://github.com/user-attachments/files/26394133/cloudnova_risk_register.xlsx) + [cloudnova_risk_summary.docx](https://github.com/user-attachments/files/26394107/cloudnova_risk_summary.docx) |
| 3 | Vendor Assessment (Google Workspace) | [vendor_assessment.xlsx](https://github.com/user-attachments/files/26394153/vendor_assessment.xlsx) + [vendor_assessment_report.docx](https://github.com/user-attachments/files/26394139/vendor_assessment_report.docx) |
| 4 | Incident Response Plan + Tabletop | [novastar_ir_plan.docx](https://github.com/user-attachments/files/26394165/novastar_ir_plan.docx) + [novastar_ir_workbook.xlsx](https://github.com/user-attachments/files/26394159/novastar_ir_workbook.xlsx) |
| 5 | SOC 2 AWS Controls + Artifacts | [novastar_soc2_aws.xlsx](https://github.com/user-attachments/files/26394187/novastar_soc2_aws.xlsx) + [novastar_soc2_report.docx](https://github.com/user-attachments/files/26394169/novastar_soc2_report.docx) |
| 6 | Compliance Dashboard | [novastar_compliance_dashboard.xlsx](https://github.com/user-attachments/files/26394237/novastar_compliance_dashboard.xlsx) + <img width="1600" height="1140" alt="compliance_dashboard" src="https://github.com/user-attachments/assets/ac4ca98e-f805-4ddc-b7e7-84ab89bc075e" /> |
| 7 | Internal Audit Report ← **This project** | [novastar_internal_audit.xlsx](https://github.com/user-attachments/files/26394256/novastar_internal_audit.xlsx) + [novastar_internal_audit_report.docx](https://github.com/user-attachments/files/26394254/novastar_internal_audit_report.docx)|

---

## ⚠️ Disclaimer

This is an educational GRC lab project using a fictional company. It is intended to demonstrate GRC programme documentation skills for portfolio purposes. Always consult a qualified auditor for real-world internal audits.

---

*NovaStar Tech GRC Portfolio — Project 7 of 7  ·  Built by Godwin Iduye  ·  © 2025*
