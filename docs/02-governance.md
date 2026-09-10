# Governance, policy and security objectives

Document GOV-01 · Version 1.0 · 7 September 2026 · Draft for a fictional company

## Proposed information security policy

CaseCo Cloud will protect the confidentiality, integrity and availability of information used to develop, operate and support its service. It will identify business and information-security requirements, assess risks consistently and choose proportionate treatments with named owners. Leadership will provide resources and review risk decisions, progress and the performance of the ISMS.

The company commits to satisfying applicable information-security requirements and continually improving its ISMS. Staff will use approved access, protect work information and devices, and report suspected security events promptly. Suppliers handling company or customer information will be assessed and managed according to their importance and exposure.

Security objectives will be measured, reviewed and updated as services and risks change. Changes to access, systems and handling arrangements will follow documented responsibilities. Exceptions require a documented risk decision; an exception does not waive binding obligations.

Proposed approval: CEO. Status: drafted, not approved or communicated in a real organization. Planned communication: induction, annual briefing, policy repository and relevant supplier/customer extracts. Review: annually and on material context or risk changes.

## Responsibilities and separation

| Role | Accountability |
| --- | --- |
| CEO | Approves policy, resources and appetite; resolves major risk decisions; chairs management review |
| Platform Lead | Owns cloud, credentials, recovery and incident coordination; supplies technical evidence |
| Head of Engineering | Owns secure development and release practices; approves source-system business access |
| Head of Support | Owns customer-support permissions and reviews; ensures ticket confidentiality |
| People and Operations Lead | Owns HR triggers, device coordination, supplier records and obligation discovery |
| Sales Lead | Owns accurate security responses and the low-impact public-site risk |
| GRC Reviewer, exercise role | Reconciles evidence, records decisions and challenges gaps; does not approve their own access |

In the exercise, AP011's cloud administrator is independently approved by the CEO. System owners approve needed access; operators apply changes; the reviewer checks the resulting evidence. A small real team must document conflicts and arrange another competent reviewer where roles overlap.

## Three proposed objectives

| ID | Objective and measure | Owner and resources | Target and review | Present evidence |
| --- | --- | --- | --- | --- |
| OBJ01 | Review 100% of assigned human accounts in CloudConsole, SourceHub and SupportDesk; leave zero known departed users enabled; record disposition of every exception | Head of Support with Platform and Engineering owners; HR roster, approvals and exports | First operational cycle by 7 October; monthly leaver reconciliation and quarterly full review | One synthetic cycle: 27/27 reviewed; three sample corrections verified. Operational performance unknown |
| OBJ02 | Complete one isolated restore of the ticket database within 8 hours, with no more than 24 hours of lost data and successful integrity checks | Platform Lead; recovery environment and engineer time | By 7 October; repeat quarterly and after material backup changes | No restore evidence; targets are proposed and require business validation |
| OBJ03 | Record required peer approval and tenant-isolation test evidence for 100% of production releases during the first full month after workflow rollout | Head of Engineering; build configuration and reviewer time | Rollout by 6 November; review first full month by 6 December | No technical release evidence yet |

For OBJ01 and OBJ03, use the complete observed population as the denominator. Missing or incomplete exports mean the metric is unavailable. Zero releases means not applicable for that period, not 100%. For OBJ02, record actual start/end times, restored data timestamp and integrity results; a scheduled backup success does not prove recovery.

## Document and decision control

Keep document ID, version, owner and review date. Retain previous approved versions and evidence snapshots. Changes to scope, risk criteria, control selection or public claims require a recorded reason and linked updates. This release is version 1.0; it contains no actual management signatures. The source-data file and evidence manifest support traceability.

At days 30, 60 and 90, leadership should review overdue actions, evidence quality, exceptions, objective results and changes in context. Record decisions, resources and follow-up owners. A real full management review must use the complete applicable requirements; the planned checkpoints do not establish conformity.
