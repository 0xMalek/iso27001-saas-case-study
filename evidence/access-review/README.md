# Access review exercise: REV-01

**All identities, approvals, actions and dates are synthetic. No live account was changed.**

The fictional HR roster contains 25 active staff and one departed employee. The access population contains 27 assigned human accounts across CloudConsole, SourceHub and SupportDesk. People without an account in these three systems remain in the roster. Every supplied access row was reviewed; this is not proof that a real system export is complete.

## Evidence sequence

1. Read the [procedure](../../docs/06-access-review-procedure.md).
2. Compare [people](people.csv), [approved access](approvals.csv) and the [before snapshot](access-before.csv), dated 1 September 2026.
3. Make your own decisions before opening the [completed review](review-decisions.csv).
4. Read the [corrective actions](corrective-actions.csv). Immediate corrections and systemic corrective actions have separate statuses.
5. Compare the [after snapshot](access-after.csv), dated 3 September, with the original population and approvals.
6. Read the [follow-up report](follow-up.md) and [file manifest](manifest.json).

Source snapshots are retained so a reader can repeat the reasoning. The manifest detects accidental file changes; a hash does not establish the authenticity of fictional evidence.

## Completed results

| Access ID | Person | Finding | Decision | Action |
| --- | --- | --- | --- | --- |
| AR004 | E004 | Unjustified administrator | Downgrade | CA02 |
| AR024 | E021 | Role mismatch | Downgrade | CA03 |
| AR027 | E026 | Departed user active | Disable | CA01 |

AR011 / E011 is the approved CloudConsole administrator. AP011 records independent CEO approval and a valid period. Retaining it shows that necessary privilege is evaluated on business need.

All 24 other rows were retained, including AR011. Three entitlement changes were verified in revised synthetic records. The recurring preventive measures remain planned, and their effectiveness has not been tested.
