# P2P Invoice Exception Management (Freight First)

A Business Analyst portfolio case study showing how a freight invoice reconciliation problem can be understood, documented, analyzed with data, and translated into a testable solution concept.

> **Portfolio project using synthetic data.** The process automation is a proposed TO-BE design, not a deployed system. Only Project 2 includes a working data analysis: SQL queries and a Power BI dashboard. Project 3 contains design and testing artifacts; it does not include a functioning portal or application.

## The business problem

Freight invoices may differ from expected charges because of mismatched rates, accessorial fees, duplicate billing, missing shipment references, or other data issues. Reviewing exceptions manually can take time and make it harder to see what needs attention first.

This case study follows the invoice from receipt through validation, reconciliation, exception handling, and resolution. It explores how a clearer process and useful exception reporting could help a finance or accounts payable team review discrepancies consistently.

## Project journey

The work is organized as three portfolio projects across a 56-days. The day ranges below describe the planned sequence, not a claim about production delivery.

### Project 1 — Discover and define (Days 3–28)

**Focus:** Business analysis documentation and process design. No software is built in this phase.

Activities and artifacts:

- Define the problem, objectives, scope, stakeholders, assumptions, and success measures.
- Map the current-state (AS-IS) freight invoice reconciliation process.
- Identify pain points, handoffs, business rules, risks, and exception scenarios.
- Develop a proposed future-state (TO-BE) process showing where automation could support the work.
- Document requirements, process flows, and traceability from business needs to proposed capabilities.

The TO-BE automation is a design on paper. It is not an implemented workflow.

### Project 2 — Analyze synthetic invoice data (Days 29–42)

**Focus:** A small, working analytics deliverable using synthetic data.

Planned scope:

- One synthetic dataset representing freight invoices and related reconciliation details.
- Approximately 15 SQL queries to profile, reconcile, and investigate invoice exceptions.
- A two-page Power BI dashboard to summarize reconciliation outcomes and highlight exceptions for review.

The queries and dashboard demonstrate how analysis can support the process. They do not connect to a real carrier, ERP, or finance system. If time is limited, the minimum version is 10 queries and one dashboard page; polish can be reduced without extending the planned timeline.

### Project 3 — Specify and validate a solution concept (Days 43–56)

**Focus:** Delivery-ready analysis and design artifacts. No code or working system is built.

Activities and artifacts:

- Convert requirements into Jira-style epics, stories, and acceptance criteria.
- Create Figma wireframes illustrating a possible invoice exception review portal. The screens are visual concepts and are not functional.
- Write test cases for key scenarios, including expected outcomes and exception handling.
- Link business needs, requirements, stories, designs, and tests to show how a team could validate a future implementation.

## End-to-end lifecycle represented

1. **Receive** a freight invoice and identify the shipment or service it relates to.
2. **Validate** required invoice details and compare charges with available reference information and business rules.
3. **Reconcile** expected and invoiced amounts; classify mismatches and other exceptions.
4. **Review and resolve** exceptions through the appropriate business process, documenting decisions and outcomes.
5. **Report and improve** by analyzing exception patterns, turnaround, and reconciliation results.

These steps describe the business process being analyzed. The portfolio artifacts explore and illustrate them; they do not execute this lifecycle in a live environment.

## Scope boundaries

**Included**

- Business analysis documents, process diagrams, and requirements.
- Synthetic data analysis using SQL and Power BI.
- Jira-style stories, Figma wireframes, and test cases.

**Not included**

- Production deployment or operational use.
- Integration with real ERP, carrier, or payment data.
- A custom application or functional invoice portal.
- Automated payment, approval, or exception resolution.

An optional, small proof of concept could flag likely duplicate invoices in the synthetic data with Python or Power Automate. It is a bonus only; it is not required for the project and is not part of the core scope.

## Tools and methods

- **Business analysis:** stakeholder analysis, requirements elicitation, process mapping, gap analysis, business rules, traceability, acceptance criteria, and UAT planning.
- **Data analysis:** SQL and synthetic data.
- **Visualization:** Power BI.
- **Delivery artifacts:** Jira-style backlog, Figma wireframes, and test cases.



##repository structure for your reference

```text
project-1-discovery-and-process/
  README.md
  requirements/
  process-maps/

project-2-data-analysis/
  data/                 # synthetic data only
  sql/
  power-bi/

project-3-solution-concept/
  user-stories/
  wireframes/
  test-cases/
```

## Disclaimer!!

This is a learning and portfolio case study. All sample data should be synthetic. The process, requirements, and interface concepts are illustrative and would need stakeholder validation before use in a real organization.
