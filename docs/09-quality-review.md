# Release verification

Version 1.0 · Verification date: 7 September 2026

## Completed checks

| Area | Result |
| --- | --- |
| Source and exports | Ten assets, twelve risks, twelve dispositions and 21 selected controls reconcile to the common dataset. All ten CSV exports match source records |
| Traceability | Unique IDs, valid asset/risk/treatment/control links, owners, rating rationales and evidence requirements checked |
| Access exercise | All 27 rows reviewed; exactly three expected exceptions identified; only those three assignments changed; justified administration retained |
| Evidence quality | Missing/duplicate approval, unknown identity, duplicate account and unexpected privilege test cases detected. All six CSV evidence hashes verified |
| Workbook calculations | 64 assertions passed in Artifact Tool, including all 25 likelihood/impact combinations, missing/zero/out-of-range/fractional/text input and later-row target changes |
| Workbook export | Saved formulas, cached results, typed dates, filters, validation, conditional formatting and frozen context checked. No formula error found |
| Visual review | All eight workbook sheets reviewed across 19 rendered ranges. Both executive-report pages, all five carousel pages and the data-flow diagram inspected |
| Public presentation | 240-word LinkedIn draft; two-page report and five-page carousel; claims identify synthetic work and partial coverage |
| Navigation | Relative file links checked after final generation |

## GitHub release recheck

On 10 September 2026, the source/export, formula-cache, evidence, PDF-content and link checks were rerun successfully (1,012 assertions). The public file set excludes personal learning notes, personalized CVs, build/QA intermediates and unrelated Word documents. Public navigation uses the reusable checkpoint worksheet. The original visual-review date remains 7 September; no workbook, diagram or report layout was changed for this release.

## Validation limits

Recalculation was tested in Artifact Tool; an interactive Microsoft Excel session was not tested. CSV and PDF exports are release snapshots, not live workbook connections. Existing-row scoring changes recalculate; added rows need formulas and summary ranges extended.

This QA verifies portfolio files and the synthetic exercise. It does not validate a real company's safeguards, certify conformity, verify the full normative requirements, or assess the learner's personal competence. Complete the personal learning checkpoints before using first-person career claims. See the reference backlog for standards and real-implementation verification still required.
