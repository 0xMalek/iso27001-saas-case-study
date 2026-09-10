# Follow-up verification: REV-01

Version 1.0. Synthetic review date: 3 September 2026. Reviewer role: GRC Reviewer. Scenario verification is distinct from the file QA performed on 7 September.

| Action | Original condition | Revised condition | Verification | Wider corrective action |
| --- | --- | --- | --- | --- |
| CA01 / AR027 | Departed E026 remained enabled as SupportDesk Agent | Same account retained in the record, enabled = No | Reconciled to HR end date and expired approval; correction verified in synthetic data | Recurring leaver reconciliation planned |
| CA02 / AR004 | E004 held SourceHub Administrator; only Developer approved | Developer, enabled = Yes | Role matches AP004; correction verified in synthetic data | Privilege-approval enforcement planned |
| CA03 / AR024 | Sales employee E021 held SupportDesk Agent; Viewer approved | Viewer, enabled = Yes | Role matches AP024; correction verified in synthetic data | Role-change reconciliation planned |
| Retained / AR011 | E011 held approved CloudConsole Administrator | Administrator, enabled = Yes | AP011 was approved by CEO and valid at both snapshots | Periodic privileged review remains planned |

## Population reconciliation

- 27 unique access IDs before and 27 after. No row was dropped to conceal an exception.
- 26 enabled accounts after correction; the departed account remains recorded as disabled.
- 24 assignments were unchanged. Exactly three assignments changed role or enabled status.
- Every enabled account in the after snapshot belongs to an active employee, matches a valid approval and uses the approved role.
- No orphaned person ID, duplicate person/system assignment, missing approval or unexpected entitlement change was found by the file checks.

## Interpretation

This is a completed document-based exercise on supplied synthetic records. A real review would also establish export completeness, disable sessions/tokens where needed, inspect activity, validate changes in each live system, and test the recurring process over time. The fixture does not demonstrate MFA deployment, technical revocation, incident investigation, or ISO conformity.

The immediate corrections are verified within this exercise. CA01-CA03 remain open for systemic action and effectiveness review. R01-R03 retain their baseline ratings; future targets need broader implementation evidence and risk-owner acceptance.
