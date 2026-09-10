# Business context and ISMS scope

Document CTX-01 Version 1.0 7 September 2026 Owner: CEO role Educational simulation

## Business and operating model

CaseCo Cloud sells a customer-support application to other businesses. Customers place contact details, ticket messages and attachments in it. The company earns subscription revenue and wants to respond accurately to enterprise security questionnaires. Customer trust, reliable service and safe software changes are the main business drivers.

The assumed workforce is 10 engineering, 3 platform, 6 support, 3 sales, 2 people/operations and 1 CEO: 25 active employees. The personnel fixture also retains one former employee. Management responsibilities can be held by members of those teams; role labels do not add headcount. The GRC Reviewer is the portfolio exercise role, not an additional employee.

Staff work remotely on company laptops. A cloud provider hosts production and backups; a source-hosting supplier supports code and builds; a business document supplier holds people and contractual records. Supplier names and geography are intentionally unspecified. These are scenario assumptions, not observations of a real organization.

## Proposed scope statement

The proposed ISMS covers the development, delivery, operation and support of CaseCo Cloud's customer-support service, including customer information, source and build systems, production cloud resources, identity and access management, employee devices, relevant people and contractual processes, and the selection and oversight of supporting suppliers.

Remote work locations and interfaces to outsourced services are included in the risk assessment. Supplier infrastructure is operated by the supplier; CaseCo retains responsibility for its own configuration, access, contractual commitments and assurance. Outsourcing does not by itself make a control irrelevant.

The separate public marketing site is included as a supporting information asset with a limited availability risk. Customer organizations' internal IT and suppliers' unrelated corporate operations are outside CaseCo's organizational boundary, while security dependencies and interfaces remain in scope. No company-owned data centre or payment-card processing is assumed. Future payments or regulated data would require reassessment.

## Information classification used in this case

Public information is approved for general release. Confidential information is limited to authorized staff and suppliers with a business need. Restricted information receives the strongest handling controls in this case because disclosure or misuse could expose customer tickets, personal records, credentials or critical administration. Asset owners validate classifications and permitted sharing. A system's classification does not authorize every user to see every record inside it; tenant boundaries and role-specific permissions still apply.

The boundaries of this portfolio are narrower than that proposed organizational ISMS: it creates selected planning artifacts and one synthetic access-review cycle. See the coverage map for work still required across the management system.

## Interested parties and assumed requirements

| Party | Need or expectation | Response in this case | Validation status |
| --- | --- | --- | --- |
| Enterprise customers | Confidential tickets, controlled support access, reliable service and accurate security answers | R01-R03, R05-R09 and evidence roadmap | Assumed customer expectations; contract terms need validation |
| Employees | Appropriate access and protected people records | R04 and R11; permissions and device practices | Scenario assumptions |
| CEO and leadership | Prioritized spend, named owners and visible remaining risk | Risk method, treatment plan and 90-day roadmap | Proposed management direction |
| Cloud and software suppliers | Defined responsibilities, safe account use and agreed handling | R06, R08 and supplier review | Agreements not obtained |
| Applicable authorities | Compliance with binding information-security and privacy duties | Obligations-validation task owned by People and Operations | Jurisdiction, data locations and actual duties not determined |

No jurisdiction-specific compliance conclusion is made. Before using the work for a real company, identify establishment and processing locations, customer markets, data categories, agreements and applicable legal advice. Do not insert a named law merely because it is well known.

## Context, uncertainty and climate considerations

Internal issues: limited specialist capacity, rapid releases, manual access changes, untested recovery and incomplete supplier assurance. External issues: enterprise assurance demands, cloud concentration and dependencies on third parties.

Climate-related disruption is considered relevant in this fictional context: extreme heat, flooding or power disruption could affect cloud services or remote workers. R06 addresses the service dependency and R04 includes offsite device handling. The supplier review will check resilience information. No customer climate-related security condition is assumed; contract discovery must check for one. This records a context judgment, not an environmental certification claim. The ISO/IAF amendment guidance is linked in References.

An opportunity is to reuse reviewed security evidence in customer questionnaires. A management-system delivery risk is that the small team cannot complete the roadmap; the CEO should review capacity at each 30-day checkpoint rather than mark late actions complete.

## Information flow

See the [diagram](../diagrams/data-flow.png) and [editable flow descriptions](../diagrams/data-flow.md). Customers reach the application, which accesses the ticket database. The database feeds backups. Staff authenticate and receive role-based access to the application, cloud console and code platform. Approved code travels through the build/release path into production. People and contractual records have a separate document-service boundary.

## Review trigger

Review scope and context quarterly, and after a new market, material supplier, service feature, data type, acquisition, serious incident or major infrastructure change. The CEO owns scope approval in a real implementation; no real approval is asserted here.
