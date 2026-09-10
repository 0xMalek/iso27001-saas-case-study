# Service and access overview

![CaseCo service and access overview](data-flow.png)

Fictional architecture. Boundaries do not demonstrate tested isolation. This drawing describes intended access relationships; the synthetic access review records exceptions separately.

## Customer information flow

```mermaid
flowchart LR
  CUSTOMER[External customer users]
  subgraph CLOUD[A03 Production cloud - supplier infrastructure]
    APP[A02 Support application]
    DB[A01 Ticket database]
    BACKUP[A07 Database backups]
    APP <-->|Read / write customer records| DB
    DB -->|Create recovery copies| BACKUP
  end
  CUSTOMER <-->|Submit and view tickets| APP
  VISITOR[Public visitors] -->|View public pages| SITE[A10 Marketing website - separate host]
```

The marketing website has no customer login, ticket data, payments or lead forms. Backup placement describes supplier hosting; it does not prove separation from production failures or recoverability.

## Staff access and releases

```mermaid
flowchart LR
  STAFF[A08 Staff laptops] -->|Authenticate| ID[A04 Identity and access records]
  ID -.->|Approved support access| APP[A02 Support application]
  ID -.->|Approved administration| CLOUD[A03 Production cloud]
  ID -.->|Approved engineering access| SOURCE[A05 Source and builds]
  SOURCE -->|Reviewed software release| CLOUD
  SECRET[A06 Service secrets] -->|Service authentication| CLOUD
```

Solid arrows describe information, authentication or release flows; dashed arrows describe authorization. The identity box summarizes the identity service and entitlement records, not a gateway carrying every request. A06 also includes build signing secrets; this diagram simplifies that relationship.

A09 People and commercial records reside in a business document service with restricted staff access. CaseCo retains responsibility for its information, access decisions, configuration and supplier oversight.
