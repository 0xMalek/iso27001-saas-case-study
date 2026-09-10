# Assessment and treatment decisions

Document ASSESS-01 · Version 1.0 · Baseline 1 September 2026; report 7 September 2026

## Baseline priorities

The twelve risks comprise **2 Critical, 7 High, 2 Moderate and 1 Low**. These are fictional qualitative judgments. The full [risk register](../registers/risks.csv) records event, existing safeguards, likelihood and impact reasoning, owners and conditional targets.

| Risk | Scenario | Owner | Baseline score | Band | Target estimate |
| --- | --- | --- | --- | --- | --- |
| R01 | Former employee retains ticket access | Head of Support | 16 | High | 8 |
| R02 | Unjustified privilege enables major compromise | Platform Lead | 20 | Critical | 10 |
| R03 | Role change leaves excessive ticket permissions | Head of Support | 12 | High | 8 |
| R04 | Lost laptop exposes work sessions | People and Operations Lead | 9 | Moderate | 3 |
| R05 | Backups fail to restore after corruption | Platform Lead | 20 | Critical | 8 |
| R06 | Cloud disruption interrupts customer service | Platform Lead | 12 | High | 8 |
| R07 | Unsafe release weakens tenant isolation | Head of Engineering | 15 | High | 10 |
| R08 | Supplier handles customer information improperly | People and Operations Lead | 12 | High | 8 |
| R09 | Slow incident response increases harm | Platform Lead | 12 | High | 6 |
| R10 | Exposed build secret permits production access | Platform Lead | 15 | High | 10 |
| R11 | People records shared with the wrong group | People and Operations Lead | 6 | Moderate | 3 |
| R12 | Brief public website outage delays enquiries | Sales Lead | 4 | Low | 4 |

R02 and R05 lead because privileged compromise and unproven recovery combine high exposure with severe consequences. R01 and R03 also receive early action because the synthetic access review makes those weaknesses concrete. Priorities consider severity and dependencies, not only sorting a numeric score.

## Treatment decisions

| Treatment | Risk | Decision | Target date | Status |
| --- | --- | --- | --- | --- |
| T01 | R01 | Modify | 2026-09-21 | Sample corrected; recurring process planned |
| T02 | R02 | Modify | 2026-10-07 | Sample corrected; broader controls planned |
| T03 | R03 | Modify | 2026-09-21 | Sample corrected; recurring process planned |
| T04 | R04 | Modify | 2026-10-22 | Planned |
| T05 | R05 | Modify | 2026-10-07 | Planned |
| T06 | R06 | Modify | 2026-11-06 | Planned |
| T07 | R07 | Modify | 2026-11-06 | Planned |
| T08 | R08 | Modify | 2026-10-22 | Planned |
| T09 | R09 | Modify | 2026-10-22 | Planned |
| T10 | R10 | Modify | 2026-10-07 | Planned |
| T11 | R11 | Modify | 2026-11-06 | Planned |
| T12 | R12 | Accept | 2026-12-06 | Accepted in simulation |

All eleven modification plans remain open. T01-T03 include verified sample corrections, but their recurring processes remain planned. Target ratings for R02, R07 and R10 remain High; the CEO and risk owners must decide on additional treatment or justified time-limited acceptance. The case contains no actual acceptance for those items.

[Treatment details](../registers/treatments.csv) specify actions, controls, evidence and approval authority. No technical safeguard is claimed to be deployed by this project. The roadmap sequences work while preserving responsibility for earlier containment decisions.

## Why these tradeoffs

- Restore testing precedes a broad resilience claim: a successful backup schedule cannot answer whether ticket data can be recovered.
- Reviewing privilege preserves the approved cloud administrator because the service needs accountable administration. It removes a repository role that lacks approval.
- Release controls address tenant isolation at the point where changes enter the service. General staff training alone would not test that boundary.
- Supplier review asks for responsibilities and evidence. A supplier badge alone would not prove CaseCo configured its own service safely.

## Acceptance record ACC-01

Risk: R12 / A10. Decision: accept score 4, Low, in the educational scenario. Simulated decision date: 7 September 2026. Decision role: Sales Lead. Review: 2026-12-06.

Reason: the static brochure site contains only public information and is separate from customer login and support. A brief outage delays enquiries but does not interrupt existing customer service. Managed hosting and alert review are retained; extra resilience is not prioritized over customer-data and recovery risks. No binding uptime obligation is assumed for this brochure site. If one exists, this decision must be revisited.

Trigger immediate reassessment if forms, authentication, sensitive information or greater commercial dependency are added. This is a populated simulated decision record, not a real person's signature or business approval.
