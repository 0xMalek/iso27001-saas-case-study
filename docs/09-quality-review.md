# Release verification

Version 1.0 Â· Verification date: 7 September 2026

## Completed checks

| Area | Result |
| --- | --- |
| Source and exports | Ten assets, twelve risks, twelve dispositions and 21 selected controls reconcile to the common dataset. All ten CSV exports match source records |
| Traceability | Unique IDs, valid asset/risk/treatment/control links, owners, rating rationales and evidence requirements checked |
| Access exercise | All 27 rows reviewed; exactly three expected exceptions identified; only those three assignments changed; justified administration retained |
| Evidence quality | Missing/duplicate approval, unknown identity, duplicate account and unexpected privilege test cases detected. All six CSV evidence hashes verified |
| Workbook calculations | 64 assertions passed in Artifact Tool, including all 25 likelihood/impact combinations, missing/zero/out-of-range/fractional/text input and later-row target changes |
| Workbook export | Saved formulas, cached results, typed dates, filters, validation, conditional formatting and frozen context checked. No formula error found |
| Visual review | All eight workbook sheets reviewed across 19 rendered ranges. Both executive-report pages and the data-flow diagram inspected |
| Public presentation | Two-page executive report; claims identify synthetic work and partial coverage |
| Navigation | Relative file links checked after final generation |

## GitHub release recheck

On 10 September 2026, the source/export, formula-cache, evidence and PDF-content checks passed (1,012 assertions in the original release). The interviewer-facing revision removes learning worksheets and career-publication materials from the current public tree. The unchanged workbook is now under `registers/` and the executive report under `reports/`. The replacement diagram separates customer information from staff access and deployment; it is a conceptual illustration, not an implemented architecture. Public links and evidence hashes are rechecked for this revision. Earlier publication materials may remain in Git commit history.

## Validation limits

Recalculation was tested in Artifact Tool; an interactive Microsoft Excel session was not tested. CSV and PDF exports are release snapshots, not live workbook connections. Existing-row scoring changes recalculate; added rows need formulas and summary ranges extended.

This QA verifies portfolio files and the synthetic exercise. It does not validate a real company's safeguards, certify conformity, verify the full normative requirements, or assess the learner's personal competence. See the reference backlog for standards and real-implementation verification still required.
