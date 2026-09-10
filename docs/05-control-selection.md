# Control selection and SoA extract

Document SOA-EXTRACT-01 · Version 1.0 · 7 September 2026

## How controls were selected

Start with business requirements, risks and necessary treatments. Then compare those needs against the Annex A reference set so relevant controls are not overlooked. Additional controls can be necessary beyond Annex A. A risk-to-control mapping alone is not a complete management system.

The [extract](../registers/soa-extract.csv) covers 21 selected controls. Each row includes a reference identifier, an original theme description, a case-specific inclusion reason, related risks, owner, status, evidence basis and expected evidence. Theme descriptions are not official control wording.

Every included row is applicable within this fictional design. The omitted Annex A controls are **not reviewed in this extract**, not excluded or declared inapplicable. No exclusion decisions are asserted. A complete SoA and Annex A comparison are future work. Outsourced hosting and remote working do not automatically justify excluding physical or supplier-related controls.

## Status vocabulary

| Status | Meaning in this release |
| --- | --- |
| Draft designed | An original planning document is populated, without real approval or deployment |
| Demonstrated in sample | A document-based exercise illustrates part of the control on synthetic data |
| Planned | Implementation or operating evidence is absent |

No control is labelled fully implemented or effective. A.5.18, A.6.5 and A.8.2 are demonstrated only within the access sample. A.5.1 and A.5.9 have drafted artifacts. Sixteen selected controls remain planned.

## Three decisions to defend

**Permission lifecycle:** R01 and R03 require current business need to drive access. A.5.18 connects approvals, periodic reviews and changes. A.6.5 connects departures to the same process. CA01 corrects one account; recurrence prevention still needs HR trigger and repeat-review evidence.

**Privileged access:** R02 warrants stricter authorization because administrative actions can affect the whole service or release chain. A.8.2 supports removing AR004's unnecessary administration and retaining AR011's authorized role. Authentication and logging plans complement it; they were not technically tested here.

**Backups and recovery:** R05 needs A.8.13 with A.5.30 because recoverability must meet business needs. Required evidence includes a timed restore and integrity checks. A document saying that backups exist is insufficient to claim the service can recover.

## Reference-check limits

Public ISO descriptions and NQA implementation guidance informed the educational structure. The exact normative wording of clauses, selected control identifiers and the complete Annex A comparison must be checked against an authorized full-text copy before real assurance use. Record unresolved points in the [reference verification backlog](../references/README.md). The full licensed standards are not included in this repository.
