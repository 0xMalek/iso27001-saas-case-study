# Working registers

These registers describe CaseCo Cloud, a fictional business. The assessment baseline is 1 September 2026. Scores are case-study judgments, not observed incident frequencies.

- [Excel workbook](isms-registers.xlsx): editable inputs, calculated risk bands and linked summary.
- [Assets](assets.csv): 10 information and technology assets.
- [Risks](risks.csv): 12 risks with current ratings, rationales and conditional target ratings.
- [Treatments](treatments.csv): a decision, owner, target date and evidence requirement for every risk.
- [SoA extract](soa-extract.csv): 21 selected controls with original theme descriptions. Partial coverage; no conclusion about omitted controls.
- [Source data](source-data.json): the common source used to generate all CSV and workbook records at release.

## Editing and interpretation

IDs are stable join keys. Semicolon-separated fields reference multiple IDs. Empty action IDs mean no correction was required. Blank employment end dates mean the person is active. Dates use YYYY-MM-DD. The 25 active employees and one former employee are distinct from the 27 assigned accounts reviewed.

Workbook formula cells calculate scores and summaries. Pale yellow numeric cells are editable scoring inputs. White text/data cells can also be edited; formula cells use pale blue. The workbook is not protected. Risk acceptance requires the documented decision process and evidence; changing a score does not approve a risk.

The workbook and CSVs are synchronized release snapshots, not a live connection. For learning, edit a separate workbook copy. For a public revision, update the common source, regenerate all dependent exports and narratives, and rerun the documented checks. Do not publish conflicting workbook and CSV versions. Existing-row scoring changes recalculate; adding records requires extending tables, formulas and summary ranges.

All existing safeguards are scenario assumptions unless explicitly identified as synthetic exercise evidence. Target risk is conditional on treatment effectiveness. The three sample corrections do not establish sustained control operation and do not change the baseline risk ratings.
