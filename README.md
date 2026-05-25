# ACE-EMR Clinical System — QA Test Plan

Comprehensive quality assurance test plan for the ACE-EMR (Electronic Medical Record) Clinical System V1.0, a healthcare application replacing the legacy eSoarian system. Developed as the final project for INFO6255 (Software Quality Assurance) at Northeastern University.

## About The Project

The ACE-EMR Clinical System manages the full patient lifecycle in a dialysis care setting — from admission and insurance verification through treatments, lab orders, billing, claims processing, and weekly financial reconciliation. The system integrates with multiple external systems including eFinance, eFile_Net, TestBoston Labs, three insurance providers (United, Tufts, AARP), and the Recon_Finance Company.

This repository contains the complete QA deliverables for validating the system across all functional areas.

## Deliverables

### Business Requirements Document (BRD)
Defines 6 core requirement areas:
- **Patient Admission** — New/Existing patient onboarding with Acceptance_Flag validation and insurance verification
- **Patient Treatments** — Dialysis modalities (Hemo, Peritoneal, Palliative) with treatment location and drug pairings
- **Lab Orders & Results** — Integration with TestBoston Labs for order submission and result processing
- **Treatment & Lab Charges** — Daily charge aggregation and transmission to eFinance
- **Financial Billing & Claims** — Claims processing through United, Tufts, and AARP insurance companies
- **Reconciliation** — Weekly claims/payments reconciliation via Recon_Finance Company

### Functional Specification Document (FSD)
30+ detailed functional specifications covering every system interaction, including positive flows, negative flows, and edge cases for each requirement area.

### Test Condition Matrix
Maps all possible input combinations across patient types, acceptance flags, clinical flags, treatment locations, modalities, insurance types, and drugs.

### Test Scenarios & Cases
Complete test scenarios covering:
- Unit Testing
- Functional Testing (end-to-end business flows)
- User Acceptance Testing
- Regression Testing
- Performance Testing

### Traceability Matrix
Maps every BRD requirement → FSD specification → Test scenario to ensure full coverage.

### Test Plan
Formal QA test plan including:
- Testing strategy and objectives
- Risk assessment and mitigation
- Data approach with anonymized test data
- Entry/exit criteria
- Defect management process (Critical/High/Medium/Low severity classification)
- Environment requirements (HIPAA-compliant with RBAC, encryption, audit logging)

## Testing Methodology

- **Methodology:** Hybrid Agile/Waterfall with four 2-week sprints
- **Test Types:** Unit, Functional, UAT, Regression, Performance
- **Defect Tracking:** Spreadsheet-based with severity classification
- **Data Strategy:** Pre-configured test patients covering all condition matrix combinations with masked/anonymized sensitive data

## Team

| Name | Role |
|------|------|
| Jaimit Joshi | Test Manager |
| Anagha Godbole | Test Lead |
| Saurabh Kashyap | QA Analyst / Regression Test Lead |
| Sai Manasa | QA Analyst |
| Sai Shashank | QA Analyst / Performance Test Lead |

## Course

- **Course:** INFO6255 — Software Quality Assurance
- **Institution:** Northeastern University
- **Semester:** Spring 2026

## License

This project is available for educational and portfolio purposes.
