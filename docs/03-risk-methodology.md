# Risk assessment and acceptance method

Document RISK-METHOD-01 · Version 1.0 · Fictional baseline: 1 September 2026

## Purpose and boundaries

This project uses an original qualitative 5-by-5 method. ISO 27001 does not prescribe this matrix or these thresholds. The assessment considers a 12-month planning horizon and the existing safeguards assumed in the scenario. Current ratings are therefore baseline ratings with those safeguards considered, not ratings for a control-free environment.

Identify the asset or process, threat event, enabling weakness and business consequence. Assign a business risk owner. Record existing safeguards and their evidence quality. Select likelihood and impact separately, record the reasoning and calculate score = likelihood × impact. Compare against appetite before choosing a treatment.

## Likelihood rubric

| Score | Label | Case-study interpretation over the planning horizon |
| --- | --- | --- |
| 1 | Rare | Exceptional exposure path with consistent, demonstrated prevention assumed after treatment |
| 2 | Unlikely | Credible but infrequent opportunity; preventive arrangements make successful occurrence less likely |
| 3 | Possible | Ordinary opportunities exist and safeguards are incomplete or inconsistently applied |
| 4 | Likely | Recurring exposure and a material weakness or a demonstrated exception make occurrence credible |
| 5 | Very likely | Persistent exposure with repeated relevant events or effectively absent prevention |

These labels express judgment, not statistical probabilities. A control exception supports an exposure judgment; it does not prove a data breach occurred. Target score 1 assumes the specified safeguards are demonstrated. Without that evidence, do not apply the target rating.

## Impact rubric

Use the highest relevant consequence across confidentiality, integrity, availability and contractual/business harm. Do not average away a severe dimension. Service durations are illustrative anchors; scope and information sensitivity can justify a higher category.

| Score | Label | Illustrative consequence |
| --- | --- | --- |
| 1 | Minimal | Easily corrected internal inconvenience; no sensitive disclosure or customer interruption |
| 2 | Minor | Limited non-core interruption under four hours; small business inconvenience and no restricted-data disclosure |
| 3 | Material | Bounded sensitive-record exposure or localized disruption; substantial internal response needed |
| 4 | Major | Significant customer information exposure, multi-customer disruption or serious contractual response |
| 5 | Severe | Broad tenant compromise, extended all-customer outage, irrecoverable core data or threat to business continuity |

## Bands and authority

| Score | Band | Required decision in this case |
| --- | --- | --- |
| 1-4 | Low | Risk owner may accept with rationale, review date and confirmation that obligations are satisfied |
| 5-9 | Moderate | Risk owner must document treatment or justified acceptance; GRC reviewer checks rationale and evidence |
| 10-16 | High | Escalate to CEO and risk owner; treatment plan required, with any temporary acceptance explicitly time-limited |
| 17-25 | Critical | Immediate leadership escalation and containment decision; acceptance is exceptional and requires CEO and owner approval |

No row becomes accepted merely because a target score is within a band. All risk owners must approve their treatment plans and residual-risk acceptance when supported by evidence. Nothing in this method permits waiver of binding legal or contractual duties.

For the simulation, R12 has a documented low-risk acceptance. All other treatment approvals and residual acceptance remain pending. High and Critical baseline items require a day-0 leadership decision and immediate containment prioritization; the roadmap dates are completion targets, not permission to leave exposure unaddressed until then.

## Treatment and remaining risk

Options considered are modify exposure, avoid the activity, share some consequences, or accept the risk. Most selected treatments modify likelihood or impact. Outsourcing or insurance does not remove CaseCo's accountability. Avoidance was not chosen for core service risks because it would stop the business service; sharing alone would not address unauthorized access or recoverability.

Target likelihood and impact are separate estimates conditional on successful treatment. Keep impact unchanged unless the action plausibly limits the consequence: tested recovery can limit outage/data-loss impact for R05; exercised containment can limit duration for R09. R02, R07 and R10 remain High even at their targets and need further leadership decisions. Do not report the difference between ordinal scores as a percentage risk reduction or financial saving.

## Worked example: R01

A04 entitlement records show AR027 enabled for E026 after departure. Manual offboarding without reconciliation makes recurrence credible: likelihood 4. Ticket disclosure could materially affect customers: impact 4. The baseline score is 16, High. T01 addresses the HR-to-system handoff and evidence. A verified recurring process is estimated to lower likelihood to 2 while impact remains 4, giving target 8. Correcting one synthetic row alone does not justify applying that target.

## Review and uncertainty

Score with asset owners, compare similar scenarios and challenge inconsistent reasoning. Missing evidence is recorded as uncertainty rather than silently treating a control as effective. Reassess at least quarterly, following serious incidents and material changes. Changes to criteria must be versioned and relevant risks rescored for comparability.

The Excel workbook calculates scores and bands and flags missing or invalid 1-5 integer inputs. It does not automate acceptance. The final release checks include all rating combinations, missing inputs and changes to a later risk row.
