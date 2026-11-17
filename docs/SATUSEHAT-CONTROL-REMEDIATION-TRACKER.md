# SATUSEHAT Control Remediation Tracker
## TaranPx — Vendor SaaS

**Purpose:** Track closure of controls identified in the available Vendor SaaS assessment workbook.  
**Status basis:** The Director confirms supporting evidence is retained in company archives. This tracker does not claim independent inspection of those private files or acceptance by SATUSEHAT.

## 1. Closure workflow

For every control:
1. Locate the source evidence in the restricted company archive.
2. Confirm the evidence relates to TaranPx production and the assessment period.
3. Check that it is current, readable, complete, and does not expose unnecessary personal or patient data.
4. Record the evidence filename/reference, date, owner, and reviewer in the internal master copy.
5. Update the workbook score only if the evidence meets the workbook's exact control definition.
6. Retain approval and submission confirmation.

## 2. Control register

| Control | Requirement | Evidence reference | Closure rule |
|---:|---|---|---|
| 1 | Formal information security policy | Internal archive — map reference | Approved, versioned policy |
| 2 | Privacy policy / personal data protection | Internal archive — map reference | Final notice aligned with actual processing |
| 3 | Personnel NDA | Internal archive — map reference | Executed agreements for relevant personnel |
| 4 | IP allowlist | Internal archive — map reference | Current configuration and scope |
| 5 | Firewall/security group/ACL least privilege | Internal archive — map reference | Production configuration and review |
| 6 | Production/staging/development separation | Internal archive — map reference | Architecture/configuration evidence |
| 8 | Secure production backup | Internal archive — map reference | Secure storage, access, retention, monitoring and encryption evidence |
| 9 | Penetration test | Internal archive — map reference | Report, scope, date, remediation evidence |
| 11 | Secret management outside source code | Internal archive — map reference | Configuration and repository review |
| 14 | Secure secret storage | Internal archive — map reference | Secret-store configuration and access controls |
| 16 | Encryption at rest | Internal archive — map reference | Configuration evidence covering relevant data and backups |
| 18 | MFA for privileged accounts | Internal archive — map reference | Coverage evidence for all privileged identities, including infrastructure |
| 19 | No production data in development/testing | Internal archive — map reference | Policy plus environment/data-handling evidence |
| 20 | Personal data protection lead | Internal archive — map reference | Formal appointment and role definition |
| 21 | Centralized logging, 90-day minimum retention | Internal archive — map reference | Configuration and retention evidence |
| 22 | Sensitive-data access monitoring | Internal archive — map reference | Monitoring configuration, alerting and review evidence |
| 23 | Disaster Recovery test | Internal archive — map reference | Dated test report, results and corrective actions |
| 24 | Information security / incident response PIC | Internal archive — map reference | Formal appointment and responsibility definition |

## 3. Controls with score 1 requiring evidence review

| Control | Requirement | Review focus |
|---:|---|---|
| 7 | FHIR transaction/network logs | Completeness, retention, access restriction and payload minimization |
| 10 | Password hashing | Actual implementation and secure algorithm/configuration |
| 12 | Software component inventory | Whether dependency manifests meet the required inventory/SBOM standard |
| 13 | Secret handling in API/deployment | Repository history, secret exposure assessment and rotation evidence |
| 15 | API synchronization logs | Completeness, access restriction and sensitive-data minimization |
| 17 | Audit trail | User/action/time coverage, tamper resistance, access and retention |

## 4. Internal ownership

Assign an individual owner and reviewer for every control in the restricted master copy. Do not publish personal contact details, infrastructure diagrams, security configurations, vulnerability reports, or evidence locations in a public repository.

## 5. Submission gate

The assessment is ready for submission only when:
- The correct workbook/template and service model are confirmed.
- Every mandatory control has a supported score.
- All mandatory zero-score controls are remediated or handled according to the official assessment rules.
- Evidence is mapped and reviewed.
- Sensitive information is redacted appropriately.
- The final workbook and evidence pack are approved by the designated company reviewer.

**Important:** A management statement that evidence exists is not a substitute for mapping that evidence to each control. SATUSEHAT's review outcome remains external and cannot be pre-declared.

© PT Taran Rainmaker Group. All rights reserved.
