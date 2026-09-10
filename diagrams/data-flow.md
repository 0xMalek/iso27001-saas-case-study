# CaseCo Cloud information flow

Fictional architecture. Arrows describe information and administrative flows; they do not assert that encryption, isolation or authentication was technically tested.

```mermaid
flowchart LR
  C[Customer users] -->|Tickets and attachments| APP[A02 Support application]
  APP -->|Tenant records| DB[A01 Ticket database]
  DB -->|Recovery copies| BK[A07 Backups]
  STAFF[A08 Staff laptops] -->|Authenticate| ID[A04 Identity and entitlements]
  ID -->|Approved roles| APP
  ID -->|Approved administration| CLOUD[A03 Production cloud]
  ID -->|Approved contribution| SRC[A05 Source and builds]
  SRC -->|Reviewed release| CLOUD
  CLOUD -->|Runs| APP
  SECRETS[A06 Service secrets] -->|Service authentication| CLOUD
  STAFF -->|Restricted business records| DOC[A09 People and commercial records]
  PUBLIC[Public visitors] -->|Public content only| WEB[A10 Marketing website]
```

Customer devices and the public internet are external to CaseCo's organizational boundary. Cloud, source and document suppliers operate supporting services. CaseCo retains responsibility for information classification, access, configuration and supplier oversight. The public site is separate from service login and customer information.
