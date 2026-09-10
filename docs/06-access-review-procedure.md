# Access review procedure

Document PROC-ACCESS-01 · Version 1.0 · Fictional systems: CloudConsole, SourceHub, SupportDesk

## Purpose and frequency

Determine whether assigned human access is justified by current employment, approved role and business need. Proposed operation: quarterly full review, monthly leaver reconciliation, and event-driven review for departures or role changes. This project completes one synthetic cycle, REV-01.

## Inputs and roles

Use the personnel roster, system exports and dated approvals. The exercise's approval register is the per-person role authority: it records approved role, authorizer, validity period and business reason. An observed system role is not its own approval.

System owners provide exports and explain role capabilities. People and Operations validates employment and changes. Managers approve business need, with CEO approval for E011's cloud administration. The GRC Reviewer compares the records. Operators carry out authorized changes; the reviewer checks the results. Nobody should attest their own privileged access without independent review.

## Review steps

1. Record review date, systems, population, export method and limits. Retain an unchanged copy of the original evidence. In a live review, reconcile exports to system totals and include groups, inherited privileges, local accounts and relevant exceptions. Here, only the supplied assigned human accounts are covered.
2. Match each access record to one unique personnel identity and one matching approval. Missing or duplicated identifiers require investigation; do not guess or silently discard them.
3. Check employment as of the review date. An enabled departed user is a finding. In a real environment, promptly validate and revoke access and sessions under the approved leaver process; assess whether activity needs investigation.
4. Check that the approved role is valid on the review date and matches the observed role. An unapproved or expired assignment must be investigated even if the person is still employed.
5. Examine powerful roles individually. Retain justified, independently approved privilege with rationale. Remove or downgrade privilege that exceeds approval. Do not remove every administrator simply to lower the account count.
6. Record Retain, Downgrade, Disable or Investigate for every row with rationale, reviewer and date. Link exceptions to action IDs and relevant risks.
7. Record immediate correction, cause, preventive/systemic action, owner and due date separately. A corrected account does not demonstrate that the process will prevent recurrence.
8. Obtain a fresh after snapshot, compare stable IDs and verify the exact approved role or disabled state. Recheck unaffected accounts to identify unintended changes. Record completion evidence and any remaining gaps.
9. Escalate overdue or unresolved access findings. Keep systemic actions open until implemented and their effectiveness assessed in a later cycle. Retain original and revised evidence according to the organization's approved retention rules.

## Fictional role expectations

SourceHub Developer can contribute code; Administrator can manage repository settings and permissions. CloudConsole Administrator can manage production; Operator can perform bounded operations; Viewer is read-only. SupportDesk Agent can handle ticket content; Viewer is restricted to approved business-level visibility. These simplified capabilities are assumptions for this exercise, not claims about commercial product permissions.

The approval register may allow specific exceptions, such as the designated cloud administrator. Compare both role and business reason. Disabled historical accounts are retained in the evidence population and need not be deleted to resolve access.

## Evidence and limits

Required exercise output: complete decision register, action log, before/after snapshots and follow-up report. Preserve synthetic labels. This exercise excludes service accounts, token/session revocation, groups and live technical verification; those remain scope extensions for real operation. No sample result demonstrates a breach or proves technical revocation.
