background-image: url(massey/img/bg-certus-slide.jpg)
class: background, center, middle

# MASSEY MOST.next
# Survey & Reporting Solution Upgrade Proposal
.small.center[Author: Jonathan Visser   |   Version: final v1.0]
.logo[<img src="massey/img/logo.png"/>]

---
layout: true
<div id="footer-content"><p><strong>Fresh Ideas.</strong> Exceptional Outcomes.</p></div>
---

**CONTENTS**
.box[

* Objective
* Summary
* Architectural Goals
* Solution Overview
* Scope
* Considerations & Assumptions
* Investment Ballpark]

---

class: center, red

# Objective

Develop and migrate to the next-generation MOST platform - improving the user experience, scalability, and reporting features, whilst retaining the best parts of the initial investment.

---

# Summary

The following represents some initial thoughts around objectives, scope, and effort. This is provided to help with high-level budgeting and planning only and does not represent a formal quotation.

To take this proposal forward, we recommend the following two-stage approach:

1. **Planning and design** Statement of Work, including workshops, architectural detailing, and creation of a detailed implementation project plan.
2. **Implementation and go-live** Statement of Work, including development, integration, and User Acceptance Testing, and out into pilot and production.

---

# Architectural Goals

* Unify survey tooling to Qualtrics platform to simplify support and maintenance of surveys.
* Support current reporting output, but enable self-service reporting also.
* Single-sign-on Integration.
* Increase capacity to support "every offering every time".
* Improve support for Mobile devices.

---

.tight[
# Solution Overview
]
.small[The recommended approach aligns the MOST solution to Massey's existing technology landscape - leveraging the best components for each job, whilst delivering a seamless and improved user experience.
.floatright[<img src="massey/img-massey-most-proposal/solution-overview.png" width="480px"/>]

Here are the noteable benefits:
* .bblue[Improved mobility, user-experience, and standardisation] through the use of Qualtrics to manage the surveys.
* .bblue[Increased participation rates] by reducing friction by implementing single-sign-on.
* .bblue[Enhanced insights] through the use of Microsoft's Power BI reporting solution and integration with enriching data.
* .bblue[ Increased scalability, improved maintenance, and future-proofing] are delivered by de-coupling the system into specialised standard components.
]

---

# Scope

### Stage One - Planning and Design

.grid[.left.box.small.blue[ ** ARCHITECTURE & DESIGN **
* Discover workshop to refine requirements.
* Architectural detailing:
  * Integration scoping
  * Business process design
  * Orchestration design
  * Target Platforms review
  * Data architecture ]

.right.box.small.yellow[** PROJECT MANAGEMENT **
* Creation of a detailed implementation project plan:
  * Costings
  * Schedule
  * Resource plan
]]

---

### Stage Two - Implementation

.grid[.left.box.small.green[**TECHNICAL**

* Development Environment set-up.
* Establishment of Power BI reporting data connections.
* Development of Orchestration layer.
* Integration to Qualtrics, SMS, Stream, Power BI, and any necessary 3rd-party data sources.
* Data migration.]

.right.box.small.blue[**BUSINESS ANALYSIS**

* Migration of SSRS reporting to Power BI reporting.
* Qualtrics survey establishment.
* User Acceptance Testing support.
* Support & Maintenance hand-over (technical).
* Training and hand-over (user).]
] 

.grid.x1[
.left.box.small.yellow[**QUALITY ASSURANCE & DELIVERY**
* Functional Testing.
* Technical Governance.
* Delivery Management.]
]

---

# Considerations & Assumptions
* Scaling and load-handling of Massey email server.
* Assuming that Power BI system is already established. The work here is limited to establishing data connections and to reproducing existing reports.
* Licensing is assumed to be covered already, and has not been investigated.

---

.tight[
# Investment Ballpark]
.small[These figures are necessarily high-level and are indicative only. The Planning & Design stage is necessary to lock-down scope, design, and pricing.]
.tight[

### Planning & Design]

.small.condense[
| Activity          | Estimate Hours | Estimate Investment |
| ----------------- | -------------- | ------------------- |
| Architecture & Design| .r[100-150] | .r[$18k-27k] |
| Project Planning |  .r[50-75] | .r[$9k-14k]|
| .r[**totals:**]	    | .r[**150-225 hrs**]	| .r[**NZ$27k-41k**] |
]
.tight[
### Implementation and go-live]
.small.condense[
| Activity          | Estimate Hours | Estimate Investment |
| ----------------- | -------------- | ------------------- |
| Development       | .r[500-750] | .r[90k-135k] |
| Business Analysis | .r[200-300] | .r[$36k-54k]  |
| Quality Assurance | .r[250-375] | .r[$45k-67k]  |
| Delivery Management | .r[200-300] | .r[$36k-54k]  |
| .r[**totals:**] | .r[**1,150-1,725 hrs**]| .r[**NZ$207k-310k**] |
]

---

class: center, blue

# Next Steps

Consider, and arrange Planning and Design initiation.
